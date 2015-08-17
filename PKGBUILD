# Maintainer: Michal Krenek (Mikos) <m.krenek@gmail.com>
pkgname=qopenvpn
pkgver=1.2
pkgrel=1
pkgdesc="Simple OpenVPN GUI written in PyQt for systemd based distributions"
arch=('any')
url="https://github.com/xmikos/qopenvpn"
license=('GPL3')
depends=('python-pyqt4')
source=(https://github.com/xmikos/qopenvpn/archive/$pkgver.tar.gz)
md5sums=('46abc9f7190073c2f30526e5769252a9')

build() {
  cd "$srcdir/$pkgname-$pkgver"
  python setup.py build
}

package() {
  cd "$srcdir/$pkgname-$pkgver"
  python setup.py install --root="$pkgdir"
}

# vim:set ts=2 sw=2 et:
