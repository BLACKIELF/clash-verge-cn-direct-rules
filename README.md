# Clash Verge CN Direct Rules

Made by **blackielovelife**.

[中文说明](README.zh-CN.md)

This is a privacy-safe Clash Verge / Mihomo merge template for common mainland China websites that should usually go `DIRECT`.

It was created after debugging intermittent first-load failures on Xiaohongshu and Bilibili, where pages sometimes failed once and worked after refresh. The goal is to cover common login, API, CDN, image, video, and redirect domains for daily-use Chinese websites.

## What It Covers

- Xiaohongshu / Rednote
- Bilibili
- Weibo
- Xinpianchang
- Baidu
- Zhihu
- Douyin
- Common China direct rules from Loyalsoldier
- LAN and China IP direct fallback

## Privacy Notice

This repository does **not** include:

- proxy nodes
- subscription URLs
- UUIDs
- passwords
- tokens
- proxy group names from a personal profile
- full generated Clash Verge runtime config

Only public rule providers and domain rules are included.

## How To Use In Clash Verge

1. Open Clash Verge.
2. Go to `Profiles`.
3. Open `Merge` / `Profile Enhancement`.
4. Paste the content of `clash-verge-merge-template.yaml`.
5. Save.
6. Restart Clash Verge or reload the profile.

## Files

- `clash-verge-merge-template.yaml`: full Clash Verge profile enhancement merge template.
- `rules/cn-stable-direct-patch.yaml`: only the extra direct rules, for people who already have their own template.

## Notes

This ruleset is intentionally conservative: it only forces direct routing for domains that are strongly associated with mainland China services. If a service still fails on first load, clear browser DNS/socket cache or restart Clash Verge after applying the rules.
