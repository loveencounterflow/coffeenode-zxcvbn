# CoffeeNode ZXCVBN


Derived from [node-zxcvbn](https://github.com/mintplant/node-zxcvbn), which itself is [zxcvbn](https://github.com/lowe/zxcvbn),
a password strength calculator, packahed as a node.js module; authored by Dan Wheeler at Dropbox; published
to npm by Michael Smith.

See [the original](https://github.com/lowe/zxcvbn) for more details.

This module has the distinction to include all files resulting from various build steps that are not terribly
obvious even from the original README. The JS code that you get with `require( 'coffeenode-zxcvbn' )` is
optimized using the ClosureJS compiler, resulting in a filesize of roughly 700MB.

# How to use

In CoffeeScript:

```coffeescript
zxcvbn = require 'coffeenode-zxcvbn'
report = zxcvbn password
``

`report` is a Plain Old Dictionary; the interesting attributes are `report[ 'crack_time_display' ]`,
`report[ 'crack_time' ]`, `report[ 'score' ]`, and `report[ 'entropy' ]`; please refer to the original documentation
linked above.



