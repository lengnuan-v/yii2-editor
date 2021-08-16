yii2-editor
===========
yii2 editor froala

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
composer require --prefer-dist lengnuan-v/yii2-editor "*"
```

or add

```
"lengnuan-v/yii2-editor": "*"
```

to the require section of your `composer.json` file.


Usage
-----

Once the extension is installed, simply use it in your code by  :

```php
    <?= lengnuan\editor\EditorWidget::widget([
    'name' => 'content',
    'options' => [
        // html attributes
        'id'=>'content'
    ],
    'clientOptions' => [
        'toolbarInline'=> false,
        'theme' =>'royal', //optional: dark, red, gray, royal
        'language'=>'en_gb' // optional: ar, bs, cs, da, de, en_ca, en_gb, en_us ...
    ]
]); ?>
```

or use with a model:

```php
    <?= lengnuan\editor\EditorWidget::widget([
    'model' => $model,
    'attribute' => 'content',
    'options' => [
        // html attributes
        'id'=>'content'
    ],
    'clientOptions' => [
        'toolbarInline' => false,
        'theme' => 'royal', //optional: dark, red, gray, royal
        'language' => 'en_gb' // optional: ar, bs, cs, da, de, en_ca, en_gb, en_us ...
    ]
]); ?>
```