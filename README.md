# caesium

caesium is a Clojure binding for libsodium.

It builds on top of [kalium][kalium], the Java binding to
[libsodium][libsodium], which in turn is a more convenient fork of
the original [NaCl][nacl] library by [djb][djb].

[kalium]: https://github.com/abstractj/kalium
[nacl]: http://nacl.cr.yp.to/.
[djb]: http://cr.yp.to/djb.html
[libsodium]: https://github.com/jedisct1/libsodium

"Real" development should most likely happen in the parent library, so
that this one can stay a simple bunch of wrappers.

One difference between kalium and caesium is that kalium follows the
structure of libsodium. For example, in libsodium, BLAKE2b lives in
`crypto_generichash`. In kalium, it lives in `crypto.Hash`. In
caesium, it lives in the `crypto_generichash` namespace.

## License

Copyright © 2014 the caesium authors (see AUTHORS)

Distributed under the Eclipse Public License either version 1.0 or (at
your option) any later version.
