# alpine-setup

## why

bootstrapping a new laptop should be easy.

## how

- [alpine-iso](./alpine-iso) flash a [standard iso](https://alpinelinux.org/downloads/) to a usb drive from any linux distro.

- [alpine-install](./alpine-install) boot into the usb drive, login as root with empty password, and run [alpine-install](./alpine-install)`.

- [alpine-setup](./alpine-setup) reboot into the installed system, and run [alpine-setup](./alpine-setup).

- restore dotfiles and other data from a [backup](https://github.com/nathants/backup).
