# `<when-do>` Web Component

_Note: this is an initial, incomplete, README and needs more documentation._

## Description

A non visual web component that wraps you content (or can be inserted as an empty tag) that has an effect when a specific datetime has passed.

## Usage and API

```html
<script src="when-do.mjs" type="module"></script>

<when-do datetime="2023-12-12T12:10" do="show">
  <p>I shall appear after 12th November 2023 at 12:10pm</p>
</when-do>
```

The `when-do` element supports the following attributes:

- `do="show|hide|scroll"` required action to do
- `datetime="isodate"` required, in the format of `2023-12-12T12:00:00`
- `apply` optional className to apply to the web component when the `do` is triggered

## TODO

- Support relative times, such as `datetime="2023-12-12T12:10 1d"`
- Fix so that the most recently passed event fires, rather than the last found web component
- Optimise code (i.e. only run code on state change)
- Add examples
- Probably more here

## License

- [MIT](https://rem.mit-license.org/)
