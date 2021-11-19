# Maintainer: dr460nf1r3 <dr460nf1r3 at chaotic dot cx>
# Maintainer: Pedro H. Lara Campos <root@pedrohlc.com>
# Thanks for archlinuxcn's package that I've used as template!

pkgname='chaotic-keyring'
pkgver='20210617'
pkgrel=2
pkgdesc='Chaotic-AUR PGP keyring'
arch=('any')
url='https://aur.chaotic.cx'
license=('GPL')
depends=('archlinux-keyring')
optdepends=('pkgstats: install to submit package usage statistics')
install=$pkgname.install
source=("keyring-$pkgver-$pkgrel.tar.gz::https://github.com/chaotic-aur/keyring/archive/$pkgver-$pkgrel.tar.gz")
sha512sums=('d28899ee38ccb7fc86ad35fff9a799ab36aa4e507ba8394908e1094f3a2ea92963b65931e17abb4ed85fcb990bd5bf7bd2c82f919aea8d2530ec8b01dd32afba')

package() {
  cd "$srcdir/keyring-$pkgver-$pkgrel"
  make PREFIX=/usr "DESTDIR=$pkgdir" install
}


