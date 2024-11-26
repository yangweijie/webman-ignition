# webman-ignition

## 安装

- `composer require yangweijie/webman-ignition`

- 将 `config/exception.php`  修改为以下内容

~~~
<?php
use Yangweijie\WebmanIgnition\ExceptionHandle;

return [
    ''=>ExceptionHandle::class
];
~~~

## 配置

~~~
return [
    'enable' => true, // 是否启用
    'show_error_msg'=>true, // 是否显示异常信息，否用原生的异常渲染
    'useDarkMode' => false, // 是否使用深色模式
    'editor'      => 'vscode',  // 打开php文件的编辑器或ide
];
~~~