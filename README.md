# YAIE.js
Yet another image encrypter implemented in JavaScript

## Warning
YAIE.js performs simple and **weak** encryption! **DO NOT USE FOR SERIOUS PURPOSE!**

To secure images for serious purpose, maybe AES/RSA/ECC is what demanded.

## Specification
YAIEv1.js simply divides image into parts and rotate every part upside down which would likely make the image hard to recognize. Therefore, YAIE does better with images that are big and complex and may be less effective when dealing with small or simple images.

YAIEv2.js uses random number generated by LCG(aka Linear Congruential Generator) to mask the origin pixel, making the result much more difficult to be recognized. A "passphrase" is required to encrypt and/or decrypt.

YAIE.js only runs on your device, locally and offline, always.