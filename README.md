jquery.inlineLabel
==================

Converts existing `<label>` to inline labels, kind of like the 
[`placeholder`](http://www.w3schools.com/html5/tryit.asp?filename=tryhtml5_input_placeholder) HTML5 attribute.

[Try the demo!](http://jsfiddle.net/Znarkus/x2NFe/)

    $('label').inlineLabel();

This will position the label elements on top of the inputs, and copy their style.

    .inlineLabel([options])

### Optional options

- `css` - Object with CSS properties/values
- `activeOpacity` - Label CSS opacity when a label is inline
- `focusOpacity` - Label CSS opacity when form field is active
- `duration` - Animation speed for changing opacity


### Example

    <form>
        <label for="name">Enter your name</label>
        <input type="text" name="name" id="name" />
    </form>

    $('label').inlineLabel({
        activeOpacity: 0.8,
        focusOpacity: 0.5,
        duration: 300,
        override_focus: true,
        css: {
            color:'red'
        }
    });

### Known issues

- You can't have an inline label within a hidden (on page load) container


## License

Copyright 2012, [Markus Hedlund](http://markushedlund.com), [Snowfire](http://snowfireit.com).  
Licensed under the MIT License.  
Redistributions of files must retain the above copyright notice.