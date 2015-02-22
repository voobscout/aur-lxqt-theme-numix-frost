# Maintainer: Voobscout <voobscout+aur@gmail.com>
pkgname=lxqt-theme-numix-frost
pkgver=1.0
pkgrel=1
pkgdesc="Numix Frost theme for LXQT"
arch=('any')
license=('unknown')
makedepends=('git' 'pkg-config' 'autoconf' 'automake' 'gettext' 'xproto' 'xtrans' 'wget')
url="https://intialonso.github.io/"
provides=('lxqt-theme-numix-frost')
source=("https://github.com/intialonso/intialonso.github.io/blob/master/themes/Numix-Frost.tar.gz?raw=true")
sha256sums=('c9592b922b4ec9153556b44e3b51373d9aca7dcf94afa80a7d05553d0f93e182')
options=(!strip)

prepare() {
  msg "Unpacking tar.gz..."
  tar xvzf "Numix-Frost.tar.gz?raw=true"
}

build() {
  msg "Nothing to build..."
}

package() {
  msg "Installing Numix-Frost theme"

  install -m 0755 \
          -d \
          ${pkgdir}/usr/share/lxqt/themes/Numix-Frost \
          ${pkgdir}/usr/share/lxqt/themes/Numix-Frost/lxqt-lightdm-greeter \
          ${pkgdir}/usr/share/lxqt/themes/Numix-Frost/lxqt-power \
          ${pkgdir}/usr/share/lxqt/themes/Numix-Frost/lxqt-runner

  install -m 0644 \
          --target-directory=${pkgdir}/usr/share/lxqt/themes/Numix-Frost \
          ${srcdir}/Numix-Frost/*.png \
          ${srcdir}/Numix-Frost/*.cfg \
          ${srcdir}/Numix-Frost/*.qss \
          ${srcdir}/Numix-Frost/*.svg

  install -m 0644 \
          --target-directory=${pkgdir}/usr/share/lxqt/themes/Numix-Frost/lxqt-lightdm-greeter \
          ${srcdir}/Numix-Frost/lxqt-lightdm-greeter/*

  install -m 0644 \
          --target-directory=${pkgdir}/usr/share/lxqt/themes/Numix-Frost/lxqt-power \
          ${srcdir}/Numix-Frost/lxqt-power/*

  install -m 0644 \
          --target-directory=${pkgdir}/usr/share/lxqt/themes/Numix-Frost/lxqt-runner \
          ${srcdir}/Numix-Frost/lxqt-runner/*
}
# vim:set ts=2 sw=2 et:
