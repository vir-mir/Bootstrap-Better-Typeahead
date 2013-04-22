# Bootstrap Better Typeahead Extension

This **Bootstrap Better Typeahead** extends the Bootstrap Typeahead plugin and adds support for a ```minLength``` option set to zero.

Setting ```minLength``` to zero now correctly opens the full list of available options on element focus and on empty queries.

#### Adding the extension to your Bootstrap application

Adding the plugin is unobtrusively - ie. you extend the bootstrap plugin by adding the following file after you included the original bootstrap plugin.

#### Example

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Bootstrap Better Typeahead Example</title>

        <!-- optional -->
        <link rel="stylesheet" href="/css/bootstrap-better-typeahead.css">
    </head>
    <body>
        <input type="text" id="selector">

        <script type="text/javascript" src="//ajax.googleapis.com/ajax/libs/jquery/2.0.0/jquery.min.js">
        <script type="text/javascript" src="//raw.github.com/twitter/bootstrap/master/js/bootstrap-typeahead.js">

        <script type="text/javascript" src="/js/bootstrap-better-typeahead.js">
        
        <script type="text/javascript">
            $(function() {
                $("#selector").typeahead({
                    minLength: 0,
                    source: ["Neque", "porro", "quisquam", "est", "qui", "dolorem", "ipsum", "quia", "dolor", "sit", "amet", "consectetur"]
                });
            });
        </script>
    </body>
</html>
```

