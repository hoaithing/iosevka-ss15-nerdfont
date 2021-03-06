# Packager: Hung Ha <hahungkk@gmail.com>
# Maintainer: Hung Ha <hahungkk@gmail.com>
pkgname=nerd-fonts-iosevka-ss15-extended
pkgver=5.0.4
pkgrel=4
pkgdesc="My Patched font Iosevka (ss15 extended variant)"
arch=("any")
url="https://github.com/ryanoasis/nerd-fonts"
license=('MIT')
depends=('fontconfig')
provides=('nerd-fonts-terminus')
conflicts=('ttc-iosevka-ss15', 'ttf-iosevka-ss15')

groups=("nerd-fonts")
source=("https://github.com/ryanoasis/nerd-fonts/releases/download/v$pkgver/Terminus.zip"
        "https://github.com/ryanoasis/nerd-fonts/raw/v$pkgver/LICENSE")

sha1sums=('edccce964227868dc866fd32f92d6b10e41dd598'
          '92fdad3c8babc0473da5f03e41fb1151417ab386')

package() {
  find . -iname "*.ttf" -execdir install -Dm644 {} "$pkgdir/usr/share/fonts/TTF/{}" \;

  install -Dm644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}

