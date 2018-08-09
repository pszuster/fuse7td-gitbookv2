# Create an AMQ to API integration

* Click on the `Integrations` tab.
* Click on the `Create Integration` button.

![](../.gitbook/assets/image %2881%29.png)

* Select `AMQ Broker` as the start connection.
* Select the `Subscribe for messages` action.

![](../.gitbook/assets/image %28137%29.png)

* Enter the following values:

| Parameter | Value |
| --- | --- |
| **Destination name** | invoices |
| **Destination Type** | Queue |

* Click on the `Next` button.

![](../.gitbook/assets/image %28162%29.png)

* Click on the `Done` button.
* Select the `OpenCRX` connection.
* Select the `POST /invoice` action**.**

![](../.gitbook/assets/image %2819%29.png)

* Click on the `Done` button**.**
* Hover over the **+** icon and click on the  **Add a Step** link.
* Select the **Log** step.

![](../.gitbook/assets/image %28146%29.png)

* Check `Message Body`.
* Enter "`INVOICE`" as **Custom Text.** 
* Click on the `Done`  button.

![](../.gitbook/assets/image %28125%29.png)

* Hover over the **+** icon \(below **LOG**\) and click on the **Add a Step** link.
* Select the `Split` step.
* Enter the following values:

| Parameter | Value |
| --- | --- |
| **Expression** | //invoice |
| **Language** | xpath |

* Click on the `Done` button.

![](../.gitbook/assets/image %2878%29.png)

{% hint style='info' %}
The Split step will separate the elements in the incoming list using the expression/language and execute each of the following steps in the integration for each element.
{% endhint %}

* Hover over the **+** icon \(below **SPLIT**\) and click on the `Add a `**`connection`.**
* Select `DataShape` connector.
* Select the `Datashape Endpoint` action.
* Click on the `Next` button.
* Select `XML Instance` as the **Output Data Type.**
* Copy and paste the contents of **Labs\lab5\invoice.xml** into the definition field.
* Enter`InvoiceXML` as the **Data Type Name.**
* Click  on the `Done` button.

![](../.gitbook/assets/image %2888%29.png)

{% hint style='info' %}
Since we want to map the output of the Shapeless Split step to the API call, we need to define what is the output of the Spit step like. For that we use the imported "Datashape" extension.
{% endhint %}

* Click on the **warning** icon in the **finish** connector.
* Click on the `Add a data mapping step` link.

![](../.gitbook/assets/image %2880%29.png)

* Expand **InvoiceXML** -&gt; **invoice** in the **Source** data structure.
* Expand **Request -&gt; body -&gt; org.opencrx.kernel.contract1.Invoice** in the **Target** data structure.

![](../.gitbook/assets/image %2843%29.png)

* Perform the following mappings:

| Source | Target |
| :--- | :--- |
| invoiceDescription | description |
| invoiceName | name |
| @number | contractNumber |
| totalAmountIncludingTax | totalAmountIncludingTax |
| totalBaseAmount | totalBaseAmount |
| totalTaxAmount | totalTaxAmount |

![](../.gitbook/assets/image %2884%29.png)

* Click on the **+** icon in the `Constants` tab.

![](../.gitbook/assets/image %28116%29.png)

* Enter the following:

| **Value** | true |
| --- | --- |
| **Value Type** | Boolean |

* Click on the `Save` button.

![](../.gitbook/assets/image %2898%29.png)

* Click on the `true` constant and map it to `noAutoRecalc`.

![](../.gitbook/assets/image %28124%29.png)

* Click on the `Done` button.
* Click on the `Publish` button.
* Enter **"**`AMQtoAPI`**"** as integration name.
* Click on the `Publish` button.



