# Send an AMQ message.

* Go to https://fuseignite-{{ book.guid }}.generic.opentlc.com:8443/console/project/amq/overview
* Login as **admin/admin.**
* Click on the blue circle.

![](../../.gitbook/assets/image %2895%29.png)

* Click on the `Open Java Console` link.

![](../../.gitbook/assets/image %282%29.png)

* Click on the `User`icon -&gt; `Preferences`**.**

![](../../.gitbook/assets/image %28151%29.png)

* Click on the **ActiveMQ** tab.
* Enter the following values:

| Parameter | Value |
| --- | --- |
| **Activemq user name** | admin |
| **Activemq password** | password |

* Click on the `Done` button.

![](../../.gitbook/assets/image %28179%29.png)

* Click on the `invoices` queue.
* Click on the `Send` tab**.**

![](../../.gitbook/assets/image %2865%29.png)

* Paste the contents of **Labs\lab5\invoices.xml** .

{% hint style='danger' %}

Make sure to select invoiceS.xml and not invoice.xml

{% endhint %}



* Make sure **Payload Format** is set to `XML`.
* Click on the `Send message` button.

![](../../.gitbook/assets/image %28176%29.png)

