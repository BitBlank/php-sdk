# B.app Resource Storage SDK for PHP

> To visit your AppKey and AppSecret, you can click [here](https://mch.b.app/#/mch_info) and read more.

### Create Order

```php

$app = new BappPhpSdk($yourAppKey, $yourAppSecret);
$app->create_order('ThisIsOrderId', 1, 'php-sdk sample', 'https://sdk.b.app/api/test/notify/test', 'https://github.com');
```

### Get order detail from the B.app server

```php
$app = new BappPhpSdk($yourAppKey, $yourAppSecret);
$app->get_order('yourOrderId');
```

### Check the sign

```php
$app = new BappPhpSdk($yourAppKey, $yourAppSecret);
$app->is_sign_ok($params);
```
