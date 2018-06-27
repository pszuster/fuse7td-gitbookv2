# Create FTP to FTP Integration

* Click on the **`Integrations`** tab.
* Click on the **`Create Integration`** button.

![](../.gitbook/assets/image%20%28166%29.png)

* Select **Openshift FTP** as the starting connection for the integration.

![](../.gitbook/assets/image%20%2826%29.png)

* Select the only available action: **Download**.

![](../.gitbook/assets/image%20%28106%29.png)

* Enter the following values:

| File name expression | file1.xml |
| --- | --- | --- |
| FTP directory | incoming |
| Delete file after download | Yes |

* Click on the **`Next`** button.

![](../.gitbook/assets/image%20%2834%29.png)

* Click on the **`Done`** button.

![](../.gitbook/assets/image%20%28153%29.png)

* Select **Openshift FTP** as the finish connection.

![](../.gitbook/assets/image%20%28157%29.png)

* Select the only available action: **Upload**.

![](../.gitbook/assets/image%20%28128%29.png)

* Enter the following values:

| File name expression | ${date:now:yyyyMMdd}.xml |
| --- | --- |
| FTP directory | outgoing |

* Click on the **`Next`** button.

![](../.gitbook/assets/image%20%28127%29.png)

* Click on the **`Done`** button.
* Click on the **`Publish`** button.

![](../.gitbook/assets/image%20%2863%29.png)

* Enter **`FTP to FTP`** as the integration name.
* Click on the **`Publish`** button.

![](../.gitbook/assets/image%20%28123%29.png)

{% hint style="info" %}
After ~5min the deployment of the integration should be done.
{% endhint %}

![](../.gitbook/assets/image%20%2896%29.png)

