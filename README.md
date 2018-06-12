# WPP Integration demo
This a sample integration of WPP into your e-shop via JSON in Java. 
## Requirements
* JDK 1.8
* Maven
## Properties
```
#eshop backend app port
server.port=8080
#elactic engine username
ee.username=70000-APIDEMO-CARD
#elactic engine password
ee.password=ohysS0-dvfMx
#wirecard payment page host
wpp.host=https://wpp-test.wirecard.com
#wirecard payment page app port
wpp.port=443
#wirecard payment page app url
wpp.url=${wpp.host}:${wpp.port}
#rest service endpoint for register payment
wpp.rest.payment.register.endpoint=${wpp.url}/api/payment/register
#wirecard payment page loader lib
wpp.paymentpageloader=${wpp.url}/loader/paymentPage.js
#wirecard payment page merchant id
wpp.maid=7a6dd74f-06ab-4f3f-a864-adc52687270a
#wirecard payment page merchant secret key
wpp.maid.secretkey=a8c3fce6-8df7-4fd6-a1fd-62fa229c5e55
```
## Build
``mvn clean install``
## Run
Using the Maven Plugin
``mvn spring-boot:run`` and then open your favorite browser and visit **http://localhost:{server.port}**
## Payment
Use test card number **4200000000000018** (CVV **018** , expiration date **01/19**) for the payment
## Authors
Wirecard - Corvus Team
