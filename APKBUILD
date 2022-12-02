pkgname=device-xiaomi-kenzo
pkgdesc="Xiaomi Redmi Note 3"
pkgver=1.0
pkgrel=0
url="https://postmarketos.org"
license="MIT"
arch="aarch64"
options="!check !archcheck"
depends="postmarketos-base mkbootimg soc-qcom-msm8916 linux-postmarketos-qcom-msm8956"
makedepends="devicepkg-dev"
source="deviceinfo"
subpackages="$pkgname-nonfree-firmware:nonfree_firmware"
build() {
	devicepkg_build $startdir $pkgname
}

package() {
	devicepkg_package $startdir $pkgname
}

nonfree_firmware() {
	pkgdesc="Proprietary firmware"
	depends="linux-firmware-qcom firmware-xiaomi-kenzo"
	mkdir "$subpkgdir"
}

sha512sums="
34102c2a02f7095324b743745f4db4529a84ff4b15ee601e80fa9af6404daf968815e772d0fdbf6aba9d86ba77bf04bad694129e0fd0b9ff8a5d19398c6c27dd  deviceinfo
"
