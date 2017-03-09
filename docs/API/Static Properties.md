# Static Properties

## Ractive.adaptors

`(Object<string, Object>)`

A map of globally available [adaptors](../Extend/Adaptors.md), where the key is the adaptor name and the value is an adaptor definition.

---

## Ractive.components

`(Object<string, Function>)`

A map of globally available [components](../Extend/Components.md), where the key is the component name and the value is a component definition.

---

## Ractive.DEBUG

`(boolean)`

Whether or not Ractive is in debug mode. Defaults to `true`.

When set to `true`, warnings to non-fatal errors are logged. When set to `false`, warnings to non-fatal errors are suppressed.

---

## Ractive.DEBUG_PROMISES

`(boolean)`

Whether or not Ractive logs errors thrown inside promises. Defaults to `true`.

When set to `true`, errors thrown in promises are logged. When set to `false`, errors inside promises are suppressed.

---

## Ractive.decorators

`(Object<string, Function>)`

A map of globally available [decorators](../Extend/Decorators.md).

---

## Ractive.defaults

`(Object<string, any>)`

The defaults for [initialisation options](../API/Initialization Options.md) with the exception of [plugin registries](../Integrations/Plugins.md).

```js
// Change the default mustache delimiters to [[ ]] globally
Ractive.defaults.delimiters = [ '[[', ']]' ];

// Future instances now use [[ ]]
ractive1 = new Ractive({
  template: 'hello [[world]]'
});
```

Configurations set on lower initializations will override the ones set higher.

```js
// Override delimiters globally
Ractive.defaults.delimiters = [ '(%', '%)' ];

new Ractive({
  template: 'hello (% world %)'
});

// Override delimiters for instances of this component
const Component = Ractive.extend({
  delimiters: [ '{%', '%}' ],
  template: 'hello {% world %}'
});

new Component({ ... });

// Override delimiters for this specific instance
new Ractive({
  delimiters: [ '[%', '%]' ]
  template: 'hello [% world %]',
});
```

---

## Ractive.easing

`(Object<string, Function>)`

A map of globally available [easing functions](../Extend/Easings.md).

Four are included by default: `linear`, `easeIn`, `easeOut` and `easeInOut`.

---

## Ractive.events

`(Object<string, Function>)`

A map of globally available [events](../Extend/Events.md).

---

## Ractive.interpolators

`(Object<string, Function>)`

A map of globally available [interpolators](../Extend/Interpolators.md).

---

## Ractive.length

Since `Ractive` is a function, and functions have a `length` equal to their number of declared arguments, `Ractive` has a `length` of `1`.

---

## Ractive.name

Like `length`, functions also have a `name`, and `Ractive`'s happens to be `"Ractive"`.

---

## Ractive.partials

`(Object<string, string|Object|Function>)`

A map of globally available [partial templates](../Extend/Partials.md).

Like [templates](../Concepts/Templates/Overview.md), partials are [parsed](../Concepts/Templates/Parsing.md) at the point of use. The parsed output is cached and utilized for future use.

---

## Ractive.svg

`(boolean)`

Whether or not the browser supports SVG.

---

## Ractive.transitions

`(Object<string, Function>)`

A map of globally available [transitions](../Extend/Transitions.md).

---

## Ractive.VERSION

The version of the currently loaded Ractive.
