#Knockout Decimal Extender

> A simple knockout extender for decimals that wraps [accounting.js](http://josscrowcroft.github.io/accounting.js/).


##Install with [Bower](http://bower.io/)

```
bower install knockout-decimal
```

Then add `knockout.decimal.js` to your project.

##How to Use

Include the script on your page (either via a normal script tag or via an AMD loader). Then use it like so:

```js
var dec = ko.observable().extend({ decimal: true });
dec("17000");

console.log(dec()); //17000
console.log(dec.formatted()); //17,000.00
```

You can also use it to set formatted decimal as a value. This is useful for binding user-editable text boxes to the `formatted` computed.

```js
dec.formatted("17,000.56");
console.log(dec()); //17,000.56
```
```