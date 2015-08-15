# Maintainer: Daniel Beecham <daniel@lunix.se>
# Contributor: Jens Staal <staal1978@gmail.com>

options=(!strip)
pkgname="gnu2busybox-grep"
pkgver="1"
pkgrel=2
pkgdesc="Replaces GNU grep with the corresponding commands from Busybox."
arch=('any')
url="http://busybox.net/"
license=('GPLv2')
depends=('busybox')
provides=('grep')
conflicts=('grep')

build() {
    msg "creating package directories"
    mkdir "$pkgdir/usr"
    mkdir "$pkgdir/usr/bin"

    msg "creating symlinks for /usr/bin"
    cd $pkgdir/usr/bin
    ln -s /bin/busybox grep
    ln -s /bin/busybox egrep
    ln -s /bin/busybox fgrep
}
 
