# Maintainer: Gia Phu <crystalforceix@gmail.com>
pkgname=compatibility-rollback-initramfs
pkgver=1.0.0
pkgrel=1
pkgdesc="Compatibility rollback hook support any filesystem for mkinitcpio"
arch=('any')
url="https://github.com/RengeOS/Compatibility-Rollback-Initramfs"
license=('GPL')
depends=('mkinitcpio' 'rsync' 'squashfs-tools')
install="${pkgname}.install"
source=()
sha256sums=()

package() {
    install -Dm644 "${startdir}/install/compatibility-rollback" \
        "${pkgdir}/usr/lib/initcpio/install/compatibility-rollback"
    
    install -Dm644 "${startdir}/hooks/compatibility-rollback" \
        "${pkgdir}/usr/lib/initcpio/hooks/compatibility-rollback"
}
