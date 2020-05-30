<h1>
Robos - robokassa integration module in JavaScript
</h1>

### Features

<img src="https://robokassa.com/img/16548865.svg">
<br/>
- This module will help you use the [ROBOKASSA](https://robokassa.com/ "ROBOKASSA") payment system for JavaScript.
- Independent functionality in the implementation of the class, allows mobile use of this module anywhere in the application.

### Installation
`npm i robos`

<br/>

### Usage

````js
const RobosConnect = require('robos');
const robos = new RobosConnect(robosConfig);

robos.generateUrl(price, invId, desc);
````

### Methods

| Name  |  Description |
| ------------ | ------------ |
| generateUrl  |  creating a link to redirect or go to the payment page (формирование подписи для создания ссылки на оплату). **return: STRING** |
|  generateSignature | signature generation to create a link (создание ссылки для редиректа или перехода на страницу оплаты). **return: STRING**  |
| checkPay | checks for successful payment (проверка на успешную оплату). **return: BOOLEAN** |



