# react-touched

Create inputs with pre-computed values, until touched.

## Use case

`react-touched` can be used when there is a value derived from the other field, but you'd like to allow user to enter its own value if needed. In the particular author's use case it was a SEO text field, by default computed using title in date. But user can just enter own SEO text if needed.

## Usage

`ReactTouched` comes as a single `TouchableInput` component you can use. All properties passed (except listed below) will be passed to the input component passed as `inputType` property.

## Examples

## Properties

* `untouchedValueFn` - ...
* `untouchedValueArgs` - ...
* `emitsUpdatesIfUnchanged` - ...
* `onChange` - ...

## API

`TouchableInput` can be referenced by the top-level component using [`ref` mechanism](https://facebook.github.io/react/docs/more-about-refs.html). It exposes following methods:

* `touch()` [returns nothing]  - artificially set the input to 'touched' state.
* `untouch()` [returns nothing] - artificially set the input back to 'untouched' state.
* `touched()` [returns bool] - check state in which input is currently.
* `value()` [returns mixed] - return the value of the input. Unlike checking `value`, it takes into account whether it's in touched/untouched state.

## License

ISC.



