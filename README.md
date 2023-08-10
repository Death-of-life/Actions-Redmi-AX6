[![GitHub release (latest by date)](https://img.shields.io/github/v/release/shawnpxtl/Actions-Redmi-AX6?style=for-the-badge&label=下载)](https://github.com/Death-of-life/Actions-Redmi-AX6/releases/latest)

### ⚠注意：值守式系统更新千万不要操作，且最好在值守式系统更新的配置中把下载地址去掉，否则真的会影响使用的！！！⚠

# 关于这个仓库

> 这个仓库基于[P3TERX/Actions-OpenWrt](https://github.com/P3TERX/Actions-OpenWrt)<br>
> [OpenWRT](https://github.com/openwrt/openwrt)/[ImmortalWrt](https://github.com/immortalwrt/immortalwrt)分支来自官方源码<br>
Fork自 [shawnpxtl](https://github.com/shawnpxtl/Actions-Redmi-AX6)
用Github Actions为AX6自动编译固件  
本项目的固件原则上每周自动编译一次，您也可以fork自行修改~  
如果您觉得本项目不错的话，可以Star一下，我会感激不尽的！就酱~  

## 特性

* [Passwall](https://github.com/xiaorouji/openwrt-passwall)
* [cloudflarespeedtest](https://github.com/mingxiaoyu/luci-app-cloudflarespeedtest)
* UU加速器
  
  cf测速可以每日自动优选ip更新passwall节点 配合[worker-vless](https://github.com/zizifn/edgetunnel/blob/main/src/worker-vless.js)使用体验极佳
  uu加速器和passwall可以完美共存互补影响

## 刷入教程

您是要刷[ImmortalWrt](tutorial/ImmortalWrt.md)还是刷[OpenWrt](tutorial/OpenWrt.md)呢？

## 后台进入方式和密码

   | 项目 | 值 |
   | :--- | :--- |
   | 默认后台地址 | `10.0.0.1`/`http://immortalwrt.lan/` |
   | 默认后台密码 | `无密码` |

## 其它教程（大多数教程均来自互联网，此处作备份用） <a id="tutorial"></a>

* [如何更新固件](tutorial/ru-he-geng-xin-gu-jian.md)
* [在刷入uboot后如何刷回官方固件](tutorial/with-uboot-Flashback-to-stock-firmware.md)
* [让AdGuard Home和OpenClash共存(自己做的设置，测试适用于本固件)](tutorial/adguard-openclash.md)
* [AX6双系统](tutorial/ax6-dualsystm.md)

## 截图

![luci\_admin\_status\_overview](https://s2.loli.net/2023/08/10/9Bm7oAJh4dXiELI.png)

## 已知问题
#### 免责声明：以下已知问题均为个人实测，可能还有未知问题，本人不对因固件导致的任何问题承担任何责任
AX6的LEDE系固件（包括supes.top编译的固件)会出现内存泄露然后死机，目前已经放弃
* (更新)因为内存导致的luci卡死问题改用Immortalwrt后不再发生
* (再次更新)若要开160Mhz请在网络-无线项目找到Generic 802.11acaxn，点击编辑，将信道设置成48(亲测可用，也可以尝试其它信道)，然后在高级设置下把国家设置为US - United States，保存并应用设置，等待一分钟左右即可


## 感谢

* [Microsoft Azure](https://azure.microsoft.com/)
* [GitHub Actions](https://github.com/features/actions)
* [OpenWRT](https://github.com/openwrt/openwrt)
* [ImmortalWrt](https://github.com/immortalwrt/immortalwrt)
* [tmate](https://github.com/tmate-io/tmate)
* [P3TERX](https://github.com/P3TERX)
* [smith97](https://www.right.com.cn/forum/thread-6054985-1-1.html)
* [robimarko/openwrt](https://github.com/robimarko/openwrt/tree/ipq807x-5.15)<br>
* 以及所有跟OpenWRT/ImmortalWrt等相关的贡献者
