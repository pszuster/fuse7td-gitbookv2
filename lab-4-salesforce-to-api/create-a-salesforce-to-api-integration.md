# Create a Salesforce to API integration

* Click on the **`Integrations`** tab.
* Click on the **`Create Integration`** button.
* Choose **IgniteSalesforce** as  start connection.
* Select **`On Create`** action.
* Select **`Lead`** as **`Object Name`**.
* Click on the **Done** button.

![](../.gitbook/assets/image%20%2841%29.png)

* Select **`OpenCRX`** as finish connection.
* Select **`POST /lead`** as action.

![](../.gitbook/assets/image%20%28109%29.png)

* Click on the **`Done`** button.

![](../.gitbook/assets/image%20%28114%29.png)

* Hover over the **+** icon between start/finish connections.
* Click on the **Add a Step** link.

![](../.gitbook/assets/image%20%284%29.png)

*  Select **Data Mapper**.
* Perform the following mappings:

| **Source** | **Target** |
| --- | --- | --- | --- |
| Description | description |
| Id | contractNumber |
| Company | name |

* In the **Company -&gt; name** mapping details, select **`Combine`** action.
* Select **`Dash`**`[-]`**Separator.**

![](../.gitbook/assets/image%20%2813%29.png)

* Hold **`Ctrl`** key and click on the **`ProductIterest_c`** **Source** field.

![](../.gitbook/assets/image%20%2853%29.png)

* Click on the **`Done`** button.
* Click on the **`Publish`** button.
* Enter **`SalesforceToAPI`** as **Integration Name**.
* Click on the **`Publish`** button.



