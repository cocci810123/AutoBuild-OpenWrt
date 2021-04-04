# AutoBuild-OpenWrt

1. 自动编译固件基于Lean的固件编译
2. 自动编译文件build-openwrt.yml基于P3TERX,eSir和Lean的workflows文件修改
3. 通过P3TERX的源码更新自动编译文件update-checker.yml保持Lean固件源码更新后自动进行新版本的固件编译
4. 通过kolpav的Delete artifacts action方法创建的delete-old-artifacts.yml可以自动删除旧工件保证上传固件目录时有足够的存储空间
