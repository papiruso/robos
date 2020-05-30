<h1>
Robos - robokassa integration module in JavaScript
</h1>

### Features

<img src="https://robokassa.com/img/16548865.svg">
<br/>
- This module will help you use the [ROBOKASSA](https://robokassa.com/ "ROBOKASSA") payment system for JavaScript.
- Independent functionality in the implementation of the class, allows mobile use of this module anywhere in the application.

### Installation
```shell
$ npm i robos
```

<br/>

### Usage

````js
const RobosConnect = require('robos');

const robosConfig = {
	mrhLogin: 'shoplogin',
	mrhPass1: 'securepass1',
	mrhPass2: 'securepass2',
};

const robos = new RobosConnect(robosConfig);

robos.generateUrl(price, invId, desc);
````

### Methods

| Name  |  Description |
| ------------ | ------------ |
| generateUrl  |  creating a link to redirect or go to the payment page (формирование подписи для создания ссылки на оплату). **return: STRING** |
|  generateSignature | signature generation to create a link (создание ссылки для редиректа или перехода на страницу оплаты). **return: STRING**  |
| checkPay | checks for successful payment (проверка на успешную оплату). **return: BOOLEAN** |

### Configs
|  Name  |  Description  |
| ------------ | ------------ |
| mrhLogin  | Store identifier specified in the “Technical settings”section of your store (Идентификатор магазина, прописанный в разделе «Технические настройки» Вашего магазина)   |
|  mrhPass1  |  merchant pass1 here |
|  mrhPass2  |  merchant pass2 here |
|  outSumCurrency  |  currency selection: USD, EUR and KZT. Default - ruble |



