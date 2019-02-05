In-Progress Document

Receipt of Drives

Check that all tapes were digitized and titles received by comparing folder file names to object identifiers in FileMaker export.
If receiving multiple drives, label each drive with the files (i.e. range of object IDs) on each drive.
Check all checksums using md5 tool. Flag any files with checksum failures.


QC

Mount hard drive as read only.
Terminal commands:
diskutil list to find where drive is mounted
diskutil unmountDisk /dev/disk2 (<---example location only)
diskutil mountDisk readOnly /dev/disk2  (<---example location only)

Do we want to check any particular technical specifications for files to ensure that vendor is meeting requested specs? Using a script, MediaConch, eyeballing?  

Have we asked for vendor to embed files with any particular metadata? I know Media Preserve embeds files for California Revealed -- in our case, I imagine it could be worthwhile to embed Title, Creator (TVTV for all), Date (just year?), and we could also include the Accession Number as a Comment.

Check that all file states (e.g. uncompressed preservation master, access H264, ProRes file, xml, photo) were received for each item. Verify files and folders are named correctly according to naming conventions.

Find correlating record in FileMaker database.
Under Technical Details tab, add relevant data re: Sound Characteristics, Color Characteristics, and Running Time. (Anything else?)
Under In-house Comments tab, copy over any vendor notes from vendor’s xml metadata. (E.g. Item # 16134 from Media Preserve: “Aligned Playback Level to program; Aligned Audio Level to program; Flagging visible in picture; Unstable Control Track; Channel2 Silent; Channel2 Mono”)

Play preservation files in Adobe Premiere, at least 90 seconds at beginning, middle, and end of recordings. Slowly scrub file back and forth (approx. 1 minute).

Add QC notes under In-house Comments tab.
Note any digital artifacts or other problems that may have been introduced in the transfer process.
Notes about inherent image/sound quality issues that would negatively impact user experience?
Conversation needed with Dave as to what issues to flag for possible image/audio correction.
Notes about content: significant personages, events, locations, or discrepancies with physical label descriptions.

Should we do any QC for H264 access files or ProRes files - or not if we’re not actually keeping those files?
MCQ Suggestion: Just ensure they are complete and correctly identified (i.e. useful for quick access).

After QC

For files flagged for possible image/audio correction: Conversation needed with Dave
For files with possible digital artifacts introduced in transfer or other problems requiring vendor attention: Flag to contact vendor for review. Still ingest as is?
For files without flags: Conversation/training needed for ingest procedures.

Procedure for making access copies available to Steve and others? Upload vendor-provided access copies to Box?
