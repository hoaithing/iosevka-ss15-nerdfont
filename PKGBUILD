# Packager: Hung Ha <hahungkk@gmail.com>
# Maintainer: Hung Ha <hahungkk@gmail.com>
pkgname=nerd-fonts-iosevka-ss15-extended
pkgver=5.0.4
pkgrel=4
pkgdesc="My own Iosevka (ss15 extended variant) patched font"
arch=("any")
url="https://github.com/ryanoasis/nerd-fonts"
license=('MIT')
depends=('fontconfig')
provides=('nerd-fonts-terminus')
conflicts=('ttc-iosevka-ss15', 'ttf-iosevka-ss15')

groups=("nerd-fonts")
source=("https://github.com/phuonghoanglua/iosevka-ss15-nerdfont/raw/main/Iosevka%20SS15%20Bold%20Extended%20Italic%20Nerd%20Font%20Complete.ttf"
        "https://github.com/phuonghoanglua/iosevka-ss15-nerdfont/raw/main/Iosevka%20SS15%20Bold%20Extended%20Nerd%20Font%20Complete.ttf"
        "https://github.com/phuonghoanglua/iosevka-ss15-nerdfont/raw/main/Iosevka%20SS15%20Extended%20Italic%20Nerd%20Font%20Complete.ttf"
        "https://github.com/phuonghoanglua/iosevka-ss15-nerdfont/raw/main/Iosevka%20SS15%20Extended%20Nerd%20Font%20Complete.ttf")

sha1sums=('6835eba39fac7d1cb18ae1836e6decb0fc0b63ad'
          '70a878b62c22332c8b577de48aec151399535b0c'
          '457af9f2b1195333e46adb6a82006c53670d1712'
          'f783194d91985b92f203c1ae06792b0ea3da2af3')

package() {
  find . -iname "*.ttf" -execdir install -Dm644 {} "$pkgdir/usr/share/fonts/TTF/{}" \;

  install -Dm644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}

