# pcb-tiny

pcb-tiny 为 pcb 项目封装了 tiny 服务端 API。

## 安装

```shell
composer require "pcb-org/pcb-tiny"
```

## 使用示例

```php
use PcbTiny\Application;

$config = [
    'base_uri' => 'http://127.0.0.1',
    'hmac_key' => 'YOUR_HMAC_KEY',
];

$app = new Application($config);

$app->withContext(['id' => $id, 'name' => $name])->makeUser()->index($params);
```
