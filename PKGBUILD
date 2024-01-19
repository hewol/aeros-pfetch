# Maintainer: Qontinuum <qontinuum.dev@protonmail.ch>
# Contributor: Caio Novais <caionov08 at gmail dot com>

pkgname=pfetch
pkgver=0.6.0
pkgrel=4
pkgdesc="A pretty system information tool written in POSIX sh."
arch=('any')
url="https://github.com/hewol/aeros-$pkgname"
license=('MIT')
provides=("$pkgname")
conflicts=('pfetch-git')
source=("https://github.com/hewol/aeros-pfetch/zipball/HEAD")
b2sums=('SKIP')

package() {
  mv HEAD pfetch.zip
  7z x pfetch.zip "$srcdir"
  install -Dm755 $srcdir/hewol-aeros-pfetch-*/pfetch "$pkgdir/usr/bin/pfetch"
  install -Dm644 $srcdir/hewol-aeros-pfetch-*/LICENSE.md "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
