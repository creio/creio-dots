# Maintainer: Alex Creio <ctlos@protonmail.com>

pkgname=creio-dots
_pkgname=dots
pkgdesc='Alex Creio dot files repo'
pkgver=v1.0.0
pkgrel=1
arch=(x86_64)
license=('WTFPL')
install=README.install
url="https://github.com/creio/dots"
makedepends=('git')
depends=(
         polkit-gnome
         openbox
)

source+=("${url}/archive/${pkgver}.tar.gz")
sha256sums=('SKIP')

# pkgver() {
#   cd ${_pkgname}
#   git log -1 --date=short --pretty=format:%ad | sed 's/-//g'
# }

package() {
  cd ${srcdir}
  mkdir -p "${pkgdir}/etc/skel"
  mkdir -p "${pkgdir}/etc/creio-dots"

  cp -rf . "$pkgdir/etc/creio-dots"
}
