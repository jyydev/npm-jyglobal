# jyglobal

jyglobal is a personal npm module for speeding up development, testing and debugging stages.

## Installation

In terminal (navigate to your project folder first):

```
npm i jyglobal
```

then in your .js file, include this code to start using:

```
require('jyglobal');

log('hello, shorthand for console.log')
cc('hi, shorthand for console.log')
```

### Functions (global scope)

- `log(message)`
  - about: shorthand for `console.log(message)`, acts exactly like `console.log(message)`
  - params:
    - `message` [optional]
      - `message`: can be integer, variable, array, object.
      - `log()`: if `message` is ommited, a blank line will be returned.
  - advanced: supports multiple params: `log(msg1, msg2, ...)` = `console.log(msg1, msg2, ...)`
- `cc(message)`
  - about:
    - light weight, shorter version of `console.log(message)`.
    - stands for **c**losed **c**aptioning in subtitle (act like subtitle on movie 😊).
    - `cc('example)` is the same as `console.log(example)`.
  - param:
    - `message` [optional]
      - `cc()`: function as a separator
      - if `message` is empty -> console.log(`----------`) in terminal
  - extra: only accept 1 param, use `log(message)` for multiple params.

### Notes

More globals will be added in the future for easier testing and debugging.
