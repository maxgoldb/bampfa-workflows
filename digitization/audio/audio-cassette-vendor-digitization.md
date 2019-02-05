# Workflows for processing audio tapes for vendor digitization (Work In Progress)

This workflow document was created for a 2018-2019 CLIR audio digitization project. Its scope includes 750 audiotapes that will be digitized by MediaPreserve. The majority of these have database [records](https://github.com/BAM-PFA/audio-database-merge) with at least minimal descriptive metadata. The cassettes also generally have paper forms with release/permission information, which will be added as applicable to database records.

## Tape prep workflow

Tapes will be pulled in 3 batches for digitization at MediaPreserve. Their  shipping cases fit 112 tapes per tote, so the batches will be in multiples of 112 (or 56 since there are two 56-tape boxes in the tote). Tapes will be pulled and digitized in reverse chronological order.

* Project assistant pulls tapes from the vault
* Last tape number is approximately #829
* Check that tape label and cassette jacket match each other
* Check database:
  * Make sure that each record for a given tape number matches the data on the tape label
  * Look for release form by date in the paper folders
  * Check the `PermissionsLegacy` and `Permissions` fields for a tape record and update as needed based on the paper form:
    * 1 = "Do not record" (there shouldn'e be a tape at all)
    * 2 = "analog partial permissions"
    * 3 = "analog full permissions"
	  * In this case also update the `Permissions` drop down to be "Online plus in-house full access"
  * Enter or correct data that is missing or wrong
  * Enter date shipped for digitization
  * Enter MediaPreserve as Digitizer
* Create a manifest that includes records marked with a particular digitization shipping date
  * Use [these instructions](openrefine-shipping-manifest-instructions.pdf)!
* Pack the tapes and paper manifest
* Ship them FedEx 3-day
* Notify vendor that tapes are in transit


## Receiving tapes & files
Tapes will be received in the same batches as they were originally shipped.

* Check that tapes returned match those on the original shipping manifest
* Check that each cassette and case match
* Mount hard drive received from vendor as read-only
  * Check that file names received from vendor match object IDs specified on manifest
    * Manifest specifies an A-side filename for each tape
    * Check for at minimum an A-side file for each
  * Transfer copy of directory tree to the MediaVault NAS
    * `rsync -arv -p chmod=rwx ./ -e ssh "user@1.2.3.4:/path/to/mediavault/CLIR"`
  * Make local copies on the project assistant computer
    * Each preservation master file should come with a sidecar md5 checksum file
    * Use a tool like [md5tool](https://github.com/cavpp/md5tool/blob/master/md5tool.py) to compare the local copy with the vendor-provided checksum
    * We may end up using a similar script or simply calling `md5` on the files
    * In any case, if any files transferred unsuccessfully locally, transfer them again
* Any discrepancies between manifest and hard drive or shipping tote contents should be reported to staff and vendor immediately
* Because we provided the vendor only with A-side details in the manifest, the project assistant may need to create new database records for additional events recorded on B-side

## QC
* Run preservation master files against MediaConch policy (TBD..)
  * note any discrepancies and contact vendor immediately in cases where a transfer was not made with correct specs
* Add vendor comments from xml file to Digitization Notes field in DB record for a given file
* Open vendor copy of preservation master file in WaveLab (TBD if this is really going to be our method) and run the Interstitial Error Check tool to search for possible digitization-related errors
* Play through several seconds of beginning, middle, and end of file and look over waveform to check for any potential volume issues (periods of low or too-high volume, etc.)
* Add QC notes to DB record for recording
* Once each file has been verified to correspond to an existing database record, rename the local preservation master files to include the database record ID for later metadata matching
  * Use rsync to copy these QC'ed and renamed files to the NAS for temporary backup until the files are confirmed fully ingested and delete the first copy
* The masters are now ready for ingest


## File ingests
* use `rsync` to transfer files to the `EDITH` server
  * This can be done as a batch:
    * running from the directory of preservation masters--`rsync -arv -p chmod=rwx ./ -e [destination]`
  * Or file by file:
    * `rsync -av -p chmod=rwx -e ssh [source file] [destination]`
* From the `EDITH` ingest screen select the file you want to ingest and select `audio database` as the Metadata Source
* Wait for the ingest to finish! It should be posted to ResourceSpace when the process is done. Search for the files you expect from the manifest and check off successfully ingested files.


## Specs
File formats:
* Preservation master:
  * 24-bit, 96kHz Broadcast Wave Format (BWF)
* Mezzanine:
  * 16-bit, 44.1kHz Broadcast Wave Format (BWF)
* Access copy (for intermediate use only; digital repository will create its own access copies)
  * MP3
