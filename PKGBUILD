# Contributor: Krzysztof Raczkowski <raczkow@gnu-tech.pl>
pkgname=servicemenu-pdf-kde4
pkgver=0.4
pkgrel=6
pkgdesc="File Manager extra PDF managing options in KDE4."
arch=('any')
url="http://kde-look.org/content/show.php/servicemenu-pdf+for+KDE4?content=37321"
license=('GPL')
depends=('kdebase-workspace>=4.5.0' 'ghostscript' 'texlive-core' 'poppler' 'pdftk')
source=(http://www.egregorion.net/works/servicemenus/servicemenu-pdf_0.4-kde4.tar.gz)
md5sums=('c3f6edf58592ad6645be33f6d0f2390a')

build() {
#  tar -xvf ${srcdir}/servicemenu-pdf_$pkgver-kde4.tar.gz
  mkdir -p ${pkgdir}/usr/share/kde4/services/ServiceMenus/
  mkdir -p ${pkgdir}/usr/bin/
  install -m 644 ${srcdir}/servicemenu-pdf_$pkgver-kde4/desktop/*.desktop ${pkgdir}/usr/share/kde4/services/ServiceMenus/
  install -m 755 ${srcdir}/servicemenu-pdf_$pkgver-kde4/bin/* ${pkgdir}/usr/bin/
}
