## How does backup work?

CloudBerry Backup is one of the leading backup solutions on the market. Its simplicity and versatility allow you to perform just about any type of backup. In this section we explain the essence of different backup types supported in our solution. But first let us briefly explain to you how the underlying backup process occur.

The main entity of CloudBerry Backup is a _backup plan_. A backup plan represents a record that contains the following information: what to back up, where to back up, how to back up, when to back up, and a number of other attributes like compression, encryption, and email notifications. Once you've configured a backup plan, it'll automatically execute according to the schedule. You don't have to manually start it or even keep CloudBerry Backup running. Our system service takes care of everything, and so you can literally just forget about backups — CloudBerry Backup will do all of it for you.

Here's a typical list of backup plans that users might have:

1. A backup plan that performs daily file-level backup of the documents folder to Amazon S3. Compression, encryption, and ransomware protection are enabled.  
2. A backup plan that performs weekly image-based backup of the entire disk to Amazon S3. Encryption is enabled while compression is disabled.
3. A backup plan that performs monthly backups of old files to Amazon Glacier \(archive storage\). Encryption and compression are enabled. 

![](/assets/backupTypes2.png)

That's how our product looks in action. Now that we've given you a sneak peek of backup types, let's go ahead and examine each in detail.

