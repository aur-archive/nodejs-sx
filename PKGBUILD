# Maintainer: Andy Weidenbaum <archbaum@gmail.com>

pkgname=nodejs-sx
_npmname=node-sx
pkgver=0.0.19
pkgrel=1
pkgdesc="Node.js library for sx Bitcoin utilities"
arch=('any')
depends=('sx-git' 'nodejs')
makedepends=('sx-git' 'npm')
url="https://github.com/vbuterin/node-sx"
license=('MIT')
provides=('nodejs-sx')

package() {
  local _npmdir="$pkgdir/usr/lib/node_modules/"
  mkdir -p $_npmdir
  cd $_npmdir
  npm install --user root -g --prefix "$pkgdir/usr" $_npmname@$pkgver
}
