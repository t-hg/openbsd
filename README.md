# OpenBSD

## GVFS / SMB

```
doas pkg_add gvfs gvfs-smb dbus avahi
doas rcctl enable multicast messagebus avahi_daemon
```

``$HOME/.xsession``:

```
[...]
exec dbus-launch --exit-with-session --sh-syntax i3
# For XFCE dbus-launch should be not necessary, you can just use:
# exec startxfce4
```
