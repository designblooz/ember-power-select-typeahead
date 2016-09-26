# Ember-power-select-typeahead

Naive implementation of a typeahead component on top of ember-power-select.

[Demo](https://ember-power-select-typeahead.pagefrontapp.com/)


## Usage

With simple strings:

```hsb
{{#power-select-typeahead search=(action 'searchAsync') selected=selected onchange=(action (mut selected)) as |number|}}
  {{number}}
{{/power-select-typeahead}}
```

With complex objects:

```hsb
{{#power-select-typeahead search=(action 'searchAsync') selected=selected extra=(hash labelPath="name") onchange=(action (mut selected)) as |user|}}
  {{user.name}}
{{/power-select-typeahead}}
```
