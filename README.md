# MJML 4 - fork


This is a fork from [mjml].

We added the following changes:

## mj-button custom-link-attrs

The `mj-button` now also accepts the `custom-link-attrs` attribute.
Whatever value you indicate there is added inside the opening link tag `<a HERE >`.

Note: for now the value doesn't seem to support quotes,
so we would need to fix it to allow attributes with values,
like `my-attr="something"`.

Example:
```html
<mj-button custom-link-attrs="mc:disable-tracking" href="#">Click me</mj-button>
```

Will generate a button layout including this link:
```html
<a mc:disable-tracking href="#">Click me</a>
```

[mjml]: https://github.com/mjmlio/mjml
