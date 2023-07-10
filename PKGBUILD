pkgname=change-wallpaper
pkgver=0.0.0
pkgrel=1
pkgdesc="User script to change wallpaper"
arch=("x86_64")
url="https://github.com/leonixyz"
license=("GPL")
depends=(
    "python-requests"
)
source=(
    "change_wallpaper"
    "change-wallpaper.service"
    "change-wallpaper.timer"
)
md5sums=(
    "aa0f694ce8878bf71af88f01b9dd20e6"
    "508e239b67bd7e1f99de442a8bc562c1"
    "784c65799fc0cbe2cae4244535d572f8"
)

package() {
    install -Dm0755 change_wallpaper "$pkgdir"/usr/local/bin/change_wallpaper
    install -Dm0644 change-wallpaper.service "$pkgdir"/usr/lib/systemd/user/change-wallpaper.service
    install -Dm0644 change-wallpaper.timer "$pkgdir"/usr/lib/systemd/user/change-wallpaper.timer
}
