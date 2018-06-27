# Import "CSV to JSON" Extension

* Click on the **`Customizations`** tab.
* Click on the **`Extensions`** tab.
* Click on the**`Import Extension`** button.

![](../.gitbook/assets/image%20%2871%29.png)

* Click on the **`Choose File`** button and select**`Labs\Lab6\csvtojson-1.0.0.jar`** .
* Click on the **`Import Extension`** button.

![](../.gitbook/assets/image%20%28122%29.png)

{% hint style="info" %}
You can augment Fuse Ignite capabilities through the creation of extensions developed in Java or Camel routes.
{% endhint %}

* This imported extension was developed using Apache Camel, in JBoss Developer Studio, where there is a visual tool to do this.

![](../.gitbook/assets/image%20%2850%29.png)

1. Receive CSV message.
2. Parse CSV according to the column list parameter.
3. Transform parsed CSV to JSON.



