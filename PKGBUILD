pkgname=python-distutils-extra
pkgver=2.39
pkgrel=6
pkgdesc='Enhancements to the Python build system'
arch=('x86_64')
license=('GPL')
url='https://launchpad.net/python-distutils-extra'
depends=('intltool' 'python3')
makedepends=('python3-setuptools' 'intltool')
source=(https://launchpad.net/$pkgname/trunk/$pkgver/+download/$pkgname-$pkgver.tar.gz)
# https://launchpad.net/python-distutils-extra/trunk/2.39/+download/python-distutils-extra-2.39.tar.gz.asc
        #$pkgbase-$pkgver.tar.gz.sig::http://launchpad.net/$pkgbase/trunk/$pkgver/+download/dist-$pkgbase-$pkgver.tar.gz.sig)
md5sums=('16e06db0ef73a35b4bff4b9eed5699b5')

package() {
  cd "${srcdir}/$pkgname-$pkgver"
  python3 setup.py install --root="${pkgdir}"
}
