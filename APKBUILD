#Maintainer: Devyansh vishwakarma <devyanshnayak@gmail.com>

pkgname=lutris
pkgver=0.5.9
pkgrel=2
pkgdesc='Open Gaming Platform'
arch='x86_64'
url='https://lutris.net/'
license='GPL3'
depends="desktop-file-utils hicolor-icon-theme polkit xrandr
         py3-dbus py3-gobject3 py3-yaml py3-evdev
         sqlite-libs cabextract"
optdepends="wine: recommended to avoid dependency issues
    wine-staging: recommended to avoid dependency issues (Staging patches)
    wine-gaming-nine: recommended to avoid dependency issues (Gallium9 patches)"

makedepends='py3-setuptools'
source="https://lutris.net/releases/lutris_${pkgver}.tar.xz"
sha512sums="49cee97aaac12c64a5fb9a38ae2e091bfd918d5c6305b5c6fbffde89f7c03fa85c8853bcb6d347ebbf66bab19d7d75ebcd54e064dbd847ec2c579c13161bddf6  lutris_0.5.9.tar.xz"
build() {
    echo "building"
}
package() {
  cd src/lutris

  python setup.py install --root="${pkgdir}" --optimize='1'
}

# vim: ts=2 sw=2 et:
