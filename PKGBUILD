# Maintainer: Robin Baumgartner <robin@baumgartners.ch>
pkgname=trytond-company
_pkgname=trytond_company
pkgver=3.4.1
_pkgdir=3.4
pkgrel=1
pkgdesc="The company module of the Tryton application platform"
arch=('any')
url='http://www.tryton.org/'
license=('GPL3')
groups=('trytond-modules')
depends=('trytond>=3.4' 'trytond-currency>=3.4' 'trytond-party>=3.4')
makedepends=('python2-distribute')
source=("http://downloads.tryton.org/$_pkgdir/$_pkgname-$pkgver.tar.gz")
md5sums=("7bc2aa6689b5d1f0fac6d372cbef76ee")

build() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py build
}

package() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py install --root=$pkgdir
}