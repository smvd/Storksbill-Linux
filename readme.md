# Storksbill linux

**Storksbill linux** is a fork of **Alpine linux** a distro mostly used for containerisation. Its designed to be *small*, *simple* and *secure*. **Storksbill** is designed to be a desktop distro focussed on development, but without changing these core principles.

### Installation.

**Storksbill linux** is currently a install script that runs in a fresh **alpine linux** ISO. But to get access to this install script you must first get networking functioning. 

After booting your live USB and logging in with the root account (no password) and connecting an ethernet cable. You must run the following commands:

```shell
setup-interfaces
ip link set <interface> up # the setup command show the interface
udhcpc
```

After that you should be ready to run the installer.

```shell
wget rebrand.ly/storksbill
chmod +x storksbill
./storksbill
```
