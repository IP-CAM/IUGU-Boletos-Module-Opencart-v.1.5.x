# IUGU - OpenCart Module for Boletos

## Installation

Module Developed by Felipo Antonoff Araújo - http://www.codemarket.com.br

Step 1) Send the Folders to the root of your Store:
admin, catalog, image, system and vqmod

Step 2) If I need permissions on the folders sent, if the hosting is configured correctly it will not be necessary

Step 3) Enter the Store Administrator and go to System -> Users -> User Groups
Click Edit on your User Group, usually the Administrator and Access and Modification permission for payment / iugu_bankslip
You can click Check all to give general permission and then click Save
Step 3 is sometimes not necessary.

Step 4) Still within the Store Administrator, go to Extensions -> Payment Methods and Search for iugu Boleto, then on its line click Install

Step 5) Now click on Edit, ready configure the Module with the iugu Token and the other options

## Test

Make a simulation of purchase in the Store and see if the Boleto Boleto payment appears, remembering that you can edit its name in the Module panel and then
proceed with the purchase.
You can use the Geradi test Token on iugu, if you just want to simulate a purchase

## Return of Status

The return is automatic, the Module already informs the iugu the return URL, also remember to install vQmod 2.3 or later
http://www.codemarket.com.br/opencart/modulos-gerais/vqmod-ferramenta-essencial
It is free and important for the use of several modules, as it changes files without touching them directly, being easier to maintain so

In the case of iugu Boleto, you need vqmod, as it accompanies a completely friendly URL xml, it places a general friendly URL in the store, because by default
Opencart only places it in some places, you need this active xml, because iugu's notification URL only gets if it is friendly

Therefore, for Return, take one more step, activate the Friendly URL of the Store and check if the address:
sualoja.com.br/iugu-boleto-notificar a white screen appears, if it appears it is right

If you already have a general friendly URL module, disable it or Felipo-SEO-URL.xml, otherwise it may cause conflict between them
If you disable Felipo-SEO-URL.xml, remember to configure the following URL in the other Module:
'payment / iugu_bankslip / callback' => 'iugu-boleto-notificar',

## License

The Module license is the GPL 3, therefore it is a free module and can be used in several stores, but without profit, any product derived from it, must
also be GPL 3 and therefore free, it does not charge its customers for it, but for its installation, configuration and testing services
For more details about it, visit - http://www.gnu.org/licenses/

If you want paid support for this module or other modules for Opencart, visit - http://www.codemarket.com.br 
