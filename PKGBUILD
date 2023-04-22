# Maintainer: David7ce
pkgname=calamares-arksys-config
_destname="/etc"
pkgdesc="ArkSys calamares installer configuration"
pkgver=0.2
pkgrel=1
arch=('any')
url="https://github.com/arksys-os/"
license=('GPL3')
makedepends=('git')
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${pkgname}::"git+${url}/${pkgname}")
sha256sums=('SKIP')

package() {
	install -dm755 ${pkgdir}${_destname}
	cp -r ${srcdir}/${pkgname}${_destname}/* ${pkgdir}${_destname}
	rm ${srcdir}/${pkgname}/README.md
	rm ${srcdir}/${pkgname}/PKGBUILD
}
