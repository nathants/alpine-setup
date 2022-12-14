# alpine-setup

## why

bootstrapping a new laptop should be easy.

## how

1. [alpine-iso](./alpine-iso):
   - flash a [standard iso](https://alpinelinux.org/downloads/) to a usb drive from any linux distro.

2. [alpine-install](./alpine-install):
   - boot into the usb drive.
   - login as root with empty password.
   - run `setup-interfaces` to get online.
   - run `rc-service networking restart`.
   - run `setup-apkrepos`.
   - run `vi /etc/apk/repositories`.
   - run [DEVICE=/dev/nvme0n1 KERNEL=lts ./alpine-install](./alpine-install).

3. [alpine-setup](./alpine-setup):
   - reboot into the installed system.
   - login as root with empty password.
   - run [./alpine-setup](./alpine-setup).

4. restore dotfiles and other data from a [backup](https://github.com/nathants/backup).
