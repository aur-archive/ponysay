# Maintainer: Sven-Hendrik Haase <sh@lutzhaase.com>
# Contributor: Erkin Batu Altunbaş <erkinbatu@gmail.com>
pkgname=ponysay
pkgver=0.6
pkgrel=1
pkgdesc="Pony wrapper for cowsay."
url="https://github.com/erkin/ponysay"
arch=('any')
license=('WTFPL')
depends=('cowsay' 'bash')
source=(ponysay-${pkgver}.tar.gz::https://github.com/erkin/ponysay/tarball/${pkgver})
md5sums=('605ce7dd3218bc41d44d03d9d9b7bc8e')

build() {
    true
}
package() {
    cd ${srcdir}/erkin-ponysay-*
    make DESTDIR="${pkgdir}" install
    install -Dm644 COPYING "$pkgdir/usr/share/licenses/$pkgname/COPYING"
}
