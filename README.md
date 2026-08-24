<p align="center">
  <img src="assets/logo.png" alt="CtrlAltDevelop — Mobile · Backend · Beyond" width="560"/>
</p>

<h1 align="center">Mohammad Zarif</h1>

<p align="center">
  <strong>Senior Software Engineer · Flutter &amp; Python · FinTech Systems</strong>
</p>

<p align="center">
  I build production-grade Flutter infrastructure and financial software, then turn the reusable parts into open-source tools for the Dart community.
</p>

<p align="center">
  <a href="https://ctrlaltdevelop.github.io"><img src="https://img.shields.io/badge/View_Portfolio-1F6FEB?style=for-the-badge&amp;logo=googlechrome&amp;logoColor=white" alt="View portfolio"/></a>
  <a href="#open-source"><img src="https://img.shields.io/badge/Open_Source-181717?style=for-the-badge&amp;logo=github&amp;logoColor=white" alt="Explore open-source projects"/></a>
  <a href="mailto:me.CtrlAltDev@proton.me"><img src="https://img.shields.io/badge/Contact_Me-6D4AFF?style=for-the-badge&amp;logo=protonmail&amp;logoColor=white" alt="Contact me"/></a>
</p>

<br/>

<table align="center">
  <tr>
    <td align="center" width="190"><strong>12 packages</strong><br/><sub>published on pub.dev</sub></td>
    <td align="center" width="190"><strong>160 / 160</strong><br/><sub>pub points on every package</sub></td>
    <td align="center" width="190"><strong>26 indicators</strong><br/><sub>in a custom chart engine</sub></td>
    <td align="center" width="190"><strong>MIT licensed</strong><br/><sub>open and reusable</sub></td>
  </tr>
</table>

## Open source

I maintain a focused ecosystem of Dart and Flutter packages extracted from real production needs: financial charting, typed architecture, application security, UI components, notifications, and build tooling. Every package is MIT licensed, publicly documented, and available on both GitHub and pub.dev.

### Flagship projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://pub.dev/packages/ohlcv_chart">ohlcv_chart</a></h3>
      <sub>Financial charting engine for Flutter</sub>
      <br/><br/>
      Candlestick, OHLC, and market-depth charts rendered directly with <code>CustomPainter</code>. Includes <strong>26 indicators</strong>, 17 drawing tools, MACD/RSI/KDJ sub-charts, price alerts, and extensive interaction support.
      <br/><br/>
      <a href="https://pub.dev/packages/ohlcv_chart"><img src="https://img.shields.io/pub/v/ohlcv_chart?style=flat-square&amp;color=0175C2&amp;label=pub.dev" alt="ohlcv_chart on pub.dev"/></a>
      <a href="https://github.com/CtrlAltDevelop/ohlcv_chart"><img src="https://img.shields.io/badge/source-GitHub-181717?style=flat-square&amp;logo=github" alt="ohlcv_chart source on GitHub"/></a>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://pub.dev/packages/verdict">verdict</a> ecosystem</h3>
      <sub>Typed results and predictable BLoC state</sub>
      <br/><br/>
      A sealed <code>Result</code> type, structured <code>Failure</code> hierarchy, and companion BLoC states that preserve the last known good data through loading and failure. Explicit error flow with zero code generation.
      <br/><br/>
      <a href="https://pub.dev/packages/verdict"><img src="https://img.shields.io/pub/v/verdict?style=flat-square&amp;color=0175C2&amp;label=verdict" alt="verdict on pub.dev"/></a>
      <a href="https://pub.dev/packages/verdict_bloc"><img src="https://img.shields.io/pub/v/verdict_bloc?style=flat-square&amp;color=0175C2&amp;label=verdict_bloc" alt="verdict_bloc on pub.dev"/></a>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://pub.dev/packages/dpop_client">dpop_client</a></h3>
      <sub>RFC 9449 security for Dart clients</sub>
      <br/><br/>
      Pure-Dart DPoP proof generation with ES256 keys, JWK thumbprints, access-token binding, PEM storage, and server-supplied nonce handling.
      <br/><br/>
      <a href="https://pub.dev/packages/dpop_client"><img src="https://img.shields.io/pub/v/dpop_client?style=flat-square&amp;color=0175C2&amp;label=pub.dev" alt="dpop_client on pub.dev"/></a>
      <a href="https://github.com/CtrlAltDevelop/dpop_client"><img src="https://img.shields.io/badge/source-GitHub-181717?style=flat-square&amp;logo=github" alt="dpop_client source on GitHub"/></a>
    </td>
    <td width="50%" valign="top">
      <h3>Developer tooling</h3>
      <sub>Safer API models and design-token workflows</sub>
      <br/><br/>
      <a href="https://pub.dev/packages/openapi_enum_patch"><code>openapi_enum_patch</code></a> repairs generated integer enums and audits unresolved names. <a href="https://pub.dev/packages/figma_tokens_gen"><code>figma_tokens_gen</code></a> converts Figma token exports into typed Flutter color APIs.
      <br/><br/>
      <a href="https://github.com/CtrlAltDevelop/openapi_enum_patch"><img src="https://img.shields.io/badge/openapi_enum_patch-GitHub-181717?style=flat-square&amp;logo=github" alt="openapi_enum_patch source"/></a>
      <a href="https://github.com/CtrlAltDevelop/figma_tokens_gen"><img src="https://img.shields.io/badge/figma_tokens_gen-GitHub-181717?style=flat-square&amp;logo=github" alt="figma_tokens_gen source"/></a>
    </td>
  </tr>
</table>

### Package catalog

<table>
  <tr>
    <td width="160"><strong>Architecture</strong></td>
    <td>
      <a href="https://pub.dev/packages/verdict"><code>verdict</code></a> ·
      <a href="https://pub.dev/packages/verdict_bloc"><code>verdict_bloc</code></a> ·
      <a href="https://pub.dev/packages/safe_json_cast"><code>safe_json_cast</code></a>
    </td>
  </tr>
  <tr>
    <td><strong>Charts &amp; UI</strong></td>
    <td>
      <a href="https://pub.dev/packages/ohlcv_chart"><code>ohlcv_chart</code></a> ·
      <a href="https://pub.dev/packages/capsule_nav_bar"><code>capsule_nav_bar</code></a> ·
      <a href="https://pub.dev/packages/sliding_segmented_control"><code>sliding_segmented_control</code></a> ·
      <a href="https://pub.dev/packages/indicator_tab_bar"><code>indicator_tab_bar</code></a>
    </td>
  </tr>
  <tr>
    <td><strong>Notifications</strong></td>
    <td>
      <a href="https://pub.dev/packages/toast_overlay"><code>toast_overlay</code></a> ·
      <a href="https://pub.dev/packages/queued_toast"><code>queued_toast</code></a>
    </td>
  </tr>
  <tr>
    <td><strong>Tooling</strong></td>
    <td>
      <a href="https://pub.dev/packages/openapi_enum_patch"><code>openapi_enum_patch</code></a> ·
      <a href="https://pub.dev/packages/figma_tokens_gen"><code>figma_tokens_gen</code></a>
    </td>
  </tr>
  <tr>
    <td><strong>Security</strong></td>
    <td><a href="https://pub.dev/packages/dpop_client"><code>dpop_client</code></a> — RFC 9449 DPoP proofs in pure Dart</td>
  </tr>
</table>

## Professional work

I serve as the **Senior Flutter Engineer at DeltaFX** and sole senior developer responsible for a cross-platform brokerage CRM spanning wallets, trading accounts, introducing-broker and affiliate management, social trading, and AI-assisted market analysis.

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>DeltaFX CRM</h3>
      <sub>Forex brokerage client portal · iOS &amp; Android</sub>
      <br/><br/>
      A modular Flutter application built with Clean Architecture and BLoC across <strong>11 feature modules</strong>, supported by generated type-safe API clients, resilient authentication, and explicit error boundaries.
    </td>
    <td width="50%" valign="top">
      <h3>BTCB <a href="https://play.google.com/store/apps/details?id=com.btcb.app"><img src="https://img.shields.io/badge/Google_Play-414141?style=flat-square&amp;logo=googleplay&amp;logoColor=white" alt="Google Play"/></a></h3>
      <sub>Cryptocurrency exchange · Futures, Spot &amp; OTC</sub>
      <br/><br/>
      A cryptocurrency exchange application with real-time market data, advanced charting, passkeys, DPoP security, <strong>9-language localization</strong>, 151 use cases, and 63 BLoCs.
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

## Core technologies

<p>
  <strong>Mobile&nbsp;&nbsp;</strong>
  <img src="https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white" alt="Flutter"/>
  <img src="https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=dart&logoColor=white" alt="Dart"/>
  <img src="https://img.shields.io/badge/BLoC-1B6AC6?style=flat-square" alt="BLoC"/>
  <img src="https://img.shields.io/badge/Clean_Architecture-3D5A80?style=flat-square" alt="Clean Architecture"/>
</p>

<p>
  <strong>Backend&nbsp;&nbsp;</strong>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI"/>
  <img src="https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white" alt="Django"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
</p>

<p>
  <strong>Trading&nbsp;&nbsp;</strong>
  <img src="https://img.shields.io/badge/MQL_4%2F5-1F6FEB?style=flat-square" alt="MQL 4 and 5"/>
  <img src="https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=csharp&logoColor=white" alt="C sharp"/>
  <img src="https://img.shields.io/badge/Backtesting-8957E5?style=flat-square" alt="Backtesting"/>
  <img src="https://img.shields.io/badge/Algorithmic_Trading-238636?style=flat-square" alt="Algorithmic Trading"/>
</p>

<p>
  <strong>Delivery&nbsp;&nbsp;</strong>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker"/>
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions"/>
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git"/>
</p>

---

<p align="center">
  <strong>Engineering financial products across mobile, backend, and automation</strong>
  <br/>
  <sub>
    9+ years of experience across brokerage, exchange, and trading-automation systems in Iran, the UAE, Germany, and Turkey.
    <br/>
    Published researcher and author of five papers on neural networks and biomedical signal analysis.
  </sub>
</p>

<p align="center">
  <a href="https://ctrlaltdevelop.github.io">Portfolio</a> ·
  <a href="mailto:me.CtrlAltDev@proton.me">Contact</a>
</p>
