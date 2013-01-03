PTags
=====
I just quickly wrote a widget for the JQuery plugin [Pines Tags](http://pinesframework.org/ptags/#demos). Pines Tags is a beautiful and easy to use plugin. Even so, this widget is very easy to use.

The Pines Tags plugin is untouched.

Have a look at the [Github Repo](https://github.com/Dadeniss/PTags).

##Requirements

Yii 1.1 or above.

##Usage
Just extract in your extensions directory and use it like every other widget:

~~~php
$this->widget('application.extensions.PTags.PTags',array(
    'id'=>'die_hard',
    'value'=>'action,bruce fucking willis,awesome,explosions,dead terrorists',
    'options'=>array(
        'editable'=>false,
        'remover'=>false
    )
));
~~~
**value** are the tags seperated by **delimiter**(standard: ",") "hardcoded" into the value of the input tag. You can leave it empty and use the **tags** option if you want to submit an array.

Options are the same as pines tags offers, but without the _ptags__-prefix:

~~~php
$options=array(
  	'tags' => array(),
		'current_text' => true,
		'delimiter' => ",",
		'trim_tags' => true,
		'show_box' => false,
		'input_box' => true,
		'remover' => true,
		'editable' => true,
		'sortable' => false,
		); 
~~~

##Resources
 * [Github Repo](https://github.com/Dadeniss/PTags)
 * [Pines tags](http://pinesframework.org/ptags/)
 * [Try out a demo](http://pinesframework.org/ptags/#demos)
 * [Yii extension: fancybox](http://www.yiiframework.com/extension/fancybox) (I have stolen the widget skeleton code :D )
