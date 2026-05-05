# CN Tracker DNS Filter

---

## Overview

CN Tracker DNS Filter is a DNS-level blocklist designed to target Chinese tracking, advertising, and telemetry domains used by major platforms such as Alibaba, Tencent, Baidu, and ByteDance.

It is intended as a supplementary filter, not a replacement for general-purpose adblocking lists.

---

## Purpose

This filter aims to:

- Block Chinese ad and tracking infrastructure
- Reduce telemetry from embedded SDKs
- Mitigate redirect-based tracking
- Enhance privacy beyond default DNS filters

---

## Scope

### Included

- Alibaba ecosystem (e.g., "mmstat", "tanx", "alimama")
- Tencent ecosystem (e.g., "gdt", "beacon", "qq analytics")
- Baidu analytics and ad systems
- ByteDance tracking endpoints
- Chinese mobile SDK trackers (e.g., Umeng, TalkingData)

### Excluded

- Global ad networks (covered by standard filters)
- Cosmetic filtering (not applicable at DNS level)
- General website-specific rules

---

## Usage

Add to AdGuard / DNS Filtering

### [Copy this link](https://raw.githubusercontent.com/mchany/CN-Tracker-DNS-Filter/refs/heads/main/CN%20Tracker%20DNS%20Filter.txt)

---

## Known Issues

Blocking certain domains may cause partial breakage:

- "qq.com" / "tencent.com" → login or content issues
- "bdstatic.com" → missing resources
- redirect domains → links may not resolve properly

Users may need to whitelist specific domains depending on usage.

---

## Disclaimer

This filter targets specific regional tracking infrastructure.
It may affect functionality of certain services.

Use at your own discretion and adjust with custom allow rules if necessary.
