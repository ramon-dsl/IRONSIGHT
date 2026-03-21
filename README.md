# IRONSIGHT

Real-time OSINT command center for monitoring the Middle East conflict. Aggregates open-source intelligence from 50+ sources across news, Telegram, military tracking, financial markets, and more into a single dashboard.

Built with Next.js, TypeScript, Tailwind CSS, and Leaflet. No API keys required. Completely free to run.

## Features

- **Live Intel Feed** — 20+ RSS news sources with keyword relevance filtering
- **Telegram OSINT** — 25 channels scraped in real-time with auto-translation
- **Israel Alert Status** — Live Pikud HaOref / Tzeva Adom missile alerts
- **Conflict Monitor** — Categorized events (strikes, defense, diplomatic, nuclear)
- **Missile / Strike Tracker** — Weapon type classification and severity
- **Regional Threat Monitor** — Per-country threat levels across 10 nations
- **Military Airspace** — Live military aircraft tracking via ADS-B
- **Naval Tracker** — Vessel monitoring via GDELT
- **Defense & Markets** — Defense contractor stocks, indices, commodities
- **Energy Markets** — Oil, natural gas, heating oil prices
- **Seismic Monitor** — USGS earthquake data
- **Hot Thermal Detect** — NASA FIRMS fire/explosion detection
- **Humanitarian Reports** — UN OCHA ReliefWeb data

## Data Sources

All data sources are free and require no API keys.

### News RSS Feeds

| Source | Region | Feed |
|--------|--------|------|
| BBC Middle East | International | `feeds.bbci.co.uk` |
| New York Times ME | US | `rss.nytimes.com` |
| Al Jazeera | Qatar/GCC | `aljazeera.com` |
| Reuters World | International | `feeds.reuters.com` |
| CNN Middle East | US | `rss.cnn.com` |
| Fox News World | US | `moxie.foxnews.com` |
| Wall Street Journal | US | `feeds.content.dowjones.io` |
| Times of Israel | Israel | `timesofisrael.com` |
| Jerusalem Post | Israel | `jpost.com` |
| Ynet News | Israel | `ynetnews.com` |
| N12 (Mako) | Israel | `rcs.mako.co.il` |
| Walla News | Israel | `rss.walla.co.il` |
| Haaretz | Israel | `haaretz.com` |
| PressTV | Iran | `presstv.ir` |
| The National | UAE/GCC | `thenationalnews.com` |
| Drop Site News | Independent | `dropsitenews.com` |
| Google News | Aggregator | `news.google.com` (3 conflict-specific searches) |
| Breaking Defense | US Defense | `breakingdefense.com` |
| Long War Journal | US Defense | `longwarjournal.org` |
| Military Times | US Defense | `militarytimes.com` |
| War on the Rocks | US Defense/Analysis | `warontherocks.com` |
| CENTCOM | US Military | `centcom.mil` |
| DoD | US Military | `defense.gov` |

### Telegram Channels

| Channel | Perspective |
|---------|------------|
| @IDFofficial | IDF Official |
| @RocketAlert | Israeli Rocket Alerts |
| @Alertisrael | Alert Israel |
| @TimesofIsrael | Times of Israel |
| @AbuAliExpress | Abu Ali Express (Israeli OSINT) |
| @OSINTdefender | OSINT Defender |
| @warfareanalysis | Warfare Analysis |
| @rnintel | RN Intel |
| @GeoPWatch | GeoPol Watch |
| @middle_east_spectator | ME Spectator |
| @Middle_East_Spectator | ME Spectator 2 |
| @HAMASW | Hamas-Israel War Updates |
| @PressTV | PressTV (Iran) |
| @iranintl_en | Iran International |
| @FarsNews_EN | Fars News (Iran) |
| @TasnimNewsEN | Tasnim News (Iran) |
| @SaberinFa | Saberin (IRGC-affiliated) |
| @defapress_ir | DefaPress (Iran MOD) |
| @sepah | IRGC Official |
| @FotrosResistancee | Fotros Resistance |
| @QudsNen | Quds News |
| @Alsaa_plus_EN | Al-Saa EN |
| @thecradlemedia | The Cradle |
| @dropsitenews | Drop Site News |
| @france24_en | France 24 |

### APIs

| Service | Data | Provider | Cost |
|---------|------|----------|------|
| CNBC Quote API | Stock prices, indices, commodities | CNBC | Free, no key |
| Tzeva Adom | Israeli missile/rocket alerts | Community mirror of Pikud HaOref | Free, no key |
| NASA FIRMS | Fire/thermal detection satellite data | NASA | Free, no key |
| USGS FDSNWS | Earthquake data | US Geological Survey | Free, no key |
| ReliefWeb | Humanitarian reports | UN OCHA | Free, no key |
| adsb.lol | Military aircraft ADS-B tracking | Community ADS-B network | Free, no key |
| EIA | US gas prices | US Energy Information Administration | Free, public demo key |
| GDELT | Global event data (naval tracking) | GDELT Project | Free, no key |
| Google Translate | Hebrew/Arabic/Farsi auto-translation | Google (unofficial) | Free, no key |

### Polling Intervals

| Feed | Interval |
|------|----------|
| Israeli Alerts (Pikud HaOref) | 5 seconds |
| Telegram Channels | 60 seconds |
| News RSS | 90 seconds |
| Strikes | 2 minutes |
| Conflicts | 3 minutes |
| Markets & Oil | 5 minutes |
| Fires (NASA FIRMS) | 10 minutes |

## Getting Started

```bash
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

## Tech Stack

- **Framework:** Next.js 15 (App Router)
- **Language:** TypeScript
- **Styling:** Tailwind CSS
- **Maps:** Leaflet / React-Leaflet
- **XML Parsing:** @xmldom/xmldom

## Disclaimer

This project aggregates publicly available open-source intelligence (OSINT) for informational purposes only. All data is sourced from public RSS feeds, public APIs, and public Telegram channels. No paywalls are bypassed, no authentication is circumvented, and no copyrighted content is reproduced -- only headlines and links are displayed.

Some data sources use unofficial public endpoints (Google Translate, CNBC quotes, Telegram embeds). These endpoints may change without notice. The project includes graceful fallbacks for all data sources.

News content, Telegram posts, and alert data belong to their respective publishers and organizations. This project does not claim ownership of any third-party content.

## License

[MIT](LICENSE)
