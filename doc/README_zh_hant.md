# B.app PHP SDK 源碼

> `AppKey` 和 `AppSecret`的相關信息，請點擊 [此處](https://mch.b.app/#/mch_info) 獲取。

### 創建訂單

```php

$app = new BappPhpSdk($yourAppKey, $yourAppSecret);
$app->create_order('ThisIsOrderId', 1, 'php-sdk sample', 'https://sdk.b.app/api/test/notify/test', 'https://github.com');
```

### 從B.app服務端獲取訂單詳情

```php
$app = new BappPhpSdk($yourAppKey, $yourAppSecret);
$app->get_order('yourOrderId');
```

### 簽名驗證

```php
$app = new BappPhpSdk($yourAppKey, $yourAppSecret);
$app->is_sign_ok($params);
```
