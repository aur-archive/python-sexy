# $Id: $
# Maintainer: Allan McRae <allan@archlinux.org>
# Contributor: Jeff Bailes <thepizzaking@gmail.com>
# Contributor: William Rea <sillywilly@gmail.com>

pkgname=python-sexy
pkgver=0.1.9
pkgrel=4
pkgdesc="Python bindings for libsexy"
arch=('i686' 'x86_64')
url="http://chipx86.com/wiki/Libsexy"
license=('LGPL')
depends=('pygtk' 'libsexy')
options=('!libtool')
source=(http://releases.chipx86.com/libsexy/sexy-python/sexy-python-$pkgver.tar.gz)
md5sums=('313f11e98555b0e9eea28219564e5063')


build() {
  cd $srcdir/sexy-python-$pkgver
  ./configure --prefix=/usr
  make || return 1
  make DESTDIR=$pkgdir install || return 1
}
