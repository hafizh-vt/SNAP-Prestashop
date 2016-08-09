
Midtrans Prestashop Payment Gateway Module
=====================================


Midtrans :heart: Prestashop!
Let your Prestashop store integrated with Midtrans payment gateway.

### Description

Midtrans payment gateway is an online payment gateway. They strive to make payments simple for both the merchant and customers. With this plugin you can allow online payment on your Prestashop store using Midtrans payment gateway.


### Installation Instruction

#### Minimum Requirements

* Prestashop 1.6 or greater
* PHP version 5.4 or greater
* MySQL version 5.0 or greater

1. [Download](/archive/master.zip) the modules from this repository.
2. Extract the modules, then rename the folder modules as **midtranspay** and zip this modules as **midtranspay.zip**
3. Go to your Prestashop administration page and go to **"Modules and Services > Modules and Services"** menu.
4. Click on the **"Add a new module"** and locate the **midtranspay.zip** file, then upload it.
5. Find the **Midtrans Pay** module in the module list and click **install**, then enable it.
6. Find the **Midtrans Pay** module in the module list and click **configure**
  * Fill **Payment Button Display Title** with text button that you want to display to customer
  * Select **Environment**, Sandbox is for testing transaction, Production is for real transaction
  * Fill in the **client key** & **server key** with your corresonding [Midtrans account](https://my.veritrans.co.id/) credentials
  * Note: key for Sandbox & Production is different, make sure you use the correct one.
  * **Map payment SUCCESS status to:** select your desired order status when payment is success.
  * **Map payment FAILURE status to:** select your desired order status when payment is failure.
  * **Map payment CHALLENGE status to:** select your desired order status when payment is challanged.
  * Other configuration are optional, you may leave it as is.


### Midtrans MAP Configuration

1. Login to your [Midtrans Acount](https://my.veritrans.co.id), select your environment (sandbox/production), go to menu `settings > configuration`
   * Payment Notification URL: `http://[your-site-url]/index.php?fc=module&module=midtranspay&controller=notification`
   * Finish Redirect URL: `http://[your-site-url]/index.php?fc=module&module=midtranspay&controller=success`
   * Unfinish Redirect URL: `http://[your-site-url]/index.php?fc=module&module=midtranspay&controller=back`
   * Error Redirect URL: `http://[your-site-url]/index.php?fc=module&module=midtranspay&controller=failure`

#### Get help

* [Veritrans sandbox login](https://my.sandbox.veritrans.co.id/)
* [Veritrans sandbox registration](https://my.sandbox.veritrans.co.id/register)
* [Veritrans registration](https://my.veritrans.co.id/register)
* [Veritrans documentation](http://docs.veritrans.co.id)
* [Veritrans Prestashop Documentation](http://docs.veritrans.co.id/vtweb/integration_prestashop.html)
* Technical support [support@veritrans.co.id](mailto:support@veritrans.co.id)