# Maintainer: DarkXero <info@techxero.com>
pkgname=kde-wallpapers-extra
_destname1="/"
pkgver=1.0
pkgrel=1
pkgdesc="More KDE Wallpapers"
arch=('any')
url="https://github.com/xerolinux"
license=('GPL3')
makedepends=('git')
depends=()
conflicts=()
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${pkgname}::"git+${url}/${pkgname}")
sha256sums=('SKIP')
package() {
	install -dm755 ${pkgdir}${_destname1}
	cp -r ${srcdir}/${pkgname}${_destname1}/* ${pkgdir}${_destname1}
	rm ${pkgdir}${_destname1}/LICENSE
	rm ${pkgdir}${_destname1}/README.md
	rm ${pkgdir}${_destname1}/PKGBUILD
}
