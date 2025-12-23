# Maintainer: @zstg <zestig@duck.com>
pkgname=stratos-ghostty-config
pkgver=1.0
pkgrel=1
pkgdesc="Ghostty configuration for StratOS"
arch=('any')
license=('GPL3')
depends=(
    'ghostty'
    'ttf-jetbrains-mono'
    'ttf-jetbrains-mono-nerd'
)
source=()
install=stratos-ghostty-config.install

prepare() {
	cp -r "$startdir/.config/" "$srcdir/"
}

package() {
    install -d "$pkgdir/etc/skel/.config"
    cp -r "$srcdir/.config/ghostty/" "$pkgdir/etc/skel/.config/"
}
