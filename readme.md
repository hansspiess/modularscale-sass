# Modular Scale !important

An opinionated fork of the great [modularscale](https://github.com/modularscale/modularscale-sass) with the addition of being able to call ms-respond() with a fourth parameter rendering declarations with `! important`.

The necessity of this feature arised when using [inuitcss](https://github.com/inuitcss/inuitcss) utility classes (eg. `.u-h1`) for custom heading formats with headings element styling via `ms-respond()`.

## Usage

Just call `ms-respond()` with four parameters (omitting `$modularscale` is not possible with four params):

```Scss
.u-h4 {
  @include ms-respond(font-size, 1, $modularscale, true);
}
```
