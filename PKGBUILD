# Maintainer: David7ce
pkgname=(arksys-calamares-config)
_destname="/etc"
pkgdesc="Calamares installer conf for Arksys"
pkgver=23.08
pkgrel=20
arch=('any')
url="https://github.com/arksys-os/"          # url="file://${PWD}" 
license=('GPL3')
makedepends=('git')
depends=()
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${pkgname}::"git+${url}/${pkgname}") # source=(${pkgname}::"git+${url}")
sha256sums=('SKIP')

package() {
	install -dm755 ${pkgdir}${_destname}
	cp -r ${srcdir}/${pkgname}${_destname}/* ${pkgdir}${_destname}
	rm ${srcdir}/${pkgname}/build.sh
	rm ${srcdir}/${pkgname}/README.MD
	rm ${srcdir}/${pkgname}/PKGBUILD
}
