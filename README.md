# WSDMatty's AUR Packages

Package sources for all the AUR packages I officially [maintain](https://aur.archlinux.org/packages/?SeB=m&K=WSDMatty), [co-maintain](https://aur.archlinux.org/packages/?SeB=c&K=WSDMatty), or unofficially host modified versions of.

## Pacman Package Repository

To make use of this repository you must first add my gpg key to your pacman keyring with pacman-key.

```sh
pacman-key --recv-keys 97928FA059F8050487930EAFACF6C1A315EDCB52
pacman-key --lsign-key 97928FA059F8050487930EAFACF6C1A315EDCB52
```
Note if you have trouble with your default key servers not being reachable try adding `--keyserver keyserver.ubuntu.com` to the first command.

Then add the following repository configuration to your `pacman.conf` after the *[extra]* repository.

```ini
[wsdm]
Server = https://wsdmatty.github.io/$repo/$arch
```
