# Maintainer: StormOSDev <linuxstormos@gmail.com>
pkgname=stormos-etc-skel-config
_destname1="/etc"
pkgver=08.28.23
pkgrel=1
pkgdesc="Desktop Config for StormOS"
arch=('any')
url="https://gitlab.com/bfitzgit23"
license=('GPL3')
makedepends=('git')
conflicts=()
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${pkgname}::"git+${url}/${pkgname}")
sha256sums=('SKIP')
package() {
	install -dm755 ${pkgdir}${_destname1}
	cp -r ${srcdir}/${pkgname}${_destname1}/* ${pkgdir}${_destname1}
	rm ${srcdir}/${pkgname}/push.sh
	rm ${srcdir}/${pkgname}/README.md
	rm ${srcdir}/${pkgname}/PKGBUILD
}
