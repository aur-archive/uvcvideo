pkgname=uvcvideo
pkgver=r104
pkgrel=2
arch=('any')
pkgdesc="uvcvideo is a class of usb video driver"
url="http://mxhaard.free.fr/"
depends=('git')
makedepends=('linux-headers')
conflicts=()
replaces=()
backup=()
source=("git://github.com/NetworkOffice/uvcvideo")
md5sums=('SKIP')

build() {
  cd "$srcdir/uvcvideo"
	make
}

package() {
  cd "$srcdir/luvcview"
  make prefix="$pkgdir/usr/" install
}

# vim:set ts=2 sw=2 et:
