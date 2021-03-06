# Get started


Welcome! These pages aim to provide all the information you need to master Ractive.

If you see something wrong, out of date, or missing from this documentation, please check out our [known issues and FAQs](Known issues, FAQs, and Tips.md), [raise an issue on GitHub](https://github.com/ractivejs/docs.ractivejs.org/issues) or - even better - submit a pull request. Your fellow Ractive users will thank you!

## Where to get Ractive

Ractive is published regularly to npm as both regular and dev builds. Since [unpkg](https://unpkg.com) mirrors the npm registry in link-friendly way, you can download or link to any Ractive version from there:

| Version | URL |
| ------- | --- |
| latest  | https://unpkg.com/ractive |
| edge | https://unpkg.com/ractive@edge |
| 0.8 unreleased stable | https://unpkg.com/ractive@v0.8-dev |
| 0.7.3 | https://unpkg.com/ractive@0.7.3 |

## 15 second overview

Using Ractive is very simple. An instance is created using `new Ractive({...})`
with the desired options:

```js
var ractive = new Ractive({
  target: 'container',
  template: '<p>{{greeting}}, {{recipient}}!</p>',
  data: { greeting: 'Hello', recipient: 'world' }
});
```

While there are no _required_ options, the three shown above - __target__, __template__ and __data__ - are the most common. They specify __what data__ to bind to __what template__ and __where__ it should be placed in the __html document__.

A good way to get up and running is with the [60 second setup](http://ractivejs.org/60-second-setup). After that, working your way through the [interactive tutorials](http://learn.ractivejs.org) will familiarise you with the various ways you can use Ractive.

Checkout the [Configuration Options](Options.md) to learn more about
all the available options.

If you get stuck at any point, visit the [Get support](Get support.md) page to find help.

## Documentation for other versions

*Documentation for previous versions: [0.3.9](../0.3.9), [0.4.0](../0.4.0), [0.5.x](../0.5), [0.6.x](../0.6), [0.7.x](../0.7), [0.8.x](../0.8)*

*Documentation for latest version: [latest](../latest)*

*Documentation for edge version: [edge](../edge)*
