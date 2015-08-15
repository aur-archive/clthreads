# Maintainer : SpepS <dreamspepser at yahoo dot it>
# Contributor: Christoph Zeiler <rabyte*gmail>
# Contributor: Tom K <tomk@runbox.com>
# Contributor: Shinlun Hsieh <yngwiexx@yahoo.com.tw>
# Contributor: Philipp Überbacher <murks at lavabit dot com>

pkgname=clthreads
pkgver=2.4.0
pkgrel=5
pkgdesc="C++ wrapper library around the POSIX threads API"
arch=('i686' 'x86_64')
url="http://kokkinizita.linuxaudio.org/linuxaudio/downloads/index.html"
license=('LGPL')
source=("http://kokkinizita.linuxaudio.org/linuxaudio/downloads/$pkgname-$pkgver.tar.bz2")
md5sums=('90b650f1f5c9f39f4d77f73aca3c53be')

build() {
  cd "$pkgname-$pkgver"
  make
}

package(){
  cd "$pkgname-$pkgver"
  install -d "$pkgdir/usr/include"
  make PREFIX="$pkgdir/usr" LIBDIR=lib install
}
