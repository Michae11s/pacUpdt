# Maintainer: Kyle Michaels <Kyle@michaels.pro>
pkgname=pacUpdt
pkgver=1.04
pkgrel=1
pkgdesc="Runs checkupdates from pacman-contrib, counts the lines and writes to /etc/pacUpdt/count, then able to be used in things like neofetch"
arch=('any')
url=""
license=('GPL3')
depends=('pacman-contrib'
         'auracle')

source=("pacUpdt"
        "pacUpdt.service"
        "pacUpdt.timer")

package() {
    cd $pkgdir

    mkdir -p usr/bin
    mkdir -p etc/pacUpdt
    mkdir -p usr/lib/systemd/system

    cp $srcdir/pacUpdt usr/bin
    cp $srcdir/pacUpdt.service usr/lib/systemd/system
    cp $srcdir/pacUpdt.timer usr/lib/systemd/system

}

md5sums=('e8160f7ced24e05cb5cf74377a6f47b7'
         'dba6d06259fd9ef867d7ffaae128baa7'
         '4f08039e8b907be25aa795a9d3bb1780')
