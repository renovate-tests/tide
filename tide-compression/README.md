# tide-compression

This crate provides compression-related middleware for Tide.

## Examples

Examples are in the `/examples` folder of this crate.

__Simple Example__

You can test the simple example by running `cargo run --example simple` while in this crate's directory, and then running either of the following commands:

```console
$ curl http://127.0.0.1:8000/ -v
$ echo 'why hello there' | gzip | curl -v --compressed -H 'Content-Encoding: gzip' 'http://127.0.0.1:8000/echo' --data-binary @-
```
