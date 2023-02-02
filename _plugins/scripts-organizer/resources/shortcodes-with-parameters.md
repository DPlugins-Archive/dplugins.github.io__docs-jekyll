---
Title: Shortcodes with Parameters
---

# PHP Code
```php

<?php

function dplugins_shortcode_func( $atts ){

$attributes = shortcode_atts( array(

'id' => '',

), $atts );

ob_start();

$post_id = $attributes['id'];

echo get_the_content($post_id);

return ob_get_clean();

}

add_shortcode( 'dplugins_shortcode', 'dplugins_shortcode_func' );

?>


```


# Usage

```
[shortcode id="YOUR-PARAMETER"]
```

# HTML Output

```html


```


