<p align="center">
  <img src="assets/logo.png" alt="CtrlAltDevelop — Mobile · Backend · Beyond" width="560"/>
</p>

<h1 align="center">Mohammad Zarif</h1>

<p align="center">
  <strong>Senior Software Engineer</strong> · Flutter &amp; Python · FinTech Systems
</p>

<p align="center">
  I build production Flutter and Django systems for brokerages and exchanges —<br/>
  then extract the reusable parts into open-source packages for the Dart and Python communities.
</p>

<p align="center">
  <a href="https://ctrlaltdevelop.me"><img src="https://img.shields.io/badge/Portfolio-1F6FEB?style=for-the-badge&amp;logo=googlechrome&amp;logoColor=white" alt="Portfolio"/></a>
  <a href="#open-source"><img src="https://img.shields.io/badge/Packages-0175C2?style=for-the-badge&amp;logo=dart&amp;logoColor=white" alt="Open-source packages"/></a>
  <a href="https://pypi.org/user/CtrlAltDevelop/"><img src="https://img.shields.io/badge/PyPI-3776AB?style=for-the-badge&amp;logo=pypi&amp;logoColor=white" alt="Packages on PyPI"/></a>
  <a href="mailto:me.CtrlAltDev@proton.me"><img src="https://img.shields.io/badge/Contact-6D4AFF?style=for-the-badge&amp;logo=protonmail&amp;logoColor=white" alt="Contact"/></a>
</p>

<br/>

<table align="center">
  <tr>
    <td align="center" width="200"><strong>17 packages</strong><br/><sub>published on pub.dev &amp; PyPI</sub></td>
    <td align="center" width="200"><strong>9+ years</strong><br/><sub>brokerage &amp; exchange systems</sub></td>
    <td align="center" width="200"><strong>MIT licensed</strong><br/><sub>documented and reusable</sub></td>
  </tr>
</table>

<br/>

---

<h2 id="open-source">Open source</h2>

Two long-running projects sit at the centre of my open-source work — a charting library that covers
a whole trading product, and a Django Ninja backend starter that covers a whole service. Both come
out of shipping real trading systems, and both are maintained as products in their own right:
documented page by page, tested, versioned, and used in production.

Around them sits a focused set of smaller, single-purpose Dart and Flutter packages. Every project
is MIT licensed and available on GitHub.

<br/>

<h3 align="center">Flagship projects</h3>

### [django-ninja-starter](https://pypi.org/project/django-ninja-starter/)

**A production-oriented Django Ninja starter, as a template and a generator**

[![PyPI version](https://img.shields.io/pypi/v/django-ninja-starter?style=flat-square&logo=pypi&logoColor=white&label=PyPI&color=3776AB)](https://pypi.org/project/django-ninja-starter/)
[![Python versions](https://img.shields.io/pypi/pyversions/django-ninja-starter?style=flat-square&logo=python&logoColor=white&color=3776AB)](https://pypi.org/project/django-ninja-starter/)
[![License](https://img.shields.io/pypi/l/django-ninja-starter?style=flat-square&color=238636)](https://github.com/CtrlAltDevelop/django-ninja-starter/blob/main/LICENSE)
[![Source](https://img.shields.io/badge/source-GitHub-181717?style=flat-square&logo=github)](https://github.com/CtrlAltDevelop/django-ninja-starter)

Shipped two ways: as a **GitHub Template**, and as an installable generator
(`pipx install django-ninja-starter`). It answers what every new API project has to
answer anyway — settings per environment, auth, versioning, CI — so the first commit
already looks like a mature service.

**The foundation**

- Feature-first layout, environment-specific settings, secure production defaults
- OpenAPI docs with a version selector in the Swagger top bar, plus ReDoc per version
- Health checks, Docker-ready, CI, typing, linting, coverage and tests from day one
- Admin themed with [Unfold](https://unfoldadmin.com): a dashboard of real numbers, a
  sidebar built from the apps you installed, and an environment badge

**Authentication — included, entirely opt-in.** Each method is its own app that
installs nothing until you name it:

- **4 login methods** · **4 second factors** · **4 social providers** · **3 token modes**
- Every login path ends by minting a signed **JWT**
- Two-step state lives in Redis, hashed; endpoints deliberately reveal nothing about
  which accounts exist

**Five feature apps, off by default.** Name one in the environment and it appears —
tables, routes, admin and all. Leave it unset and the project carries none of it:

| App | What you get |
|---|---|
| `cms` | Pages of sections of typed, translatable fields; drafts, schedules, signed preview links |
| `notifications` | One surface over REST, GraphQL, gRPC and a WebSocket that keeps a second device in step |
| `support` | Live chat and tickets as one thing, plus channels, groups and direct messages |
| `shop` | Catalogue, variants and stock, campaigns, basket, orders, coupons and payments |
| `wallet` | Balances derived from movements; deposits, transfers, crypto, conversion, approvals |

**Scaffolding built in**

```bash
python manage.py startapi users --api-version v1
```

Creates the app module and a matching endpoint test, registers the router, and exposes
`GET /api/v1/users/` — visible immediately in the v1 OpenAPI schema.

<sub>Python 3.12+ · Django 5.2 and 6.x · one documentation page per app</sub>

<br/>

### [ohlcv_chart](https://pub.dev/packages/ohlcv_chart)

**The trading screen and the reporting charts around it, in one dependency**

[![pub.dev version](https://img.shields.io/pub/v/ohlcv_chart?style=flat-square&logo=dart&logoColor=white&label=pub.dev&color=0175C2)](https://pub.dev/packages/ohlcv_chart)
[![pub points](https://img.shields.io/pub/points/ohlcv_chart?style=flat-square&logo=dart&logoColor=white&color=0175C2)](https://pub.dev/packages/ohlcv_chart/score)
[![License](https://img.shields.io/github/license/CtrlAltDevelop/ohlcv_chart?style=flat-square&color=238636)](https://github.com/CtrlAltDevelop/ohlcv_chart/blob/main/LICENSE)
[![Source](https://img.shields.io/badge/source-GitHub-181717?style=flat-square&logo=github)](https://github.com/CtrlAltDevelop/ohlcv_chart)

A candlestick chart with **31 indicators** and **29 drawing tools**, and **39 other
chart widgets** beside it — the order book and the tape, the charts a backtest report
is built from, and the ones a dashboard is. Everything is rendered with
`CustomPainter`: no WebView, no JavaScript bridge, no charting library underneath.
Every feature is free, including commercially; there is no paid tier.

<a href="https://github.com/CtrlAltDevelop/ohlcv_chart#gallery"><img src="https://raw.githubusercontent.com/CtrlAltDevelop/ohlcv_chart/main/screenshots/chart-types.png" width="100%" alt="Eight chart types rendered by ohlcv_chart"/></a>

**The candlestick chart**

- **8 chart types**, plus Heikin-Ashi, Renko, line break, Kagi, point & figure and
  range bars as transforms of the source candles
- **31 indicators**, each a configured instance — `ATR(8)` and `ATR(14)` run side by
  side — with higher-timeframe values that never repaint
- **29 drawing tools** with a line editor, multi-select, undo/redo, keyboard
  shortcuts, JSON persistence and price alerts
- Bar replay, linked charts, an overview strip, order and position lines, session
  dividers and a live price line

**The other 39 charts**

- **Order flow** — market profile, footprint, order-book heatmap, cumulative delta,
  liquidity map, open interest and funding
- **Backtests** — equity curve with drawdown, Monte Carlo fan, R-multiple
  distribution, trade timeline, seasonality, calendar P&L
- **Dashboards** — treemap, sunburst, sankey, chord, marimekko, stream, parallel
  coordinates, box plot, violin, bullet, gauge, waffle, funnel and more
- **Derivatives** — options payoff with break-evens, volatility smiles and term
  structures, pair spreads with z-score

<sub>Dart 3.12+ · Flutter 3.44+ · themeable end to end · one documentation page per feature</sub>

<br/>

<h3 align="center">Supporting packages</h3>

<p align="center"><sub>Small, single-purpose packages extracted from production Flutter work — each one solving one problem completely.</sub></p>

<br/>

**Architecture** — <sub>explicit error flow and predictable state, with zero code generation</sub>

| Package | What it does | Link |
|---|---|---|
| [`verdict`](https://pub.dev/packages/verdict) | A sealed `Result` type and structured `Failure` hierarchy, so calls return a typed verdict instead of throwing across layer boundaries | [pub.dev ↗](https://pub.dev/packages/verdict) |
| [`verdict_bloc`](https://pub.dev/packages/verdict_bloc) | BLoC states that keep the last known good data through loading and error, plus a paginated list bloc built on `verdict` | [pub.dev ↗](https://pub.dev/packages/verdict_bloc) |
| [`safe_json_cast`](https://pub.dev/packages/safe_json_cast) | Typed casts for decoded JSON that fail loudly and name the field, so a malformed payload surfaces at the parse site rather than deep in the UI | [pub.dev ↗](https://pub.dev/packages/safe_json_cast) |

**UI components** — <sub>themeable widgets with motion that feels native</sub>

| Package | What it does | Link |
|---|---|---|
| [`anchored_popover`](https://pub.dev/packages/anchored_popover) | A popover that anchors to a widget instead of the screen — it follows its anchor as the list scrolls, flips and clamps to stay on screen, then fades itself back out | [pub.dev ↗](https://pub.dev/packages/anchored_popover) |
| [`capsule_nav_bar`](https://pub.dev/packages/capsule_nav_bar) | A bottom navigation bar that floats over the content as a rounded capsule, its selection marked by a pill sliding between destinations | [pub.dev ↗](https://pub.dev/packages/capsule_nav_bar) |
| [`sliding_segmented_control`](https://pub.dev/packages/sliding_segmented_control) | A themeable segmented control with a pill sliding between segments and an optional body that cross-fades underneath it | [pub.dev ↗](https://pub.dev/packages/sliding_segmented_control) |
| [`indicator_tab_bar`](https://pub.dev/packages/indicator_tab_bar) | A fixed-width indicator that underlines the label rather than the tab, plus a sliver `AnimatedSwitcher` for cross-fading each tab's body | [pub.dev ↗](https://pub.dev/packages/indicator_tab_bar) |
| [`diamond_percent_slider`](https://pub.dev/packages/diamond_percent_slider) | An integer slider on a scale of diamonds, with a thumb that leans the way it is dragged and a bubble showing the value while it moves | [pub.dev ↗](https://pub.dev/packages/diamond_percent_slider) |
| [`ruler_scrubber`](https://pub.dev/packages/ruler_scrubber) | An accessible ruler-style numeric scrubber for picking a value by sliding a measured scale | [pub.dev ↗](https://pub.dev/packages/ruler_scrubber) |

**Notifications** — <sub>two takes on overlay toasts, for different needs</sub>

| Package | What it does | Link |
|---|---|---|
| [`toast_overlay`](https://pub.dev/packages/toast_overlay) | An animated, themeable overlay toast with an auto-dismiss countdown ring and an optional copyable support reference id | [pub.dev ↗](https://pub.dev/packages/toast_overlay) |
| [`queued_toast`](https://pub.dev/packages/queued_toast) | Overlay toasts that queue per screen position, de-duplicate identical messages, and stack up to five at a time | [pub.dev ↗](https://pub.dev/packages/queued_toast) |

**Networking &amp; security** — <sub>the transport and auth layers behind a live exchange app</sub>

| Package | What it does | Link |
|---|---|---|
| [`dpop_client`](https://pub.dev/packages/dpop_client) | DPoP proof JWTs for Dart (**RFC 9449**) — ES256 key handling, PEM storage, JWK thumbprints, access-token binding, and server-supplied nonces | [pub.dev ↗](https://pub.dev/packages/dpop_client) |
| [`socket_hub`](https://pub.dev/packages/socket_hub) | One WebSocket, many channels — ref-counted subscriptions derived from stream listeners, batched frames, typed payload routing, and resubscribe on reconnect | [pub.dev ↗](https://pub.dev/packages/socket_hub) |

**Tooling** — <sub>codegen and design-system chores, automated</sub>

| Package | What it does | Link |
|---|---|---|
| [`openapi_enum_patch`](https://pub.dev/packages/openapi_enum_patch) | Prepares an OpenAPI export for codegen: names the integer enums `swagger_parser` produces, generates the enum files it skips, and audits the ones still unnamed | [pub.dev ↗](https://pub.dev/packages/openapi_enum_patch) |
| [`figma_tokens_gen`](https://pub.dev/packages/figma_tokens_gen) | Generates Flutter `Color` constants and palette maps from Figma design-token JSON exports — ships a CLI and a customisable library API | [pub.dev ↗](https://pub.dev/packages/figma_tokens_gen) |

<br/>

---

## Professional work

I am **Senior Flutter Engineer at DeltaFX**, working on a cross-platform brokerage CRM covering
wallets, trading accounts, introducing-broker and affiliate management, social trading, and
AI-assisted market analysis.

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>DeltaFX CRM</h3>
      <sub>Forex brokerage client portal · iOS &amp; Android</sub>
      <br/><br/>
      A modular Flutter application built on Clean Architecture and BLoC, with one module per
      feature, generated type-safe API clients, resilient authentication, and explicit error
      boundaries at every layer seam.
      <br/><br/>
      <sub>Wallets · Trading accounts · IB &amp; affiliate management · Social trading · KYC</sub>
    </td>
    <td width="50%" valign="top">
      <h3>BTCB <a href="https://play.google.com/store/apps/details?id=com.btcb.app"><img src="https://img.shields.io/badge/Google_Play-414141?style=flat-square&amp;logo=googleplay&amp;logoColor=white" alt="Google Play"/></a></h3>
      <sub>Cryptocurrency exchange · Futures, Spot &amp; OTC</sub>
      <br/><br/>
      An exchange client with real-time market data, advanced charting, passkey sign-in and DPoP
      request signing, and full multi-language localization — built on the same modular
      architecture.
      <br/><br/>
      <sub>Futures · Spot · OTC · Order book · Streaming charts · Passkeys</sub>
    </td>
  </tr>
</table>

<br/>

---

## Core technologies

<table>
  <tr>
    <td width="120"><strong>Mobile</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white" alt="Flutter"/>
      <img src="https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=dart&logoColor=white" alt="Dart"/>
      <img src="https://img.shields.io/badge/BLoC-1B6AC6?style=flat-square" alt="BLoC"/>
      <img src="https://img.shields.io/badge/Clean_Architecture-3D5A80?style=flat-square" alt="Clean Architecture"/>
      <img src="https://img.shields.io/badge/CustomPainter-0468D7?style=flat-square" alt="CustomPainter"/>
    </td>
  </tr>
  <tr>
    <td><strong>Backend</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python"/>
      <img src="https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white" alt="Django"/>
      <img src="https://img.shields.io/badge/Django_Ninja-4B8BBE?style=flat-square" alt="Django Ninja"/>
      <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI"/>
      <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
    </td>
  </tr>
  <tr>
    <td><strong>Trading</strong></td>
    <td>
      <img src="https://img.shields.io/badge/MQL_4%2F5-1F6FEB?style=flat-square" alt="MQL 4 and 5"/>
      <img src="https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=csharp&logoColor=white" alt="C sharp"/>
      <img src="https://img.shields.io/badge/Backtesting-8957E5?style=flat-square" alt="Backtesting"/>
      <img src="https://img.shields.io/badge/Algorithmic_Trading-238636?style=flat-square" alt="Algorithmic Trading"/>
    </td>
  </tr>
  <tr>
    <td><strong>Delivery</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker"/>
      <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions"/>
      <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git"/>
    </td>
  </tr>
</table>

<br/>

---

## Research

Author of five peer-reviewed papers on neural networks and biomedical signal analysis, published
before moving into financial software full time. The same habits carry over: measure first,
model explicitly, and document the method well enough that someone else can reproduce it.

<br/>

---

<p align="center">
  <strong>Engineering financial products across mobile, backend, and automation</strong>
  <br/>
  <sub>9+ years across brokerage, exchange, and trading-automation systems in Iran, the UAE, Germany, and Turkey.</sub>
</p>

<p align="center">
  <a href="https://ctrlaltdevelop.me">Portfolio</a> ·
  <a href="https://github.com/CtrlAltDevelop">GitHub</a> ·
  <a href="https://pypi.org/user/CtrlAltDevelop/">PyPI</a> ·
  <a href="mailto:me.CtrlAltDev@proton.me">Contact</a>
</p>
