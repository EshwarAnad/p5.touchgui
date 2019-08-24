[Home](../README.md) | [Reference](REFERENCE.md)

# GuiCrossfader / GuiCrossfaderV
## Description
Crossfader class. 

*Note: vertical crossfader class is virtually the same, just with a different orientation.*

-----

## Variables

-----

### val
[[Back to top]](#description)

##### Example
```javascript
crossfader.val = 0.5;
```
```javascript
if (crossfader.isChanged) {
    print(crossfader.val);
}
```

##### Description
Value of the `GuiCrossfader`.

-----

### min
[[Back to top]](#description)

##### Example
```javascript
crossfader.min = -100;
```

##### Description
Lower bound of the `GuiCrossfader` range.

-----

### max
[[Back to top]](#description)

##### Example
```javascript
crossfader.max = 100;
```

##### Description
Upper bound of the `GuiCrossfader` range.

-----

### isInteger
[[Back to top]](#description)

##### Example
```javascript
crossfader.isInteger = True;
```

##### Description
Sets the mode of the `GuiCrossfader` so that all values are integers.

-----

## Functions

-----

### [setStyle()]()
[[Back to top]](#description)

##### Example
```javascript
crossfader.setStyle("fillBg", color(255, 0, 0));
```
```javascript
crossfader.setStyle({
    fillBg: color("#FF0000"),
    rounding: 10,
    trackWidth: 0.1
});
```

##### Description
Individual `GuiCrossfader` objects can be styled using this method. There are two types of input it takes. Use an input string and value to set an individual property, and use an `Object` with key/value notation to set multiple properties at once.

##### Syntax
```javascript
setStyle(property, value)
setStyle(Object)
```

##### Parameters
`property` String: name of property to be set
`value` Number|String|Object: value of property to be set
`Object` Object: multiple propertys and values to be set

##### Returns
`None`

-----

## Style
[[Back to top]](#description)

The `GuiCrossfader` style properties are:
* `strokeWeight` Number: the weight (in pixels) of the stroke
* `rounding` Number: radius of corners
* `trackWidth` Number: width of all crossfader tracks between 0 (line) and 1 (full)
* `fillBg` p5.Color: default background fill color
* `fillBgHover` p5.Color: hover background fill color
* `fillBgActive` p5.Color: active background fill color
* `fillTrack` p5.Color: default track fill color
* `fillTrackHover` p5.Color: hover track fill color
* `fillTrackActive` p5.Color: active track fill color
* `fillHandle` p5.Color: default handle fill color
* `fillHandleHover` p5.Color: hover handle fill color
* `fillHandleActive` p5.Color: active handle fill color
* `strokeBg` p5.Color: default background stroke color
* `strokeBgHover` p5.Color: hover background stroke color
* `strokeBgActive` p5.Color: active background stroke color
* `strokeTrack` p5.Color: default track stroke color
* `strokeTrackHover` p5.Color: hover track stroke color
* `strokeTrackActive` p5.Color: active track stroke color
* `strokeHandle` p5.Color: default handle stroke color
* `strokeHandleHover` p5.Color: hover handle stroke color
* `strokeHandleActive` p5.Color: active handle stroke color
* `strokeCenter` p5.Color: default center line stroke color
* `strokeCenterHover` p5.Color: hover center line stroke color
* `strokeCenterActive` p5.Color: active center line stroke color