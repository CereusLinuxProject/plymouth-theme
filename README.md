# Plymouth theme
A simple plymouth theme for Cereus Linux

<a href="https://codeberg.org/cereus-linux/plymouth-theme">
    <img alt="Get it on Codeberg" src="https://get-it-on.codeberg.org/get-it-on-white-on-black.png" height="60">
</a>

The source code is mainly hosted on [Codeberg](https://codeberg.org/cereus-linux/plymouth-theme) with a mirror available on [GitHub](https://github.com/CereusLinuxProject/plymouth-theme). **Issues and pull requests should be made in Codeberg**.

# INSTALLATION:
This theme is packaged under [cereus-core](https://sourceforge.net/projects/cereus-linux/files/repos/cereus-core/) repository as `cereus-plymouth-theme` and is included on all desktop editions (except Base, of course). 

To apply it, run:

    # plymouth-set-default-theme cereus_simply
    # xbps-reconfigure -f linux<version>

Where `<version>` is your current kernel version (like 6.6). You can check this by running `uname -r`.

Make sure your boot kernel parameters include `splash` and optionally, `quiet` for a silent boot. If you're using GRUB, add them at `/etc/default/grub`:

	GRUB_CMDLINE_LINUX_DEFAULT="... quiet splash"

And then run `update-grub` as root.
 
# License
This theme is licensed under GPLv3, for more details check LICENSE.
