# Maintainer: vn158 <vn158 at seznam dot cz>
pkgname=fiosign
pkgver=4.0.2
pkgrel=1
pkgdesc="Fio bank signing tool."
arch=('i686' 'x86_64')
url="http://www.fio.cz"
license=('custom:free')
groups=()
depends=(java-jce_ustrength)
makedepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=(!strip)

source=(http://www.fio.cz/apps/signer_client.jar http://www.fio.cz/apps/bcprov-jdk16-146.jar $pkgname)
noextract=(signer_client.jar bcprov-jdk16-146.jar)

md5sums=('c7e905fc969205b58ad19802e44f8061'
         '881ce7b0e75a764892eafa63af7e4d38'
         '96a46c0a1737038982eec27df09fb73f')
sha1sums=('2a158ee7f298af0ccc335d60e083e59b4e584679'
          'ce091790943599535cbb4de8ede84535b0c1260c'
          '970199b7757ceb43ed04446c729d84da4131e492')

package() {
  cd "$startdir"
  install -d -m755 $pkgdir/usr/share/$pkgname
  install -d -m755 $pkgdir/usr/bin
  install -m644 *.jar $pkgdir/usr/share/$pkgname
  install -m755 $pkgname $pkgdir/usr/bin
}
