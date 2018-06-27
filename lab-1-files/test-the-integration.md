# Test the integration

* Go to **http://ftp.apps-{{ book.guid }}.generic.opentlc.com**
* Click on **`Advanced Login`**
* Enter the following values:

| Parameter | Value |
| --- | --- | --- | --- | --- |
| Host | vsftpd.ftp.svc.cluster.local |
| Port | 21 |
| Username | admin |
| Password | password |
| Passive mode | Checked |

* Click on the **`Login`** button.

![](../.gitbook/assets/image%20%2817%29.png)

* Click on the **`incoming`** folder.
* Click on the **Upload** button.
* Upload **Labs\Lab1\file1.xml** to the FTP server.

![](../.gitbook/assets/image%20%28172%29.png)

* Click on the **`Submit`** button (green arrow).

![](../.gitbook/assets/image%20%2864%29.png)

* Click on the **Back** (blue) arrow button.
* Navigate to the **Outgoing** folder.
* You should have a file with the current date as filename.

![](../.gitbook/assets/image%20%28145%29.png)

* Go back to **Fuse Ignite**  console.
* Click on the **`Integrations`** tab.
* Click on the **`Activity`** tab.

![](../.gitbook/assets/image%20%28156%29.png)

{% hint style="success" %}
Notice that there's been one activity in the deployed integration
{% endhint %}

* Click on the **`Metrics`** tab.

![](../.gitbook/assets/image%20%28163%29.png)

{% hint style="success" %}
In the metrics section, you can see one message has been processed by the deployed integration.
{% endhint %}

