# yii2-smser

Yii2 SMS extension （短信扩展）

## Installation

The preferred way to install this extension is through [composer](http://getcomposer.org/download/). Check the [composer.json](https://github.com/daixianceng/yii2-smser/blob/master/composer.json) for this extension's requirements and dependencies.

To install, either run

```
$ php composer.phar require lkk/yii2-smser "*"
```

or add

```
"lkk/yii2-smser": "*"
```

to the ```require``` section of your `composer.json` file.

## Usage

```php
return [
    'components' => [
        'smser' => [
            'class' => 'lkk\smser\HuyiSmser',
            'username' => 'username',
            'password' => 'password',
        ]
    ],
];
```

OR

```php
return [
    'components' => [
        'smser' => [
            'class' => 'lkk\smser\HuyiSmser',
            'apikey' => 'wcJRH2mh7BbfIsaWLD4QCbllCaVpZNIp', // 请替换成您的apikey
        ]
    ],
];
```

```php
Yii::$app->smser->send('13000000000', '短信内容');
```

## License

**yii2-smser** is released under the BSD 3-Clause License. See the bundled `LICENSE` for details.
