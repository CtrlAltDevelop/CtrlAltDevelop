<p align="center">
  <img src="assets/logo.png" alt="CtrlAltDevelop — Mobile · Backend · Beyond" width="560"/>
</p>

<h1 align="center">Mohammad Zarif</h1>

<p align="center">
  <strong>Senior Software Engineer</strong> · Flutter &amp; Python · FinTech Systems
</p>

<p align="center">
  I build production-grade Flutter and Django systems for brokerages and exchanges —<br/>
  then extract the reusable parts into open-source packages for the Dart and Python communities.
</p>

<p align="center">
  <a href="https://ctrlaltdevelop.github.io"><img src="https://img.shields.io/badge/View_Portfolio-1F6FEB?style=for-the-badge&amp;logo=googlechrome&amp;logoColor=white" alt="View portfolio"/></a>
  <a href="#-open-source"><img src="https://img.shields.io/badge/Open_Source-181717?style=for-the-badge&amp;logo=github&amp;logoColor=white" alt="Explore open-source projects"/></a>
  <a href="mailto:me.CtrlAltDev@proton.me"><img src="https://img.shields.io/badge/Contact_Me-6D4AFF?style=for-the-badge&amp;logo=protonmail&amp;logoColor=white" alt="Contact me"/></a>
</p>

<br/>

<table align="center">
  <tr>
    <td align="center" width="180"><strong>17 packages</strong><br/><sub>published on pub.dev &amp; PyPI</sub></td>
    <td align="center" width="180"><strong>160 / 160</strong><br/><sub>pub points on every package</sub></td>
    <td align="center" width="180"><strong>9+ years</strong><br/><sub>in brokerage &amp; exchange systems</sub></td>
    <td align="center" width="180"><strong>MIT licensed</strong><br/><sub>open, documented, reusable</sub></td>
  </tr>
</table>

<br/>

---

<h2 id="-open-source">🧩 Open source</h2>

Two large, long-running projects sit at the centre of my open-source work — a complete financial
charting engine for Flutter, and a production-oriented Django Ninja backend starter. Both are the
distilled result of shipping real trading products, and both are maintained as full products in
their own right: documented, tested, versioned, and used in production.

Around them sits a focused set of smaller, single-purpose Dart and Flutter packages. Every project
is MIT licensed and available on GitHub.

<br/>

<h3 align="center">⭐ Flagship projects</h3>

<table>
<tr>
<td width="50%" valign="top">

### 🐍 [django-ninja-starter](https://pypi.org/project/django-ninja-starter/)

**A production-oriented Django Ninja API template and project generator**

[![PyPI](https://img.shields.io/badge/view_on-PyPI-3776AB?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/django-ninja-starter/)
[![Source](https://img.shields.io/badge/source-GitHub-181717?style=flat-square&logo=github)](https://github.com/CtrlAltDevelop/django-ninja-starter)
[![Python](https://img.shields.io/badge/Python-3.12+-3776AB?style=flat-square&logo=python&logoColor=white)](https://pypi.org/project/django-ninja-starter/)
[![Django](https://img.shields.io/badge/Django-5.2%20%7C%206.x-092E20?style=flat-square&logo=django&logoColor=white)](https://pypi.org/project/django-ninja-starter/)

A complete backend foundation, shipped two ways: as a **GitHub Template** and as an
**installable project generator** (`pipx install django-ninja-starter`). It answers the
questions every new API project has to answer anyway — settings per environment, auth,
versioning, CI — so the first commit already looks like a mature service.

**What's in the box**

- **Structure** — feature-first source layout, one app per capability
- **Config** — environment-specific settings with secure production defaults
- **API** — OpenAPI docs with a version selector in the Swagger top bar
- **Ops** — health checks, Docker-ready, CI pipeline included
- **Quality** — typing, linting, coverage and tests wired from day one

**Authentication — included, and entirely opt-in.** Each method is its own app that installs
nothing until you name it:

- **4 login methods** · **4 second factors** · **4 social providers** · **3 token modes**
- Every login path ends by minting a signed **JWT**
- One documentation page per app: routes, models, admin, setup, usage

**Scaffolding built in**

```bash
python manage.py startapi users --api-version v1
```

Creates the app module and a matching endpoint test, registers the router, and exposes
`GET /api/v1/users/` — visible immediately in the v1 OpenAPI schema and the Swagger version
selector.

</td>
<td width="50%" valign="top">

### 📈 [ohlcv_chart](https://pub.dev/packages/ohlcv_chart)

**The most complete candlestick charting engine for Flutter**

[![pub.dev](https://img.shields.io/badge/view_on-pub.dev-0175C2?style=flat-square&logo=dart&logoColor=white)](https://pub.dev/packages/ohlcv_chart)
[![Source](https://img.shields.io/badge/source-GitHub-181717?style=flat-square&logo=github)](https://github.com/CtrlAltDevelop/ohlcv_chart)
[![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)](https://pub.dev/packages/ohlcv_chart)

Rendered entirely with `CustomPainter` — **no charting library underneath**, no platform views,
no WebView. Built for real trading screens: smooth pan and zoom across large candle sets,
crosshair inspection, and live streaming updates without dropping frames. It powers the
charting in a production cryptocurrency exchange.

**What it draws**

- **8 chart types** — candlestick, OHLC bars, line, area and more
- **31 indicators** — MA, EMA, BOLL, MACD, RSI, KDJ, and beyond
- **29 drawing tools** — trendlines, channels, Fibonacci, shapes, annotations
- **Sub-charts** — stacked MACD / RSI / KDJ panes with a shared crosshair
- **Market depth** — a dedicated order-book depth chart
- **Alerts** — draggable price alerts drawn on the axis
- **Bar replay** — step back through history to rehearse a strategy

**Built for production**

- Themeable end to end — colours, typography, grid, and axis formatting
- Streaming-friendly: append or patch the latest candle without a full rebuild
- Gesture model tuned for touch and mouse, including scroll-wheel zoom
- Fully documented with a runnable example app

</td>
</tr>
</table>

<br/>

<h3 align="center">📦 Supporting packages</h3>

<p align="center"><sub>Small, single-purpose packages extracted from production Flutter work — each one solving one problem completely.</sub></p>

<br/>

**🏛️ Architecture** — <sub>explicit error flow and predictable state, with zero code generation</sub>

| Package | What it does | Link |
|---|---|---|
| [`verdict`](https://pub.dev/packages/verdict) | A sealed `Result` type and structured `Failure` hierarchy, so calls return a typed verdict instead of throwing across layer boundaries | [pub.dev ↗](https://pub.dev/packages/verdict) |
| [`verdict_bloc`](https://pub.dev/packages/verdict_bloc) | BLoC states that keep the last known good data through loading and error, plus a paginated list bloc built on `verdict` | [pub.dev ↗](https://pub.dev/packages/verdict_bloc) |
| [`safe_json_cast`](https://pub.dev/packages/safe_json_cast) | Typed casts for decoded JSON that fail loudly and name the field, so a malformed payload surfaces at the parse site rather than deep in the UI | [pub.dev ↗](https://pub.dev/packages/safe_json_cast) |

**🎨 UI components** — <sub>polished, themeable widgets with motion that feels native</sub>

| Package | What it does | Link |
|---|---|---|
| [`anchored_popover`](https://pub.dev/packages/anchored_popover) | A popover that anchors to a widget instead of the screen — it follows its anchor as the list scrolls, flips and clamps to stay on screen, then fades itself back out | [pub.dev ↗](https://pub.dev/packages/anchored_popover) |
| [`capsule_nav_bar`](https://pub.dev/packages/capsule_nav_bar) | A bottom navigation bar that floats over the content as a rounded capsule, its selection marked by a pill sliding between destinations | [pub.dev ↗](https://pub.dev/packages/capsule_nav_bar) |
| [`sliding_segmented_control`](https://pub.dev/packages/sliding_segmented_control) | A themeable segmented control with a pill sliding between segments and an optional body that cross-fades underneath it | [pub.dev ↗](https://pub.dev/packages/sliding_segmented_control) |
| [`indicator_tab_bar`](https://pub.dev/packages/indicator_tab_bar) | A fixed-width indicator that underlines the label rather than the tab, plus a sliver `AnimatedSwitcher` for cross-fading each tab's body | [pub.dev ↗](https://pub.dev/packages/indicator_tab_bar) |
| [`diamond_percent_slider`](https://pub.dev/packages/diamond_percent_slider) | An integer slider on a scale of diamonds, with a thumb that leans the way it is dragged and a bubble showing the value while it moves | [pub.dev ↗](https://pub.dev/packages/diamond_percent_slider) |
| [`ruler_scrubber`](https://pub.dev/packages/ruler_scrubber) | A performant, accessible ruler-style numeric scrubber for picking a value by sliding a measured scale | [pub.dev ↗](https://pub.dev/packages/ruler_scrubber) |

**🔔 Notifications** — <sub>two takes on overlay toasts, for different needs</sub>

| Package | What it does | Link |
|---|---|---|
| [`toast_overlay`](https://pub.dev/packages/toast_overlay) | An animated, themeable overlay toast with an auto-dismiss countdown ring and an optional copyable support reference id | [pub.dev ↗](https://pub.dev/packages/toast_overlay) |
| [`queued_toast`](https://pub.dev/packages/queued_toast) | Overlay toasts that queue per screen position, de-duplicate identical messages, and stack up to five at a time | [pub.dev ↗](https://pub.dev/packages/queued_toast) |

**🔐 Networking &amp; security** — <sub>the transport and auth layers behind a live exchange app</sub>

| Package | What it does | Link |
|---|---|---|
| [`dpop_client`](https://pub.dev/packages/dpop_client) | DPoP proof JWTs for Dart (**RFC 9449**) — ES256 key handling, PEM storage, JWK thumbprints, access-token binding, and server-supplied nonces | [pub.dev ↗](https://pub.dev/packages/dpop_client) |
| [`socket_hub`](https://pub.dev/packages/socket_hub) | One WebSocket, many channels — ref-counted subscriptions derived from stream listeners, batched frames, typed payload routing, and resubscribe on reconnect | [pub.dev ↗](https://pub.dev/packages/socket_hub) |

**🛠️ Tooling** — <sub>codegen and design-system chores, automated</sub>

| Package | What it does | Link |
|---|---|---|
| [`openapi_enum_patch`](https://pub.dev/packages/openapi_enum_patch) | Prepares an OpenAPI export for codegen: names the integer enums `swagger_parser` produces, generates the enum files it skips, and audits the ones still unnamed | [pub.dev ↗](https://pub.dev/packages/openapi_enum_patch) |
| [`figma_tokens_gen`](https://pub.dev/packages/figma_tokens_gen) | Generates Flutter `Color` constants and palette maps from Figma design-token JSON exports — ships a CLI and a customisable library API | [pub.dev ↗](https://pub.dev/packages/figma_tokens_gen) |

<br/>

---

## 💼 Professional work

I serve as **Senior Flutter Engineer at DeltaFX**, and as sole senior developer on a cross-platform
brokerage CRM spanning wallets, trading accounts, introducing-broker and affiliate management,
social trading, and AI-assisted market analysis.

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>DeltaFX CRM</h3>
      <sub>Forex brokerage client portal · iOS &amp; Android</sub>
      <br/><br/>
      A modular Flutter application built on Clean Architecture and BLoC across
      <strong>11 feature modules</strong>, supported by generated type-safe API clients,
      resilient authentication, and explicit error boundaries at every layer seam.
      <br/><br/>
      <sub>Wallets · Trading accounts · IB &amp; affiliate management · Social trading · KYC</sub>
    </td>
    <td width="50%" valign="top">
      <h3>BTCB <a href="https://play.google.com/store/apps/details?id=com.btcb.app"><img src="https://img.shields.io/badge/Google_Play-414141?style=flat-square&amp;logo=googleplay&amp;logoColor=white" alt="Google Play"/></a></h3>
      <sub>Cryptocurrency exchange · Futures, Spot &amp; OTC</sub>
      <br/><br/>
      A full exchange client with real-time market data, advanced charting, passkeys and DPoP
      request signing, <strong>9-language localization</strong>, <strong>151 use cases</strong>
      and <strong>63 BLoCs</strong>.
      <br/><br/>
      <sub>Futures · Spot · OTC · Order book · Streaming charts · Passkeys</sub>
    </td>
  </tr>
</table>

<table align="center">
  <tr>
    <td align="center" width="250"><strong>118K LOC</strong><br/><sub>production Flutter codebase</sub></td>
    <td align="center" width="250"><strong>7 days → 2 hours</strong><br/><sub>analytics pipeline runtime</sub></td>
    <td align="center" width="250"><strong>+15% profit</strong><br/><sub>from automated strategies</sub></td>
  </tr>
</table>

<br/>

---

## ⚙️ Core technologies

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

<p align="center">
  <strong>Engineering financial products across mobile, backend, and automation</strong>
  <br/>
  <sub>
    9+ years across brokerage, exchange, and trading-automation systems in Iran, the UAE, Germany, and Turkey.
    <br/>
    Published researcher and author of five papers on neural networks and biomedical signal analysis.
  </sub>
</p>

<p align="center">
  <a href="https://ctrlaltdevelop.github.io">Portfolio</a> ·
  <a href="https://github.com/CtrlAltDevelop">GitHub</a> ·
  <a href="mailto:me.CtrlAltDev@proton.me">Contact</a>
</p>
