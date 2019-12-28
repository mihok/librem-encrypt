# Librem Key hook for Arch Linux initcpio

This mkinitcpio hook allows you to use a PGP-compatible smart card during early
boot to decrypt your full disk encrypted system. The scripts are slight
modifications of the `encrypt` hook that already comes installed.

More information on why this was created and how you can set up something
similar can be found in the blog post [here][1].

# Installation

For more information on `mkinitcpio` and custom hooks please read up on the
Arch Linux wiki page [here][2] and see [mkinitcpio(8)][3] for details.

Custom hooks come in two parts, an install hook and the script that actually
runs when the device is booted. The install hook can be put into
`/etc/initcpio/install/` and the run hook can be placed in `/etc/initcpio/hooks/`.


[1]: https://mihok.today/
[2]: https://wiki.archlinux.org/index.php/Mkinitcpio
[3]: https://jlk.fjfi.cvut.cz/arch/manpages/man/mkinitcpio.8
