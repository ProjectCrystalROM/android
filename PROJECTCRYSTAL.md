# ProjectCrystalROM CM12.1

Fork of the upstream Android manifest using the standard cm-12.1 branch and
project layout. Modified projects select ProjectCrystalROM forks; unchanged
projects retain upstream selections, including the separate CAF RIL entry.

repo init -u https://github.com/ProjectCrystalROM/android.git -b cm-12.1
repo sync

Supported integration: LG K7 MS330, Android5.1.1/API22, independent custom kernel
at kernel/lge/m1-custom. Use the established Trusty/Java7 build environment and
stage the pinned original microG APKs/ARM JNI using the vendor helper. Retain
original APK signatures. TWRP is required; CM12 Cyanogen recovery is broken.

The component revisions are hardware-qualified. This manifest mapping passed
XML/path/branch checks but awaits a fresh sync/full-build qualification. Existing
CM12 checkout was not re-synced or overwritten. No private keys/images included.

The common-tree security/cm12.1-asb branch holds the single security ledger.
Security research/backports/validation are CM12.1-only. Pending APN-source
default changes remain on vendor/cm pending/cm12.1-apn-defaults until tested.
