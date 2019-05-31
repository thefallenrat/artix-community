# Maintainer: nous

pkgname=artix-dark-theme
pkgver=20190601
pkgver() {
  date +%Y%m%d
}
pkgrel=1
pkgdesc="Dark themes for the community ISOs of Artix Linux. GTK2/3, QT5, Plasma splash."
arch=('any')
url="https://gitea.artixlinux.org/nous/artix-dark-theme"
license=('GPL')
source=('git+https://gitea.artixlinux.org/nous/artix-dark-theme.git')
sha256sums=('SKIP')
depends=('artix-backgrounds' 'artix-icons')
makedepends=('git')
optdepends=('gtk2' 'gtk3' 'qt5' 'plasma' 'gtk-engines' 'xcursor-premium' 'qt5ct' 'openbox')

package() {
  cd "${srcdir}/$pkgname"
  mkdir -p "${pkgdir}"/usr/share/themes
  cp -rf usr "${pkgdir}"/
}
