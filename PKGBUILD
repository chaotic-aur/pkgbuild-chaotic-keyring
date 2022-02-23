# Maintainer: dr460nf1r3 <dr460nf1r3 at chaotic dot cx>
# Maintainer: Pedro H. Lara Campos <root@pedrohlc.com>
# Thanks for archlinuxcn's package that I've used as template!

pkgname='chaotic-keyring'
pkgver='20220220'
pkgrel=1
pkgdesc='Chaotic-AUR PGP keyring'
arch=('any')
url='https://aur.chaotic.cx'
license=('GPL')
depends=('archlinux-keyring')
optdepends=('pkgstats: install to submit package usage statistics')
install=$pkgname.install
source=("keyring-$pkgver-$pkgrel.tar.gz::https://github.com/chaotic-aur/keyring/archive/$pkgver-$pkgrel.tar.gz")
sha512sums=('47d1ac2569d211b9c486ef01b01b8fda4276a84934f3f5302460215c28be623fcb6d1f7bc897cdff3f87dbe9dbf28135671ae64fe8ad328240a5710bcda8c004')

package() {
  cd "$srcdir/keyring-$pkgver-$pkgrel"
  make PREFIX=/usr "DESTDIR=$pkgdir" install
}


