# xian

Quantumult X 规则与重写片段。所有文件链接均为国内镜像（gh-proxy），直接点开即用。

## 文件链接

| 文件 | 说明 | 镜像链接 |
|---|---|---|
| Block-Apple-Asset.qx.list | 冻结证书信任资产：拦截 Apple OTA PKI / MobileAsset 资产域名 | https://gh-proxy.com/https://raw.githubusercontent.com/xian9158/xian/main/Block-Apple-Asset.qx.list |
| Block-Apple-Asset.qx.conf | 冻结证书信任资产完整配置：17 条放行 + 8 条拦截 + 远程引用 | https://gh-proxy.com/https://raw.githubusercontent.com/xian9158/xian/main/Block-Apple-Asset.qx.conf |
| Chrome.list | Google Chrome 浏览器内置服务、同步及搜索分流规则 | https://gh-proxy.com/https://raw.githubusercontent.com/xian9158/xian/main/Chrome.list |
| Douyin-Proxy.list | 抖音走代理分流规则 | https://gh-proxy.com/https://raw.githubusercontent.com/xian9158/xian/main/Douyin-Proxy.list |
| Huya-AdBlock.list | 虎牙直播去广告过滤规则 | https://gh-proxy.com/https://raw.githubusercontent.com/xian9158/xian/main/Huya-AdBlock.list |
| Huya-AdBlock.snippet | 虎牙直播去广告重写片段 | https://gh-proxy.com/https://raw.githubusercontent.com/xian9158/xian/main/Huya-AdBlock.snippet |
| Waimai-AdBlock.list | 歪麦霸王餐去开屏广告过滤规则 | https://gh-proxy.com/https://raw.githubusercontent.com/xian9158/xian/main/Waimai-AdBlock.list |
| XiaoCan-AdBlock.snippet | 小蚕霸王餐去广告重写片段 | https://gh-proxy.com/https://raw.githubusercontent.com/xian9158/xian/main/XiaoCan-AdBlock.snippet |

## QX 订阅用法

在 Quantumult X 配置的 `[filter_remote]` 里加一行（以冻结证书信任资产为例）：

```
https://gh-proxy.com/https://raw.githubusercontent.com/xian9158/xian/main/Block-Apple-Asset.qx.list, tag=冻结证书信任资产, update-interval=86400, opt-parser=false, enabled=true
```

`.snippet` 文件在 QX「重写 - 引用」里添加对应镜像链接即可。
