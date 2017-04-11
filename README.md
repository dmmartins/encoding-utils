# encoding-utils

Encoding/decoding tools I use once in a while (some more than others) when developing/debugging software.

## bin-encode

Encode input in binary format:

    $ echo "Hello world" | bin-encode
    01001000 01100101 01101100 01101100 01101111 00100000 01110111 01101111 01110010 01101100 01100100

## bin-decode

Decode binary input to ascii:

    $ echo "01001000 01100101 01101100 01101100 01101111 00100000 01110111 01101111 01110010 01101100 01100100" | bin-decode
    Hello world

## encode64

Encode input in base64:

    $ echo "Hello world" | encode64
    SGVsbG8gd29ybGQ=

## decode64

Decode base64 input to ascii:

    $ echo "SGVsbG8gd29ybGQ=" | decode64
    Hello world

## hex-encode

Encode input to hex format:

    $ echo "Hello World" | hex-encode
    48 65 6C 6C 6F 20 57 6F 72 6C 64

## hex-decode

Decode hex input to ascii:

    $ echo "48 65 6C 6C 6F 20 57 6F 72 6C 64" | hex-decode
    Hello World

## urlencode

Encode input to as URI component:

    $ echo "hello@world" | urlencode
    hello%40world

## urldecode

Decode URI component input to ascii:

    $ echo "hello%40world" | urldecode
    hello@world

