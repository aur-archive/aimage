# Contributor: Abakus <java5 at arcor dot de>
pkgname=aimage
pkgver=3.2.4
pkgrel=1
pkgdesc="is a program to create aff-images"
arch=('i686' 'x86_64')
url="http://www.afflib.org"
license=('GPL')
depends=('afflib')
source=("http://www.afflib.org/downloads/${pkgname}-${pkgver}.tar.gz")
md5sums=('bb6e4e91524612570a481b6470fe7cd1')

build() {
	cd $srcdir/$pkgname-$pkgver
	./configure --prefix=/usr --sysconfdir=/etc
	make || return 1
	make DESTDIR=$pkgdir install || return 1
}

