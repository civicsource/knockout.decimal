#Knockout Decimal Extender

> A simple knockout extender for decimals that wraps [accounting.js](http://josscrowcroft.github.io/accounting.js/).


## Installation

```
npm install knockout.decimal
```

## Usage

```js
var dec = ko.observable().extend({ decimal: true });
dec("17000");

console.log(dec()); //17000
console.log(dec.formatted()); //17,000.00
```

You can also use it to set formatted decimal as a value. This is useful for binding user-editable text boxes to the `formatted` computed.

```js
dec.formatted("17,000.56");
console.log(dec()); //17000.56
```
