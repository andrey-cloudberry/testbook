## Hybrid Backup in CloudBerry Backup

Following the best practices in the backup industry unquestionably demands some sort of combination of local and cloud backup. With that in mind, many of our users choose to configure at least two different backup plans—one for local and another for cloud backup. This approach is  not particularly efficient in that it puts extra workload on the utilized computer. First, the files are uploaded from the computer to the local storage—let's say a local NAS—and then the same process repeats to upload the files from the computer to the cloud storage. A more sensible approach here would be to first transfer the files to the NAS and then upload them from the NAS to the cloud. That would give some relief to the main computer, requiring less disk operations. The Hybrid Backup combines those aforementioned two backup plans into one which naturally makes it easier to do the setup process. Further, encryption and compression are only performed once during the initial backup to the local storage. The already encrypted and compressed files are then uploaded to the cloud storage.

Hybrid backup is available for **all types of backup**. 

### Setting up Hybrid Backup

The Backup Wizard in CloudBerry Backup 5.6 immediately asks you if you want to configure a hybrid or merely a local or cloud backup. Select **Hybrid Backup **and click **Next**.

![](/assets/screen1-3.png)

Now select the required local storage.

![](/assets/screen2-5.png)

Proceed to specify the cloud storage.

![](/assets/screen3-4.png)

The remaining steps are identical to the steps of a regular backup plan. Conclude configuring the plan and execute it upon finishing.

Also, note that currently filename encryption is not supported.

