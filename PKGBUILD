# Maintainer: Tristelune  <tristelune1 at gmail dot com>
pkgname=kinskydesktop
pkgver=4.3.13
pkgrel=1
pkgdesc="UPNP/DLNA control point"
url="http://oss.linn.co.uk/trac/wiki/Kinsky"
arch=('i686' 'x86_64')
license=('BSD')
depends=('mono')
source=('http://oss.linn.co.uk/Releases/Kinsky/Davaar/kinsky_4.3.13-1_all.deb'
		'kinsky.patch')
md5sums=('47aa4a22432a42b70a720c7a050cb51e'
		'860c473926ddf57718b161728231abd4')

build(){
	cd "${srcdir}"
	tar xvzf data.tar.gz
	cd ${srcdir}/usr/
	patch -p1 -i ${srcdir}/kinsky.patch
}

package(){
	cd "${srcdir}"
	mv usr/ ${pkgdir}/
}
