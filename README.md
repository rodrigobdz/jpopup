# jPopup #
### Simple lightweight javascript popup modal plugin ###

### Another popop? ###
Yep, I needed simple as possible modal plugin for personal use, so jPopup was born.

### Install ###

With npm:
```sh
npm install jpopup
```

With Bower:
```sh
bower install jpopup
```

### Usage ###

Include required javascript:
```sh
<script src="jPopup.js"></script>
```

Include css:
```sh
<link href='jPopup.css' rel='stylesheet' type='text/css'>
```
Initialize jPopup:
```sh
<script>
    var myPopup = new jPopup({
    	content: '<p>My popup text</p>'
    });
</script>
```

### Demo ###

Demo available [here](http://www.rvdizajn.com/jpopup/).

### Example ###

```sh
<script>
    document.querySelector('.openPopup').addEventListener('click', function() {

        var jPopupDemo = new jPopup({

            content: '<strong>Hurray</strong>\
                    <p>You can put any content you want here.</p>'

        });

    });
</script>
```

### Options ###

jPopup can take an optional parameters - an object of key/value settings:

- **content** String *(required)* - string of content to display
- **hash** Boolean *(default:true)* - should popup append hashtag (`#popup`) in the current url (applied [History API](https://developer.mozilla.org/en-US/docs/Web/API/History_API))

Default css styling are placed in `/sass/library/_setup.scss`:

- **$baseBreakpoint** *(default:680px)* - media query breakpoint value
- **$bgColor** *(default:#fff)* - popup background color
- **$closeBtnColor** *(default:#adadad)* - color of close button


### API ###

`open()` - open popup

`close()` - close popup


### Browser support ###

It works in every modern browser where [Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise) and [classList](https://developer.mozilla.org/en-US/docs/Web/API/Element/classList) are supported.

Consider using polyfills for [Promise](https://github.com/stefanpenner/es6-promise) and [classList](https://github.com/eligrey/classList.js/) features if needed.


### License  ###

jPopup is licensed under the [MIT license](http://opensource.org/licenses/MIT).
