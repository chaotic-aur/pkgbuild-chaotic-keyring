# Maintainer: dr460nf1r3 <dr460nf1r3 at chaotic dot cx>
# Maintainer: Pedro H. Lara Campos <root@pedrohlc.com>
# Thanks for archlinuxcn's package that I've used as template!

pkgname='chaotic-keyring'
pkgver='20220130'
pkgrel=1
pkgdesc='Chaotic-AUR PGP keyring'
arch=('any')
url='https://aur.chaotic.cx'
license=('GPL')
depends=('archlinux-keyring')
optdepends=('pkgstats: install to submit package usage statistics')
install=$pkgname.install
source=("keyring-$pkgver-$pkgrel.tar.gz::https://github.com/chaotic-aur/keyring/archive/$pkgver-$pkgrel.tar.gz")
sha512sums=('9e2ceb837b2831dbfdce5627deed92b477aa46d924b3c658da04bb494d8faa8f4a8a1c0ecc26729fa316b601a32a17bf6c9d16bb7d401266e45e1dd2d22e1ae8')

package() {
  cd "$srcdir/keyring-$pkgver-$pkgrel"
  make PREFIX=/usr "DESTDIR=$pkgdir" install
}


