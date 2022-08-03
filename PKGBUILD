# Maintainer: dr460nf1r3 <dr460nf1r3 at chaotic dot cx>
# Maintainer: Pedro H. Lara Campos <root@pedrohlc.com>
# Thanks for archlinuxcn's package that I've used as template!

pkgname='chaotic-keyring'
pkgver='20220803'
pkgrel=1
pkgdesc='Chaotic-AUR PGP keyring'
arch=('any')
url='https://aur.chaotic.cx'
license=('GPL')
depends=('archlinux-keyring')
optdepends=('pkgstats: install to submit package usage statistics')
install=$pkgname.install
source=("keyring-$pkgver-$pkgrel.tar.gz::https://github.com/chaotic-aur/keyring/archive/$pkgver-$pkgrel.tar.gz")
sha512sums=('faa9805dfdaf7cb809fe186d85724964f0ff7304008dd0d9e7379ae5649a103971ecd653326abca77092a6395b62da94eedc144c15679ac4c4b920229ebe23e8')

package() {
  cd "$srcdir/keyring-$pkgver-$pkgrel"
  make PREFIX=/usr "DESTDIR=$pkgdir" install
}


