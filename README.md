# assemblecam-legal

AssembleCam / 汇摄影 App Store legal + marketing pages — hosted on Cloudflare Pages at `https://assemblecam.lx06.com`.

Modeled after [pick10-legal](https://github.com/lixiao90s/pick10-legal).

## Pages

| File | URL | App Store 用途 |
|------|-----|----------------|
| `index.html` | `/` | 官网首页 / Marketing URL |
| `support.html` | `/support` | **Support URL** |
| `privacy.html` | `/privacy` | **Privacy Policy URL** |
| `terms.html` | `/terms` 或 `/terms.html` | 用户协议 / 自定义 EULA |
| `legal.html` | `/legal.html` | 法律文档索引 |
| `app-ads.txt` | `/app-ads.txt` | AdMob 验证 |

## App Store Connect 填写

| 字段 | URL |
|------|-----|
| Privacy Policy URL | `https://assemblecam.lx06.com/privacy` |
| Support URL | `https://assemblecam.lx06.com/support` |
| Marketing URL | `https://assemblecam.lx06.com/` |

Support email (in-app / ASC): `lixiao918918@gmail.com`  
Bundle ID: `com.lixiao.app.cameratool`

## Deploy — GitHub + Cloudflare Pages

1. Push this repo to GitHub (`lixiao90s/assemblecam-legal`)
2. Cloudflare Dashboard → Workers & Pages → Create → Pages → Connect to Git
3. Select `assemblecam-legal`
4. Build settings: Framework preset **None**, Build command empty, Output directory `/`
5. Custom domains → `assemblecam.lx06.com`

## Local preview

```bash
cd assemblecam-legal
python -m http.server 8080
# open http://localhost:8080
```
