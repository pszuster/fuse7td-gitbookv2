# Create an API Connector

{% hint style='info' %}
The API Connector is a "meta-connector" that can be used to create multiple connectors. To do this, you only need a valid swagger document that properly describes the REST API.
{% endhint %}

* Click on the  **`Customizations`** tab.
* Click on the **`Create API Connector`** button.

![](../.gitbook/assets/image%20%2860%29.png)

* Click on the **`Choose File`**button.
* Select **`Lab4/contract_api.json`**.
* Click on the **`Next`** button.

![](../.gitbook/assets/image%20%2814%29.png)

* Click on the  `Next` button.

![](../.gitbook/assets/image%20%2868%29.png)

{% hint style="info" %}
Ignite parses the swagger document, and identifies all the available operations. 

More info about  swagger: [https://swagger.io/](https://swagger.io/)
{% endhint %}

* Click on the **`Next`** button.

![](../.gitbook/assets/image%20%2827%29.png)

* Enter the following values:

| **Parameter** | **Value** |
| --- | --- | --- | --- |
| **Connector Icon** | &lt;click on the **Choose File** button and select **Lab4\opencrx.gif&gt;** |
| **Connector Name** | OpenCRX |
| **Description** | OpenCRX API |
| **Host** | http://opencrx.opencrx.svc.cluster.local|

* Click on the `Create API Connector` button.

![](.gitbook/assets/Selection_273.png)



