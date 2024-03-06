# Maintainer: dr460nf1r3 <dr460nf1r3 at chaotic dot cx>
# Maintainer: Pedro H. Lara Campos <root@pedrohlc.com>
# Thanks for archlinuxcn's package that I've used as template!

pkgname='chaotic-keyring'
pkgver='20240206'
pkgrel=1
pkgdesc='Chaotic-AUR PGP keyring'
arch=('any')
url='https://aur.chaotic.cx'
license=('GPL')
depends=('archlinux-keyring')
replaces=('chaotic-kf5-dummy')
optdepends=('pkgstats: install to submit package usage statistics')
install=$pkgname.install
source=("keyring-$pkgver-$pkgrel.tar.gz::https://github.com/chaotic-aur/keyring/archive/$pkgver-$pkgrel.tar.gz")
sha512sums=('dbdd8f939ec6ebc654a64603adb7a03d59845eed2fbd84957a3dd62e26b2828481026667437bcccdc74cef2173a9ed61bb44e5193d05c678a0c77d871be5c44e')

package() {
  cd "$srcdir/keyring-$pkgver-$pkgrel"
  make PREFIX=/usr "DESTDIR=$pkgdir" install
}


