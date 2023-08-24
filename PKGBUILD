# Maintainer: David7ce
pkgname=(arksys-calamares-config)
_destname="/etc"
pkgdesc="Calamares installer conf for Arksys"
pkgver=23.08
pkgrel=20
arch=('any')
url="file://${PWD}" # url="https://github.com/arksys-os/"
license=('GPL3')
makedepends=('git')
depends=()
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${pkgname}::"git+${url}")  # source=(${pkgname}::"git+${url}/${pkgname}")
sha256sums=('SKIP')

package() {
	install -dm755 ${pkgdir}${_destname}
	cp -r ${srcdir}/${pkgname}${_destname}/* ${pkgdir}${_destname}
	rm ${srcdir}/${pkgname}/build.sh
	rm ${srcdir}/${pkgname}/README.md
	rm ${srcdir}/${pkgname}/PKGBUILD
}
