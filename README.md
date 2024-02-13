# Plymouth Theme

Archlinux Plymouth theme using the ACPI BGRT graphics as background

## Installing

You'll need the following dependencies:
* plymouth
* plymouth-theme-spinner

Copy the theme into plymouth themes.

```bash
\# cp -r pop-basic/* /usr/share/plymouth/themes/arch-basic/
```

then set the theme as default and build a new initramfs to apply the changes.

```bash
\# plymouth-set-default-theme -R arch-basic
```

If you want to test this is theme in your running X11 session, you'll need the following dependencies:
* plymouth-x11

### Modes

#### Boot up
```bash
\# plymouth change-mode --boot-up
```
#### Shutdown
```bash
\# plymouth change-mode --shutdown
```
#### Reboot
```bash
\# plymouth change-mode --reboot
```
#### Updates
```bash
\# plymouth change-mode --updates
```
#### Firmware upgrade
```bash
\# plymouth change-mode --firmware-upgrade
```
#### System upgrade
```bash
\# plymouth change-mode --system-upgrade
```
### User interaction

#### Message
```bash
\# plymouth message --text="The quick brown fox jumps over the lazy dog"
```
#### Password prompt
```bash
\# plymouth --ask-for-password
```