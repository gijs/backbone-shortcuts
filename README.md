# Backbone.Shortcuts

*Backbone.js + Keymaster.js = Backbone.Shortcuts.*

## Downloads

  * [Development Version](https://raw.github.com/bry4n/backbone-shortcuts/master/backbone.shortcuts.js) 1.031 kb, full source code
  * [Production Version](https://raw.github.com/bry4n/backbone-shortcuts/master/backbone.shortcuts.min.js) 0.577 kb, packed and gzipped

## Dependencies

* [Underscore.js ~> 1.3.1](http://underscorejs.org/)
* [Backbone.js ~> 0.9.1](http://backbonejs.org/)
* [Keymaster.js ~> 1.0.2](https://github.com/madrobby/keymaster/)

## Usage

**HTML**

```html
<script src="underscore.min.js"></script>
<script src="backbone.min.js"></script>
<script src="keymaster.min.js"></script>
<script src="backbone.shortcuts.min.js"></script>
```

**JavaScript**

```javascript
var ShortcutKeys = Backbone.Shortcuts.extend({
  shortcuts: {
    "ctrl+r" : "reloadPage"
  },
  reloadPage: function() {
    alert("Reloaded!!");
  }
});

var shortcuts = new ShortcutKeys;
```

**CoffeeScript**

```coffeescript
class ShortcutKeys extends Backbone.Shortcuts
  shortcuts:
    "ctrl+r" : "reloadPage"
  reloadPage: -> alert "Reload!!!"

shortcuts = new ShortcutKeys
```

Read [example.html](https://github.com/bry4n/backbone-shortcuts/blob/master/example.html)

## Author
Bryan Goines, [@bryangoines](http://twitter.com/bryangoines)
