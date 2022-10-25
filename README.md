# Feather Flatpak

This is the flatpak manifest for packaging [Feather](https://featherwallet.org/),
a free Monero desktop wallet.

## Notes about building

It requires a decent amount of RAM. Due to having 16 cores, `flatpak-builder`
scheduled 16 paralell jobs which were too much for my 8G RAM + 10G swap.
Specifying `--jobs=8` worked well for me.

## State

All optional features are turned off, most notably, this includes the embedded
TOR proxy. It's planned to package it all when the basics are working smoothly.

## Author's blessing

... is still in progress. See [this issue](https://github.com/feather-wallet/feather/issues/47)
