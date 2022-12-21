Google Chart
============
Render Google chart as image

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require jambtc/yii2-gchart-as-image "dev-master"
```

or add

```
"jambtc/yii2-gchart-as-image": "dev-master"
```

to the require section of your `composer.json` file.


Usage
-----

Once the extension is installed, simply use it in your code by.
Thanks.


You also can refer to https://developers.google.com/chart/interactive/docs/quick_start

```php

    <div class="col-sm-5">
            <?php
            use jambtc\googlechart\GoogleChart;
    
            echo GoogleChart::widget(['visualization' => 'PieChart',
                'asImage' => true, // render as Image
                'data' => [
                    ['Task', 'Hours per Day'],
                    ['Work', 11],
                    ['Eat', 2],
                    ['Commute', 2],
                    ['Watch TV', 2],
                    ['Sleep', 7]
                ],
                'options' => ['title' => 'My Daily Activity']
            ]);
            
            ?>
        </div>
```
