LBUM #

This code lets you embed an Eversnap album directly on your website.

## Installation

Include this code right before the closing body tag (</body>):

``` js
<script type="text/javascript">
!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0];if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src="https://s3.amazonaws.com/media.weddingsnap.com/platform/widget.min.js";fjs.parentNode.insertBefore(js,fjs);}}(document,"script","eversnap-wjs");
</script>
```

Include this code where you want the album to appear:
``` html
<a class="eversnap-album" height="300" width="300" href="https://www.eversnappro.com/album/<id>"></a>
```

where **<id>** is the id of the album you want to display.

Pretty easy, right?!

## Customization
We provide a basic API to customize the widget appearance, accessible through the HTML tag attributes.

- **WIDTH**: widget width
- **HEIGHT**: widget height
- **DATA-CUSTOM-STYLE**: a JSON String specifying one or more of the following keys:
    - **h_color**: header text color
    - **h_bg**: header background color
    - **btn_color**: join button text color
    - **btn_bg**: join button background color

This is an example of a well-formatted data-custom-style attribute value:
`'{"h_bg":"rgb(0,255,255)","h_color":"black","btn_bg":"black","btn_color":"white"}'`

As you can see you can specify colors in the way you prefer, all [CSS's specifications](https://developer.mozilla.org/en-US/docs/Web/CSS/color) are supported.

**NOTE**: If the format isn't correct the widget will throw a console error and use the default Eversnap colors.
