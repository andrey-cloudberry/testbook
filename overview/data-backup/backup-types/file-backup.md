## File-level Backup in CloudBerry Backup

The most commonly used type of backup in CloudBerry Backup is file-level backup. It essentially allows you to back up individual files from your computer to the backup destination \(local or cloud storage\). This is great for backing up important project files, source code, personal documents, photos, presentations, Microsoft Office documents, and so forth. This type of backup is mainly designed to ensure that your most sensitive and important information is regularly backed up and therefore not vulnerable in the event of hardware malfunction or ransomware strike.

We do not recommend using file-level backup to back up your entire storage device. For this purpose, [image-based](/overview/data-backup/backup-types/image-based-backup.md) backup is a better choice, and we suggest you take a look at it down in the section.

File-level backup can be configured in the so-called _Backup Wizard_ by clicking on the _Files_ button on the main toolbar or by using the _Ctrl+B_ shortcut.

![](/assets/backup1.png)

The Backup Wizard will appear, prompting you to configure the backup plan. The first step is to indicate whether you want to perform backup just to a local or cloud storage or whether you want to use [**Hybrid Backup**](/overview/data-backup/backup-types/hybrid-backup.md)** **to back up data simultaneously to a local and a cloud storage.

Optionally, you can enable ransomware protection so that our app will automatically flag potentially ransomware-encrypted files.

![](/assets/wizard1.PNG)

If you selected _Hybrid Backup_, first specify the local storage that will be used to store the backup. If this is the first time you're setting up a backup plan, click **Add New Account** to add a local storage.

![](/assets/wizard2p.PNG)

Enter the display name and path for the storage and click **OK**.

![](/assets/wizard3.PNG)

Next, specify the desired cloud backup storage. Again, if this is the first time you're setting up a backup plan, click **Add New Account** to add a cloud storage.

![](/assets/wizard4.PNG)

As you can tell, we support the vast majority of cloud storage services on the market. Locate your storage and double-click on it. We'll go with Amazon S3 in this tutorial, as it is by far the most popular cloud storage on the market.

![](/assets/wizard5.PNG)

In the freshly appeared window, specify your credentials: **the display name**, **access key,** and **secret key**. Finally, specify the bucket name and click **OK**.

![](/assets/wizard6.png)

Enter the plan name and click **Next**.

![](/assets/wizard7.PNG)

Select the required advanced options and click **Next**.

![](/assets/wizard8.PNG)

Specify the files and folders you'd like to back up and click **Next**.

![](/assets/wizard9.PNG)

In the next step you can specify which files should be skipped and a number of other options.

![](/assets/wizard10.PNG)

Now you can enable compression and encryption. CloudBerry Backup supports up to 256-bit military grade encryption by default. Similarly, you can enable Server Side Encryption on S3. Note that we don't store the key anywhere for security purposes. If you forget it, the data is permanently gone.

![](/assets/wizard11.PNG)

The next step is retention policy configuration. You can indicate if you want to delete versions older than a pre-defined number of days from the modification or backup date. Similarly, you can explicitly determine the number of versions of each file to be retained on the storage.

![](/assets/wizard12.PNG)

Next up is scheduling. Here you can set the required schedule with various parameters like frequency, recurrence, immediate resumption of the plan following the computer restart, and the like.

![](/assets/wizard13.PNG)

To ensure that you can at any point revert to the older versions, it is recommended to perform full backup every now and then. You can schedule full backup with the required frequency and even enforce it when the size of block-level backup exceeds the specified threshold.

![](/assets/wizard15.PNG)

Next, specify the optional pre- and post-actions. These are essentially scripts that can be executed prior to and immediately following backup. For instance, you can run a script that turns off the computer when the backup plan completes executing. Alternatively, you can run a script that, say, disables all incoming connections during the plan execution. Backup chain allows you to automatically trigger another backup plan when the current one completes.

![](/assets/wizard16.PNG)

Finally, you can configure email notifications to be notified of backup plan executions and failures. We even support custom SMTP servers if you use one of those. Also available is optional detailed reporting.

![](/assets/wizard17.png)

Review the plan's summary and click **Next**.

![](/assets/wizard18.PNG)

Select the _Run backup now_ checkbox and click **Finish**, at last.

![](/assets/wizard19.PNG)

The Backup Wizard will be closed, and the backup plan will start executing. In the meantime, you can observe the backup process in the green progress bar in the dedicated dashboard section.

![](/assets/wizard20.PNG)

That's it! When the plan completes, you will be notified over email about the status \(granted you've enabled notifications\). If you've enabled scheduling, the plan will recurrently execute without you having to open the app or click any buttons. Close the app and feel certain that your files are regularly backed up and impervious to any cyber maleficence.

