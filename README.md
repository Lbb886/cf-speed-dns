## cf-speed-dns是什么?
CloudflareSpeedTest 推送「每5分钟自选优选 IP」获取Cloudflare CDN 延迟和速度最快 IP ！

## cf-speed-dns有哪些功能？
* CloudflareSpeedTest优选IP，实时更新列表页面。[https://ip.164746.xyz](https://ip.164746.xyz)
* CloudflareSpeedTest优选IP，Top接口(默认)[https://ip.164746.xyz/ipTop.html](https://ip.164746.xyz/ipTop.html)；Top10接口[https://ip.164746.xyz/ipTop10.html](https://ip.164746.xyz/ipTop10.html)。
* DNSPOD实时域名解析推送，fork 本项目。
  * Action配置，Actions secrets and variables 添加 DOMAIN(例如：164746.xyz)，SUB_DOMAIN（例如：dns），SECRETID（xxxxx），SECRETKEY（xxxxx），WECHAT_WEBHOOK（xxxxx）。
* DNSCF实时域名解析推送，fork 本项目。
  * Action配置，Actions secrets and variables 添加 CF_API_TOKEN(例如：xxxxx)，CF_ZONE_ID（例如：xxxxx），CF_DNS_NAME（dns.164746.xyz），WECHAT_WEBHOOK（xxxxx）。
* ~~接入PUSHPLUS消息通知。[https://www.pushplus.plus/push1.html](https://www.pushplus.plus/push1.html)~~ （改企业微信机器人消息通知）

## 基于原项目[cf-speed-dns](https://github.com/ZhiXuanWang/cf-speed-dns)修改
* 改企业微信机器人推送（DNSCF）  2024-11-24 （DNSPOD） 2024-11-27
* 添加手动执行dns_cf_push工作流 2024-11-24  dns_pod_push  2024-11-27
* 优化dnscf.py代码 2024-11-25
* 接口改成自建接口，代码适配 2024-11-29

## 接口请求
```javascript
curl 'https://ip.164746.xyz/ipTop.html'
```
## 接口返回
```javascript
104.16.204.6,104.18.103.125
```

## 感谢
[XIU2](https://github.com/XIU2/CloudflareSpeedTest)、[ddgth](https://github.com/ddgth/cf2dns)
