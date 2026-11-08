I build firmware for routers I own, infrastructure for LLM traffic, and market systems that fail closed.

Most of the work is the last mile: reproducible builds, installers with a rollback path,
and services that stay quiet when the data is wrong.

**Now** — BYTE 1.0.7 for the AW1000, the 9router control plane on musl, and ROTD's daily miss reports.

---

## Selected work

**Firmware**

- **[AW1000_NSS_BYTE](https://github.com/Ace1337z/AW1000_NSS_BYTE)** — NSS-offload OpenWrt for the Arcadyan AW1000. Kernel 6.18.60, working RJ11 telephony, one sysupgrade image. Ships as BYTE 1.0.7.
- **[RT-AX52_BYTE](https://github.com/Ace1337z/RT-AX52_BYTE)** — ImmortalWrt 25.12 for the ASUS RT-AX52. PassWall2 and Xray baked in, built by CI on every push.
- **[AW1000_BYTE](https://github.com/Ace1337z/AW1000_BYTE)** — retired ImmortalWrt build. The `repo` branch remains online as a signed opkg feed.

**OpenWrt tooling**

- **[luci-app-9router](https://github.com/Ace1337z/luci-app-9router)** — LuCI control plane for 9router-go. SHA256-verified static binary, procd supervision, rollback copy kept on disk.
- **[luci-app-byte](https://github.com/Ace1337z/luci-app-byte)** — Install, wire, inspect and undo the AdGuard Home + PassWall2 DNS chain from one page.
- **[openwrt-agh-passwall2](https://github.com/Ace1337z/openwrt-agh-passwall2)** — Idempotent AGH + PassWall2 installer with config validation and automatic rollback.

**Systems**

- **[Runner-of-the-Day](https://github.com/Ace1337z/Runner-of-the-Day)** — Micro-cap runner detector. Ranks before it alerts, fails closed on stale data, and writes a miss report for every runner it did not flag.
- **[LOOPR](https://github.com/Ace1337z/LOOPR)** — Ranked racket-sports match play with real ELO. Expo + Supabase, no mock mode.
- **[penny-early-warning](https://github.com/Ace1337z/penny-early-warning)** — Archived first attempt at pre-move micro-cap alerts.

---

## How I work

- Ship the rollback path with the change.
- Missing data is a failure, not a pass.
- A reproducible build beats a clever one.
- No mock mode. Fake data is worse than no data.

## Stack

`OpenWrt` `C` `Go` `Python` `TypeScript` `Shell` `Supabase` `Expo` `GitHub Actions`

## Elsewhere

[GitHub](https://github.com/Ace1337z) · [Telegram](https://t.me/bytewrt)
