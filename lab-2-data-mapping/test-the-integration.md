# Test the integration



* Wait until the integration is published:

![](../.gitbook/assets/image%20%28108%29.png)

* Go to **http://ftp.apps-&lt;GUID&gt;.generic.opentlc.com**
* Click on **`Advanced Login`**
* Enter the following values:

| Host | vsftpd.ftp.svc.cluster.local |
| --- | --- | --- | --- | --- |
| Port | 21 |
| Username | admin |
| Password | password |
| Passive mode | Checked |

* Click on the **`Login`** button.

![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LDgEtlo1zua2etnJvxn%2F-LDngljqU3as7X5EMh1K%2F-LDnhY6bbRbRgEDYlMJS%2Fimage.png?alt=media&token=49f765c7-7436-420e-a724-02d4aeb4210f)

* Click on the **`incoming`** folder.
* Click on the **`Upload`** button.

![](../.gitbook/assets/image%20%2823%29.png)

* Upload **Lab2\customer.xml** to the FTP server.
* Click on the **`Submit`** button.

![](../.gitbook/assets/image%20%28132%29.png)

* Click on the **Back** arrow button.
* Go back to **Fuse Ignite** console.
* Click on the **`Activity`** tab.

![](../.gitbook/assets/image%20%28110%29.png)

{% hint style="info" %}
You can see a detail of every processed message
{% endhint %}

* Click on the **`Metrics`** tab.

![](../.gitbook/assets/image%20%2829%29.png)

* Open a browser tab and go to your dropbox.com account.
* Go to **`My Files -> Apps -> IgniteApp`**
* There should be a **`customer.json`** file.

![](../.gitbook/assets/image%20%2893%29.png)

* Double-click on the file to see its contents.

![](../.gitbook/assets/image%20%2862%29.png)



