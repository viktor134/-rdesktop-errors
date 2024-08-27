
## Troubleshooting

If you see the `UI(error): ui_init(), failed to open X11 display` error, it means there is an issue with the X11 display setup. Please ensure the following:

- **X11 Server**: Make sure the X11 server is running on your system.
- **DISPLAY Variable**: Verify that the `DISPLAY` environment variable is set correctly.
- **X11 Authentication**: Check the `.Xauthority` file in your home directory and ensure it has the correct permissions.
- **Remote Connections**: If connecting via SSH, ensure X11 forwarding is enabled.



## Usage

Bourne, Bash or Korn shell:

```
export DISPLAY=localhost:0.0
```

BashDownload  C shell
```
setenv DISPLAY localhost:0.0
```
And again test 
```
rdesktop -f remote-host -u '' -r scard 
```
[What is the DISPLAY environment variable? X11](https://datacadamia.com/ssh/x11/display)
[Rdesktop](https://github.com/rdesktop/rdesktop/releases)




