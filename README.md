<div align="center">

# ACE1337z

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=2800&pause=900&color=00B5E2&center=true&vCenter=true&width=720&lines=firmware+wrangler+%C2%B7+LLM+plumbing+%C2%B7+trading+systems;flashing+OpenWrt+on+hardware+I+actually+own;routing+LLM+traffic+through+a+42+MB+Go+gateway;hunting+micro-cap+runners+before+the+crowd" alt="ACE1337z" />

I build firmware for routers I own, plumbing for free LLM tiers, and trading
automation I try not to leave unattended.

[![OpenWrt](https://img.shields.io/badge/OpenWrt-00B5E2?style=flat-square&logo=openwrt&logoColor=white)](https://openwrt.org)
[![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)](https://github.com/Ace1337z/AW1000_NSS_BYTE)
[![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)](https://github.com/Ace1337z/luci-app-9router)
[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://github.com/Ace1337z/Runner-of-the-Day)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://github.com/Ace1337z/LOOPR)
[![Shell](https://img.shields.io/badge/Shell-4EAA25?style=flat-square&logo=gnubash&logoColor=white)](https://github.com/Ace1337z/openwrt-agh-passwall2)

<a href="https://github.com/Ace1337z?tab=repositories"><img src="https://img.shields.io/badge/repos-10-0d1117?style=flat-square&logo=github&logoColor=white" alt="repos"></a>
<a href="https://t.me/bytewrt"><img src="https://img.shields.io/badge/Telegram-@bytewrt-26A5E4?style=flat-square&logo=telegram&logoColor=white" alt="Telegram"></a>

</div>

---

### Currently shipping

<table>
<tr>
<td width="50%" valign="top">

#### [AW1000_NSS_BYTE](https://github.com/Ace1337z/AW1000_NSS_BYTE)

<sub><code>OpenWrt</code> · <code>C</code> · <code>IPQ807x</code></sub>

**BYTE 1.0.7.** Custom firmware for the Arcadyan AW1000 on the `ppe-nss`
tree. NSS Wi-Fi offload, kernel 6.18.60, working RJ11 phone, PassWall2 and
9Router baked in. One sysupgrade image, reproducible from CI.

[![release](https://img.shields.io/github/v/release/Ace1337z/AW1000_NSS_BYTE?style=flat-square&label=release&color=00B5E2)](https://github.com/Ace1337z/AW1000_NSS_BYTE/releases)
[![last commit](https://img.shields.io/github/last-commit/Ace1337z/AW1000_NSS_BYTE?style=flat-square&label=last%20commit&color=5a6472)](https://github.com/Ace1337z/AW1000_NSS_BYTE/commits/main)

</td>
<td width="50%" valign="top">

#### [luci-app-9router](https://github.com/Ace1337z/luci-app-9router)

<sub><code>OpenWrt</code> · <code>Shell</code> · <code>Go</code></sub>

LuCI control plane for **9router-go**. Downloads the CGO-free static gateway,
verifies it against `SHA256SUMS.txt`, supervises it under procd, and keeps a
rollback copy. Built for musl, not glibc.

[![last commit](https://img.shields.io/github/last-commit/Ace1337z/luci-app-9router?style=flat-square&label=last%20commit&color=5a6472)](https://github.com/Ace1337z/luci-app-9router/commits/main)
[![packages](https://img.shields.io/badge/apk%20%2B%20ipk-ready-00B5E2?style=flat-square)](https://github.com/Ace1337z/luci-app-9router)

</td>
</tr>
<tr>
<td width="50%" valign="top">

#### [luci-app-byte](https://github.com/Ace1337z/luci-app-byte)

<sub><code>OpenWrt</code> · <code>Shell</code> · <code>LuCI</code></sub>

One page that installs, wires, inspects and **undoes** the AdGuard Home +
PassWall2 DNS chain. Feed-managed packages, vendored installer pin, IPv4-only
listeners by design.

[![last commit](https://img.shields.io/github/last-commit/Ace1337z/luci-app-byte?style=flat-square&label=last%20commit&color=5a6472)](https://github.com/Ace1337z/luci-app-byte/commits/main)
[![packages](https://img.shields.io/badge/apk%20%2B%20ipk-ready-00B5E2?style=flat-square)](https://github.com/Ace1337z/luci-app-byte)

</td>
<td width="50%" valign="top">

#### [openwrt-agh-passwall2](https://github.com/Ace1337z/openwrt-agh-passwall2)

<sub><code>OpenWrt</code> · <code>Shell</code></sub>

Conflict-free AdGuardHome + PassWall2 installer. Backs up every touched file,
validates the YAML before dnsmasq gives up port 53, auto-rolls back if AGH stops
answering, and reruns idempotently.

[![last commit](https://img.shields.io/github/last-commit/Ace1337z/openwrt-agh-passwall2?style=flat-square&label=last%20commit&color=5a6472)](https://github.com/Ace1337z/openwrt-agh-passwall2/commits/main)

</td>
</tr>
<tr>
<td width="50%" valign="top">

#### [RT-AX52_BYTE](https://github.com/Ace1337z/RT-AX52_BYTE)

<sub><code>OpenWrt</code> · <code>Shell</code> · <code>MT7981B</code></sub>

**ImmortalWrt 25.12** for the ASUS RT-AX52. PassWall2 and Xray baked in,
Footstrap UI, tuned for 256 MB RAM. Push, let Actions build, download the
release.

[![release](https://img.shields.io/github/v/release/Ace1337z/RT-AX52_BYTE?style=flat-square&label=release&color=00B5E2)](https://github.com/Ace1337z/RT-AX52_BYTE/releases)
[![last commit](https://img.shields.io/github/last-commit/Ace1337z/RT-AX52_BYTE?style=flat-square&label=last%20commit&color=5a6472)](https://github.com/Ace1337z/RT-AX52_BYTE/commits/main)

</td>
<td width="50%" valign="top">

#### [Runner-of-the-Day](https://github.com/Ace1337z/Runner-of-the-Day)

<sub><code>Python</code> · <code>Telegram</code> · <code>Finviz</code></sub>

Stricter successor to penny-early-warning. Ranks US micro-caps for the day's
explosive move, fails closed on stale or conflicting data, and writes a MISS
REPORT explaining every runner it did not flag. Decision support only.

[![last commit](https://img.shields.io/github/last-commit/Ace1337z/Runner-of-the-Day?style=flat-square&label=last%20commit&color=5a6472)](https://github.com/Ace1337z/Runner-of-the-Day/commits/main)

</td>
</tr>
</table>

### Also in the shop

- **[LOOPR](https://github.com/Ace1337z/LOOPR)** — ranked match play for racket sports. Expo + Supabase, real ELO, no mock mode.
- **[AW1000_BYTE](https://github.com/Ace1337z/AW1000_BYTE)** — retired ImmortalWrt 25.12 build. The `repo` branch lives on as the signed opkg feed.
- **[penny-early-warning](https://github.com/Ace1337z/penny-early-warning)** — archived first pass at pre-move micro-cap alerts.

### How I build

```text
fail closed        missing data is never a pass
reproducible       pinned trees, CI builds, signed feeds
undo included      every installer ships a rollback path
no mock mode       fake data is worse than no data
```

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=Ace1337z&show_icons=true&hide_border=true&bg_color=00000000&title_color=00B5E2&icon_color=00B5E2&text_color=8b949e&include_all_commits=true&rank_icon=github" alt="GitHub stats" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Ace1337z&layout=compact&hide_border=true&bg_color=00000000&title_color=00B5E2&text_color=8b949e&langs_count=8" alt="Top languages" />

<br>

<sub>Rank 1337, by choice.</sub>

</div>
