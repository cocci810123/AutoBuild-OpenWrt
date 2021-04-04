# AutoBuild-OpenWrt

[![GitHub release (latest by date)](https://img.shields.io/github/v/release/cocci810123/AutoBuild-OpenWrt?style=flat-square)](https://github.com/cocci810123/AutoBuild-OpenWrt/releases)
[![GitHub stars](https://img.shields.io/github/stars/cocci810123/AutoBuild-OpenWrt?style=flat-square)](https://github.com/cocci810123/AutoBuild-OpenWrt/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/cocci810123/AutoBuild-OpenWrt?style=flat-square)](https://github.com/cocci810123/AutoBuild-OpenWrt/network/members)
<!-- ![GitHub All Releases](https://img.shields.io/github/downloads/cocci810123/AutoBuild-OpenWrt/total?style=flat-square) -->

1. 自动编译固件基于Lean的固件编译
2. 自动编译文件build-openwrt.yml基于P3TERX,eSir和Lean的workflows文件修改
3. 通过P3TERX的源码更新自动编译文件update-checker.yml保持Lean固件源码更新后自动进行新版本的固件编译
4. 通过kolpav的Delete artifacts action方法创建的delete-old-artifacts.yml可以自动删除旧工件保证上传固件目录时有足够的存储空间
