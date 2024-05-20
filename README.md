# OpenBSD

## GVFS / SMB

```
doas pkg_add gvfs gvfs-smb dbus avahi
doas rcctl enable multicast messagebus avahi_daemon
```

``$HOME/.xession``:

```
[...]
exec dbus-launch --exit-with-session --sh-syntax i3
```
