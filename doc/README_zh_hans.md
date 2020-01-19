# B.app PHP SDK 源码

> `AppKey` 和 `AppSecret`的相关信息，请点击 [此处](https://mch.b.app/#/mch_info) 获取。

### 创建订单

```php

$app = new BappPhpSdk($yourAppKey, $yourAppSecret);
$app->create_order('ThisIsOrderId', 1, 'php-sdk sample', 'https://sdk.b.app/api/test/notify/test', 'https://github.com');
```

### 从B.app服务端获取订单详情

```php
$app = new BappPhpSdk($yourAppKey, $yourAppSecret);
$app->get_order('yourOrderId');
```

### 签名验证

```php
$app = new BappPhpSdk($yourAppKey, $yourAppSecret);
$app->is_sign_ok($params);
```
