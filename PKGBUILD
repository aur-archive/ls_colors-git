# Maintainer: Testuser_01 <arch@nico-siebler.de>

pkgname=ls_colors-git
_pkgname=LS_COLORS
pkgver=20110925
pkgrel=1
pkgdesc="This is a collection of extension:color mappings, suitable to use as your LS_COLORS environment variable."
url="https://github.com/trapd00r/LS_COLORS"
arch=('any')
install="${pkgname}.install"
license=('unknown')

build() {
  git clone git://github.com/trapd00r/LS_COLORS.git --depth=1 || return 1
  mkdir -p ${pkgdir}/usr/share || return 1
  install -D ${srcdir}/${_pkgname}/LS_COLORS ${pkgdir}/usr/share || return 1
}

