# VPS2SUSE

> Install openSUSE on your VPS, no matter what the current OS is.

## Usage

1. Install curl with your current package manager

2. Run this script

```
$ curl -OL https://raw.githubusercontent.com/U2FsdGVkX1/vps2suse/main/vps2suse # or use https://cdn.jsdelivr.net/gh/U2FsdGVkX1/vps2suse@main/vps2suse
$ chmod +x vps2suse
$ sudo ./vps2suse #[OPTIONS]
```

3. Sync data and reboot

```
$ sudo $SHELL -c 'sync && reboot -f'
```

4. Connect to server after about 3 minutes.

```
# the root password from the original system (or by using vps2suse as password if no root password was set).
$ ssh root@your-server-ip
```

5. Change your root password

```
passwd
```

### Options

```
-h Show help messages.
-s Set OS version, For example "-s Leap-15.3" (Default: Tumbleweed).
-c Set architecture type for the container image (Default: auto detect).
-m Set mirror address (Default: https://download.opensuse.org).
```

## Credits

This project is based on [vps2arch](https://github.com/drizzt/vps2arch)

## License

GNU General Public License 3.0
