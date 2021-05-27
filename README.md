# VPS2SUSE

> Install openSUSE on your VPS, no matter what's the current OS.

## Usage

1. Install curl with your current package manager

2. Run this script

```
$ curl -L https://cdn.jsdelivr.net/gh/U2FsdGVkX1/vps2suse@main/vps2suse | sudo $SHELL -s -- [OPTIONS]
```

3. Sync data and reboot

```
$ sudo $SHELL -c 'sync && reboot -f'
```

4. Change your root password (Default: vps2arch)

```
passwd
```

### Options

```
-h Show help messages.
-c Set architecture type for the container image (Default: auto detect).
-m Set mirror address (Default: https://download.opensuse.org).
```

## Credits

This project is based on [vps2arch](https://github.com/drizzt/vps2arch)

## License

GNU General Public License 3.0
