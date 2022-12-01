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
354079b4b20507d9bf4f6cdcc83832ec26eaa451f2dde6e28a9b1c81b22db944b6b656b192041d05be67ecd1e6e412ad312ab3b7d59f6a6822fef18244e52989  deviceinfo
646cedb1c4675ef04530f8cab305a48767ddc894d1d08541aae3a4c124268ca9ef88aa4fa6ad507d8618f4355144a206a32f5a75ade8e60ab1fc9a338d5209f8  fb.modes
19b0a9ae89ad4ad1adfcc2a1b5a1abfe71f560c2857e392f904c393f0b3bb4d29d7c2fbf8e080227d50e7e13f53fd5a5f3b0902c89582ec3e2742430ade19f07  directfbrc
"
