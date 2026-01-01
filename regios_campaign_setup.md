# Regios Energiegenossenschaft Campaign Setup Documentation

**Campaign Period:** 30 Days  
**Total Budget:** EUR 1,500  
**Target Region:** Mühlviertel (Meta) / Upper Austria (Google)  
**Target Audience:** Male & Female, 30+, Property Owners  
**Products:** Beteiligung (Genossenschaft) & Regionaler Grünstrom

---

## ⚠️ IMPORTANT: Assets Pending Replacement

### LANDSCAPE IMAGES FOR RESPONSIVE DISPLAY ADS (1200x628) ARE TEMPORARY CROPS

The landscape (1200x628) images used in Google Responsive Display Ads were cropped from the `Google/RAW/` folder as a temporary solution. These MUST be replaced with properly designed landscape assets once the design team delivers them.

**Affected Campaigns:**
- Google Display Targeting Grünstrom (Responsive Ads)
- Google Display Targeting Genossenschaft (Responsive Ads)

**Note:** Retargeting uses Classic HTML5 banners ONLY (no Responsive).

**Image Sources:**
- Landscape (1200x628): Cropped from `Google/RAW/` folder ⚠️ REPLACE WHEN READY
- Square (1080x1080): From `Social Media/Targeting/Posts/Carousels/1080x1080/` folder ✓

---

## Branded Slogans Reference (MUST USE)

### Main Tagline
- **Strom vom Mühlviertel: Fair, Regional und Grün**

### Dialect Slogans (Mühlviertel specific)
- **Mia san ned Deppad**
- **Mia Mühlviertel san ned Deppad**
- **Mia Mühlviertel entscheiden selber wie es uns weitergeht**
- **Zeigen wir was unser kleines "Bauernland" drauf hat!**

### Energy Element Slogans
- Unser Wasser, Unsere Sonne, Unser Wind, UNSERE ENERGIE REGIOS
- Unsere Stabilität, Unsere Sicherheit, Unsere Zukunft, UNSERE ENERGIE REGIOS
- UNSER MÜHLVIERTEL, UNSERE ENERGIE REGIOS

### Testimonial Slogans
- Unsere Sarah, Unsere Bürger:in, Unser Mühlviertel, UNSERE ENERGIE REGIOS
- Unsere Susanne, Unsere Gemeinde, Unser Mühlviertel, UNSERE ENERGIE REGIOS
- Unsere Jakob, Unsere Bauern, Unser Mühlviertel, UNSERE ENERGIE REGIOS
- Unser Christian, Unsere Stabilität, UNSERE ENERGIE REGIOS
- Unsere Norbert, Unsere Unabhängigkeit, UNSERE ENERGIE REGIOS
- Unsere Sarah, Unsere Gemeinschaft, UNSERE ENERGIE REGIOS
- Unsere Susanne, Unsere Lebensqualität, UNSERE ENERGIE REGIOS

### Call to Actions
- Stärken wir gemeinsam die Region
- Stärken wir gemeinsam das Mühlviertel
- Investiere in die Stabilität des Mühlviertel
- Mach jetzt gleich mit bei der Energiegenossenschaft
- Über 2 Millionen Euro wurden schon in das Mühlviertel investiert
- Über 15 Leitbetriebe aus dem Mühlviertel sind schon dabei
- Über 45 Hektar Grund und Dachflächen sind bereits gepachtet
- Über 250.000 Bürger:innen leben in unserem Mühlviertel
- Über 18 Gemeinden aus dem Mühlviertel sind schon dabei
- Deine Nachbarschaft: In einer Gemeinschaft leben auf die du stolz sein kannst

### Mission & USP
- **Mission:** Unsere Mission ist die Selbstbestimmung über die regionale Energieversorgung durch gemeinsames Eigentum zu sichern
- **Elevator Pitch:** Regios: Ein Energiemodell für regionale Selbstbestimmung, wirtschaftliche Stabilität und faire, grüne Energieversorgung für eine unabhängige und nachhaltige Zukunft
- **USP:** Regios ist die einzige Marke, die wirtschaftliche Stabilität durch ein integriertes Angebot aus Investitionspaketen, grüner Energie und grüner Pacht im Energiemarkt gewährleistet

---

## Table of Contents

1. [UTM Naming Convention](#1-utm-naming-convention)
2. [Budget Allocation](#2-budget-allocation)
3. [Google Search Campaign](#3-google-search-campaign)
4. [Google Display Campaigns](#4-google-display-campaigns)
5. [Google YouTube Campaigns](#5-google-youtube-campaigns)
6. [Meta Facebook Campaigns](#6-meta-facebook-campaigns)
7. [Meta Instagram Campaigns](#7-meta-instagram-campaigns)
8. [Retargeting Campaigns](#8-retargeting-campaigns)
9. [Landing Pages & URLs](#9-landing-pages--urls)
10. [Audience Setup](#10-audience-setup)
11. [Asset Mapping](#11-asset-mapping)
12. [Looker Studio Requirements](#12-looker-studio-requirements)
13. [Campaign Checklist](#13-campaign-checklist)

---

## 1. UTM Naming Convention

### UTM Parameter Structure

All campaigns must follow this strict naming convention for Looker Studio compatibility:

```
utm_source     = [platform]
utm_medium     = [campaign_type]
utm_campaign   = [product]_[funnel_stage]_[creative_theme]
utm_content    = [asset_type]_[asset_name]
utm_term       = [audience_segment] (for search only)
```

### Platform Values (`utm_source`)

| Platform | Value |
|----------|-------|
| Google Search | `google` |
| Google Display | `google` |
| Google YouTube | `google` |
| Meta Facebook | `facebook` |
| Meta Instagram | `instagram` |

### Medium Values (`utm_medium`)

| Campaign Type | Value |
|---------------|-------|
| Search Ads | `cpc` |
| Display Ads | `display` |
| Video Ads | `video` |
| Social Ads | `social` |
| Retargeting | `retargeting` |

### Campaign Values (`utm_campaign`)

| Product | Funnel Stage | Theme | Example |
|---------|--------------|-------|---------|
| gruenstrom | tofu | sonne | `gruenstrom_tofu_sonne` |
| gruenstrom | tofu | wasser | `gruenstrom_tofu_wasser` |
| gruenstrom | tofu | wind | `gruenstrom_tofu_wind` |
| genossenschaft | tofu | stabilitaet | `genossenschaft_tofu_stabilitaet` |
| genossenschaft | tofu | zukunft | `genossenschaft_tofu_zukunft` |
| genossenschaft | tofu | mitgliedschaft | `genossenschaft_tofu_mitgliedschaft` |
| gruenstrom | mofu | retargeting | `gruenstrom_mofu_retargeting` |
| genossenschaft | bofu | testimonial_sarah | `genossenschaft_bofu_testimonial_sarah` |
| brand | search | generic | `brand_search_generic` |

### Content Values (`utm_content`)

| Asset Type | Example |
|------------|---------|
| Video 15s | `video15_sonne_16x9` |
| Video 30s | `video30_genossenschaft_1x1` |
| Banner HTML5 | `banner_stabilitaet_300x250` |
| Carousel | `carousel_sonne_1080x1080` |
| Story | `story_wind_9x16` |
| Testimonial | `testimonial_sarah_short` |

---

## 2. Budget Allocation

### Total Budget: EUR 1,500 / 30 Days

| Platform | Campaign Type | Daily Budget | Monthly Budget | % of Total |
|----------|---------------|--------------|----------------|------------|
| **Google** | Search (Brand/Generic) | €5.00 | €150 | 10% |
| **Google** | Display Targeting Classic (HTML5) | €4.00 | €120 | 8% |
| **Google** | Display Targeting Responsive | €4.00 | €120 | 8% |
| **Google** | Display Retargeting Classic (HTML5) | €5.00 | €150 | 10% |
| **Google** | YouTube Targeting | €3.33 | €100 | 7% |
| **Meta** | Facebook Targeting | €10.00 | €300 | 20% |
| **Meta** | Facebook Retargeting | €6.67 | €200 | 13% |
| **Meta** | Instagram Targeting | €8.33 | €250 | 17% |
| **Meta** | Instagram Retargeting | €3.67 | €110 | 7% |
| **Total** | | **€50.00** | **€1,500** | **100%** |

### Budget Rationale (Based on Historical Performance & Available Assets)

- Meta campaigns showed best Cost per Result: €0.22 to €0.34 per link click
- Google Display CPM: €1.13 to €7.98 (variable)
- YouTube Non skippable CPM: €6.42 to €6.67
- **Targeting:** Both Classic HTML5 AND Responsive Display Ads (to test which performs better)
- **Retargeting:** Classic HTML5 ONLY (higher quality for warm audiences)
- **Responsive Display image sources:** Landscape from Google/RAW (temporary), Square from Social Media Carousels

---

## 3. Google Search Campaign

### Campaign: `[Search > Brand+Generic > Upper Austria > 30+] Regios`

**Settings:**

| Setting | Value |
|---------|-------|
| Campaign Type | Search |
| Goal | Website Traffic |
| Network | Google Search only (no partners) |
| Location | Upper Austria, Austria |
| Language | German |
| Bid Strategy | Manual CPC (Max €0.80) |
| Daily Budget | €5.00 |
| Ad Schedule | All day |
| Device Targeting | All devices |

**Audience:**
- Age: 30 to 65+
- Gender: All

### Ad Group 1: Brand Terms

**Keywords (Exact Match):**
```
[regios]
[regios energie]
[regios energiegenossenschaft]
[regios mühlviertel]
[regios genossenschaft]
[regios grünstrom]
```

**Responsive Search Ad:**

| Field | Content |
|-------|---------|
| Final URL | `https://www.regios.at/?utm_source=google&utm_medium=cpc&utm_campaign=brand_search_generic&utm_content=rsa_brand&utm_term={keyword}` |
| Headline 1 | Regios Energiegenossenschaft |
| Headline 2 | Fair, Regional & Grün |
| Headline 3 | Strom vom Mühlviertel |
| Headline 4 | Von Bürger:innen für Bürger:innen |
| Headline 5 | Mia san ned Deppad |
| Headline 6 | 18+ Gemeinden dabei |
| Headline 7 | Über 2 Mio. € investiert |
| Headline 8 | UNSERE ENERGIE REGIOS |
| Description 1 | Faire, sichere Energie im Mühlviertel. Mach jetzt mit bei der Energiegenossenschaft! |
| Description 2 | Stärken wir gemeinsam das Mühlviertel. 18 Gemeinden und 15 Leitbetriebe sind dabei! |
| Description 3 | Mia san ned Deppad! Unser Wasser, Unsere Sonne, Unser Wind. Jetzt informieren! |
| Description 4 | Von Bürger:innen, für Bürger:innen. Gemeinsam für eine nachhaltige Zukunft! |

### Ad Group 2: Generic Energy Terms

**Keywords (Phrase Match):**
```
"grünstrom oberösterreich"
"regionaler strom mühlviertel"
"energiegenossenschaft oberösterreich"
"ökostrom mühlviertel"
"erneuerbare energie mühlviertel"
"nachhaltige energie oberösterreich"
"strom genossenschaft"
"bürgerenergie österreich"
```

**Negative Keywords:**
```
job
jobs
karriere
arbeit
praktikum
kostenlos
gratis
preis
vergleich
billig
günstig
wechsel
kündigen
```

**Responsive Search Ad:**

| Field | Content |
|-------|---------|
| Final URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=cpc&utm_campaign=gruenstrom_search_generic&utm_content=rsa_generic&utm_term={keyword}` |
| Headline 1 | Grünstrom aus dem Mühlviertel |
| Headline 2 | Mia san ned Deppad |
| Headline 3 | Fair, Regional & Nachhaltig |
| Headline 4 | Strom aus Sonne, Wind & Wasser |
| Headline 5 | UNSERE ENERGIE REGIOS |
| Headline 6 | Jetzt Teil werden |
| Headline 7 | Stabilität für die Region |
| Headline 8 | Von Bürger:innen getragen |
| Description 1 | Strom vom Mühlviertel: Fair, Regional und Grün. Von Bürger:innen, für Bürger:innen. |
| Description 2 | Investiere in die Stabilität des Mühlviertel. Über 2 Mio. € bereits investiert! |
| Description 3 | Mia Mühlviertel entscheiden selber. Stärken wir gemeinsam das Mühlviertel! |

### Sitelink Extensions (Both Ad Groups)

**Sitelink 1: Bürger**

| Field | Content |
|-------|---------|
| Sitelink Text | Für Bürger:innen |
| Description Line 1 | Unsere Sarah, Unsere Gemeinschaft |
| Description Line 2 | UNSERE ENERGIE REGIOS |
| Final URL | `https://www.regios.at/buerger?utm_source=google&utm_medium=cpc&utm_campaign=brand_search_generic&utm_content=sitelink_buerger` |

**Sitelink 2: Beteiligung**

| Field | Content |
|-------|---------|
| Sitelink Text | Beteiligung |
| Description Line 1 | Investiere in die Stabilität |
| Description Line 2 | Über 2 Mio. € investiert |
| Final URL | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=cpc&utm_campaign=brand_search_generic&utm_content=sitelink_beteiligung` |

**Sitelink 3: Regionaler Grünstrom**

| Field | Content |
|-------|---------|
| Sitelink Text | Regionaler Grünstrom |
| Description Line 1 | Fair, Regional und Grün |
| Description Line 2 | Sonne, Wind und Wasser |
| Final URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=cpc&utm_campaign=brand_search_generic&utm_content=sitelink_gruenstrom` |

**Sitelink 4: Grundstücksentwicklung**

| Field | Content |
|-------|---------|
| Sitelink Text | Grundstücksentwicklung |
| Description Line 1 | 45+ Hektar bereits gepachtet |
| Description Line 2 | Grüne Pacht fürs Mühlviertel |
| Final URL | `https://www.regios.at/grundstuecksentwicklung?utm_source=google&utm_medium=cpc&utm_campaign=brand_search_generic&utm_content=sitelink_grundstueck` |

**Sitelink 5: Kontakt**

| Field | Content |
|-------|---------|
| Sitelink Text | Kontakt |
| Description Line 1 | Persönliche Beratung |
| Description Line 2 | Wir sind für dich da |
| Final URL | `https://www.regios.at/kontakt?utm_source=google&utm_medium=cpc&utm_campaign=brand_search_generic&utm_content=sitelink_kontakt` |

---

## 4. Google Display Campaigns

### Campaign Structure Overview

| Campaign Type | Ad Format | Purpose |
|---------------|-----------|---------|
| **Targeting Classic** | HTML5 Banners | Prospecting with high-quality animated banners |
| **Targeting Responsive** | Responsive Display Ads | Prospecting with auto-optimized placements |
| **Retargeting Classic** | HTML5 Banners | Remarketing with high-quality animated banners |

**Note:** We use Responsive Display Ads for TARGETING only. Retargeting uses Classic HTML5 only.

---

### Asset Sources

**Classic Display (HTML5 Banners):**
- Location: `Google/Retargeting/Banners/HTML5/`
- Themes: Wasser, Wind, Licht (Sonne), Stabilitaet, Zukunft, Sarah

**Responsive Display Ads:**
- Landscape (1200x628): `Google/RAW/` folder ⚠️ TEMPORARY CROPS - REPLACE WHEN DESIGN READY
- Square (1080x1080): `Social Media/Targeting/Posts/Carousels/1080x1080/` folder ✓

---

### Campaign A: Display Targeting Grünstrom (Classic HTML5)
`[Display > Classic > Targeting > Upper Austria > 30+] Gruenstrom`

**Settings:**

| Setting | Value |
|---------|-------|
| Campaign Type | Display |
| Campaign Subtype | Standard Display Campaign |
| Goal | Website Traffic |
| Network | Display Network |
| Location | Upper Austria, Austria |
| Language | German |
| Bid Strategy | Target CPM (€3.00) |
| Daily Budget | €2.00 |
| Frequency Cap | 5 impressions per user per day |

**Audience Targeting:**
- Age: 30 to 65+
- Gender: All
- Household Income: Top 50%
- Affinity Audiences: Green Living Enthusiasts, Home & Garden/Home Improvement
- In Market: Business Services/Utilities, Real Estate/Residential Properties

---

#### Ad Group 1: Wasser (HTML5 Banners)

| Size | File | UTM URL |
|------|------|---------|
| 300x250 | Google/Retargeting/Banners/HTML5/Wasser_300x250.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=display&utm_campaign=gruenstrom_tofu_wasser&utm_content=banner_wasser_300x250` |
| 300x600 | Google/Retargeting/Banners/HTML5/Wasser_300x600.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=display&utm_campaign=gruenstrom_tofu_wasser&utm_content=banner_wasser_300x600` |
| 320x50 | Google/Retargeting/Banners/HTML5/Wasser_320x50.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=display&utm_campaign=gruenstrom_tofu_wasser&utm_content=banner_wasser_320x50` |
| 336x280 | Google/Retargeting/Banners/HTML5/Wasser_336x280.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=display&utm_campaign=gruenstrom_tofu_wasser&utm_content=banner_wasser_336x280` |
| 728x90 | Google/Retargeting/Banners/HTML5/Wasser_728x90.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=display&utm_campaign=gruenstrom_tofu_wasser&utm_content=banner_wasser_728x90` |

---

#### Ad Group 2: Wind (HTML5 Banners)

| Size | File | UTM URL |
|------|------|---------|
| 300x250 | Google/Retargeting/Banners/HTML5/Wind_300x250.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=display&utm_campaign=gruenstrom_tofu_wind&utm_content=banner_wind_300x250` |
| 300x600 | Google/Retargeting/Banners/HTML5/Wind_300x600.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=display&utm_campaign=gruenstrom_tofu_wind&utm_content=banner_wind_300x600` |
| 320x50 | Google/Retargeting/Banners/HTML5/Wind_320x50.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=display&utm_campaign=gruenstrom_tofu_wind&utm_content=banner_wind_320x50` |
| 336x280 | Google/Retargeting/Banners/HTML5/Wind_336x280.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=display&utm_campaign=gruenstrom_tofu_wind&utm_content=banner_wind_336x280` |
| 728x90 | Google/Retargeting/Banners/HTML5/Wind_728x90.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=display&utm_campaign=gruenstrom_tofu_wind&utm_content=banner_wind_728x90` |

---

#### Ad Group 3: Licht/Sonne (HTML5 Banners)

| Size | File | UTM URL |
|------|------|---------|
| 300x250 | Google/Retargeting/Banners/HTML5/Licht_300x250.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=display&utm_campaign=gruenstrom_tofu_sonne&utm_content=banner_licht_300x250` |
| 300x600 | Google/Retargeting/Banners/HTML5/Licht_300x600.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=display&utm_campaign=gruenstrom_tofu_sonne&utm_content=banner_licht_300x600` |
| 320x50 | Google/Retargeting/Banners/HTML5/Licht_320x50.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=display&utm_campaign=gruenstrom_tofu_sonne&utm_content=banner_licht_320x50` |
| 336x280 | Google/Retargeting/Banners/HTML5/Licht_336x280.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=display&utm_campaign=gruenstrom_tofu_sonne&utm_content=banner_licht_336x280` |
| 728x90 | Google/Retargeting/Banners/HTML5/Licht_728x90.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=display&utm_campaign=gruenstrom_tofu_sonne&utm_content=banner_licht_728x90` |

---

### Campaign A2: Display Targeting Grünstrom (Responsive)
`[Display > Responsive > Targeting > Upper Austria > 30+] Gruenstrom`

**Settings:**

| Setting | Value |
|---------|-------|
| Campaign Type | Display |
| Campaign Subtype | Standard Display Campaign |
| Goal | Website Traffic |
| Network | Display Network |
| Location | Upper Austria, Austria |
| Language | German |
| Bid Strategy | Target CPM (€3.00) |
| Daily Budget | €2.00 |
| Frequency Cap | 5 impressions per user per day |

**Audience Targeting:** Same as Classic campaign above.

---

#### Responsive Display Ad: Sonne

| Field | Content |
|-------|---------|
| Final URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=display&utm_campaign=gruenstrom_tofu_sonne&utm_content=responsive_sonne` |
| Landscape Image (1200x628) | Google/RAW/[Sonne image cropped] ⚠️ TEMPORARY |
| Square Image (1080x1080) | Social Media/Targeting/Posts/Carousels/1080x1080/sonne/Sonne_1080x1080_1.png |
| Headline 1 | Unsere Sonne, UNSERE ENERGIE |
| Headline 2 | Mia san ned Deppad |
| Headline 3 | Regional. Fair. Grün. |
| Headline 4 | Grünstrom aus dem Mühlviertel |
| Headline 5 | Sonnenenergie für die Region |
| Long Headline | Unsere Sonne, Unser Mühlviertel, UNSERE ENERGIE REGIOS |
| Description 1 | Stärken wir gemeinsam das Mühlviertel. Investiere in die Stabilität der Region. |
| Description 2 | Über 2 Millionen Euro wurden schon in das Mühlviertel investiert. Mach jetzt mit! |
| Description 3 | Strom vom Mühlviertel: Fair, Regional und Grün. Von Bürger:innen, für Bürger:innen. |
| Description 4 | Mia Mühlviertel san ned Deppad! Sonnenenergie aus der Region. Jetzt informieren! |
| Business Name | Regios Energiegenossenschaft |

---

#### Responsive Display Ad: Wasser

| Field | Content |
|-------|---------|
| Final URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=display&utm_campaign=gruenstrom_tofu_wasser&utm_content=responsive_wasser` |
| Landscape Image (1200x628) | Google/RAW/[Wasser image cropped] ⚠️ TEMPORARY |
| Square Image (1080x1080) | Social Media/Targeting/Posts/Carousels/1080x1080/wasser/wasser_1080x1080_1.png |
| Headline 1 | Unser Wasser, UNSERE ENERGIE |
| Headline 2 | Mia san ned Deppad |
| Headline 3 | Regional. Fair. Grün. |
| Headline 4 | Wasserkraft aus dem Mühlviertel |
| Headline 5 | Regionale Wasserkraft |
| Long Headline | Unser Wasser, Unser Mühlviertel, UNSERE ENERGIE REGIOS |
| Description 1 | Stärken wir gemeinsam das Mühlviertel. Investiere in die Stabilität der Region. |
| Description 2 | Über 18 Gemeinden aus dem Mühlviertel sind schon dabei. Werde Teil der Bewegung! |
| Description 3 | Strom vom Mühlviertel: Fair, Regional und Grün. Von Bürger:innen, für Bürger:innen. |
| Description 4 | Mia Mühlviertel san ned Deppad! Wasserkraft aus der Region. Jetzt informieren! |
| Business Name | Regios Energiegenossenschaft |

---

#### Responsive Display Ad: Wind

| Field | Content |
|-------|---------|
| Final URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=display&utm_campaign=gruenstrom_tofu_wind&utm_content=responsive_wind` |
| Landscape Image (1200x628) | Google/RAW/[Wind image cropped] ⚠️ TEMPORARY |
| Square Image (1080x1080) | Social Media/Targeting/Posts/Carousels/1080x1080/wind/WInd_1080x1080_1.png |
| Headline 1 | Unser Wind, UNSERE ENERGIE |
| Headline 2 | Mia san ned Deppad |
| Headline 3 | Regional. Fair. Grün. |
| Headline 4 | Windenergie aus dem Mühlviertel |
| Headline 5 | Regionale Windkraft |
| Long Headline | Unser Wind, Unser Mühlviertel, UNSERE ENERGIE REGIOS |
| Description 1 | Stärken wir gemeinsam das Mühlviertel. Investiere in die Stabilität der Region. |
| Description 2 | Über 15 Leitbetriebe aus dem Mühlviertel sind schon dabei. Jetzt informieren! |
| Description 3 | Strom vom Mühlviertel: Fair, Regional und Grün. Von Bürger:innen, für Bürger:innen. |
| Description 4 | Mia Mühlviertel san ned Deppad! Windenergie aus der Region. Jetzt informieren! |
| Business Name | Regios Energiegenossenschaft |

---

### Campaign B: Display Targeting Genossenschaft (Classic HTML5)
`[Display > Classic > Targeting > Upper Austria > 30+] Genossenschaft`

**Settings:**

| Setting | Value |
|---------|-------|
| Campaign Type | Display |
| Campaign Subtype | Standard Display Campaign |
| Goal | Website Traffic |
| Network | Display Network |
| Location | Upper Austria, Austria |
| Language | German |
| Bid Strategy | Target CPM (€3.00) |
| Daily Budget | €2.00 |
| Frequency Cap | 5 impressions per user per day |

**Audience Targeting:**
- Age: 30 to 65+
- Gender: All
- Household Income: Top 50%
- Affinity Audiences: Green Living Enthusiasts, Banking & Finance/Investment
- In Market: Business Services/Utilities, Real Estate/Residential Properties

---

#### Ad Group 1: Stabilitaet (HTML5 Banners)

| Size | File | UTM URL |
|------|------|---------|
| 160x600 | Google/Retargeting/Banners/HTML5/Stabilitaet_160x600.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=display&utm_campaign=genossenschaft_tofu_stabilitaet&utm_content=banner_stabilitaet_160x600` |
| 300x250 | Google/Retargeting/Banners/HTML5/Stabilitaet_300x250.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=display&utm_campaign=genossenschaft_tofu_stabilitaet&utm_content=banner_stabilitaet_300x250` |
| 300x600 | Google/Retargeting/Banners/HTML5/Stabilitaet_300x600.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=display&utm_campaign=genossenschaft_tofu_stabilitaet&utm_content=banner_stabilitaet_300x600` |
| 320x50 | Google/Retargeting/Banners/HTML5/Stabilitaet_320x50.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=display&utm_campaign=genossenschaft_tofu_stabilitaet&utm_content=banner_stabilitaet_320x50` |
| 320x100 | Google/Retargeting/Banners/HTML5/Stabilitaet_320X100.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=display&utm_campaign=genossenschaft_tofu_stabilitaet&utm_content=banner_stabilitaet_320x100` |
| 336x280 | Google/Retargeting/Banners/HTML5/Stabilitaet_336x280.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=display&utm_campaign=genossenschaft_tofu_stabilitaet&utm_content=banner_stabilitaet_336x280` |
| 728x90 | Google/Retargeting/Banners/HTML5/Stabilitaet_728x90.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=display&utm_campaign=genossenschaft_tofu_stabilitaet&utm_content=banner_stabilitaet_728x90` |
| 970x250 | Google/Retargeting/Banners/HTML5/Stabilitaet_970x250.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=display&utm_campaign=genossenschaft_tofu_stabilitaet&utm_content=banner_stabilitaet_970x250` |

---

#### Ad Group 2: Zukunft (HTML5 Banners)

| Size | File | UTM URL |
|------|------|---------|
| 300x250 | Google/Retargeting/Banners/HTML5/Zukunft_300x250.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=display&utm_campaign=genossenschaft_tofu_zukunft&utm_content=banner_zukunft_300x250` |
| 300x600 | Google/Retargeting/Banners/HTML5/Zukunft_300x600.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=display&utm_campaign=genossenschaft_tofu_zukunft&utm_content=banner_zukunft_300x600` |
| 320x50 | Google/Retargeting/Banners/HTML5/Zukunft_320x50.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=display&utm_campaign=genossenschaft_tofu_zukunft&utm_content=banner_zukunft_320x50` |
| 336x280 | Google/Retargeting/Banners/HTML5/Zukunft_336x280.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=display&utm_campaign=genossenschaft_tofu_zukunft&utm_content=banner_zukunft_336x280` |
| 728x90 | Google/Retargeting/Banners/HTML5/Zukunft_728x90.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=display&utm_campaign=genossenschaft_tofu_zukunft&utm_content=banner_zukunft_728x90` |

---

### Campaign B2: Display Targeting Genossenschaft (Responsive)
`[Display > Responsive > Targeting > Upper Austria > 30+] Genossenschaft`

**Settings:**

| Setting | Value |
|---------|-------|
| Campaign Type | Display |
| Campaign Subtype | Standard Display Campaign |
| Goal | Website Traffic |
| Network | Display Network |
| Location | Upper Austria, Austria |
| Language | German |
| Bid Strategy | Target CPM (€3.00) |
| Daily Budget | €2.00 |
| Frequency Cap | 5 impressions per user per day |

**Audience Targeting:** Same as Classic campaign above.

---

#### Responsive Display Ad: Stabilitaet

| Field | Content |
|-------|---------|
| Final URL | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=display&utm_campaign=genossenschaft_tofu_stabilitaet&utm_content=responsive_stabilitaet` |
| Landscape Image (1200x628) | Google/RAW/[Stabilitaet image cropped] ⚠️ TEMPORARY |
| Square Image (1080x1080) | Social Media/Targeting/Posts/Carousels/1080x1080/Stabilitaet/Stabilitaet_1080x1080_1.png |
| Headline 1 | Unsere Stabilität, UNSERE ENERGIE |
| Headline 2 | Mia san ned Deppad |
| Headline 3 | Investiere in die Region |
| Headline 4 | Wirtschaftliche Stabilität |
| Headline 5 | Beteiligung am Mühlviertel |
| Long Headline | Unsere Stabilität, Unsere Sicherheit, Unsere Zukunft, UNSERE ENERGIE REGIOS |
| Description 1 | Investiere in die Stabilität des Mühlviertel. Über 2 Mio. € bereits in die Region investiert. |
| Description 2 | Mia Mühlviertel entscheiden selber wie es uns weitergeht. Jetzt Mitglied werden! |
| Description 3 | Regios: Ein Energiemodell für regionale Selbstbestimmung und wirtschaftliche Stabilität. |
| Description 4 | Mach jetzt gleich mit bei der Energiegenossenschaft. Von Bürger:innen, für Bürger:innen. |
| Business Name | Regios Energiegenossenschaft |

---

#### Responsive Display Ad: Zukunft

| Field | Content |
|-------|---------|
| Final URL | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=display&utm_campaign=genossenschaft_tofu_zukunft&utm_content=responsive_zukunft` |
| Landscape Image (1200x628) | Google/RAW/[Zukunft image cropped] ⚠️ TEMPORARY |
| Square Image (1080x1080) | Social Media/Targeting/Posts/Carousels/1080x1080/Zukunft/Zukunft_1080x1080_1.png |
| Headline 1 | Unsere Zukunft, UNSERE ENERGIE |
| Headline 2 | Mia san ned Deppad |
| Headline 3 | Gemeinsam stark |
| Headline 4 | Zukunft fürs Mühlviertel |
| Headline 5 | Nachhaltige Energie |
| Long Headline | Ein Modell für regionale Selbstbestimmung, Stabilität und eine lebenswerte Zukunft |
| Description 1 | Mach jetzt gleich mit bei der Energiegenossenschaft. Über 18 Gemeinden sind schon dabei! |
| Description 2 | Zeigen wir was unser kleines Bauernland drauf hat! Von Bürger:innen, für Bürger:innen. |
| Description 3 | Stärken wir gemeinsam das Mühlviertel. Jetzt Teil der Energiegenossenschaft werden! |
| Description 4 | Mia Mühlviertel san ned Deppad! Gemeinsam für eine nachhaltige Zukunft. |
| Business Name | Regios Energiegenossenschaft |

---

### Campaign C: Display Retargeting (Classic HTML5)
`[Display > Classic > Retargeting > Upper Austria > 30+] Retargeting`

**Settings:**

| Setting | Value |
|---------|-------|
| Campaign Type | Display |
| Campaign Subtype | Standard Display Campaign |
| Goal | Website Traffic |
| Network | Display Network |
| Location | Upper Austria, Austria |
| Language | German |
| Bid Strategy | Target CPA (€2.00) |
| Daily Budget | €5.00 |
| Frequency Cap | 3 impressions per user per day |

**Audience Targeting:**
- Remarketing Lists: Website Visitors (All) Past 30 days
- Audience: Bürger (visitors to /buerger)
- Audience: Genossenschaft (visitors to /beteiligung)
- Audience: Grünstrom (visitors to /regionaler gruenstrom)

---

#### Ad Group 1: Grünstrom Retargeting (HTML5 Banners)

**Use same banners as Targeting but with retargeting UTM medium:**

**Theme: Wasser**

| Size | File | UTM URL |
|------|------|---------|
| 300x250 | Google/Retargeting/Banners/HTML5/Wasser_300x250.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=retargeting&utm_campaign=gruenstrom_mofu_retargeting&utm_content=banner_wasser_300x250` |
| 300x600 | Google/Retargeting/Banners/HTML5/Wasser_300x600.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=retargeting&utm_campaign=gruenstrom_mofu_retargeting&utm_content=banner_wasser_300x600` |
| 320x50 | Google/Retargeting/Banners/HTML5/Wasser_320x50.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=retargeting&utm_campaign=gruenstrom_mofu_retargeting&utm_content=banner_wasser_320x50` |
| 336x280 | Google/Retargeting/Banners/HTML5/Wasser_336x280.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=retargeting&utm_campaign=gruenstrom_mofu_retargeting&utm_content=banner_wasser_336x280` |
| 728x90 | Google/Retargeting/Banners/HTML5/Wasser_728x90.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=retargeting&utm_campaign=gruenstrom_mofu_retargeting&utm_content=banner_wasser_728x90` |

**Theme: Wind**

| Size | File | UTM URL |
|------|------|---------|
| 300x250 | Google/Retargeting/Banners/HTML5/Wind_300x250.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=retargeting&utm_campaign=gruenstrom_mofu_retargeting&utm_content=banner_wind_300x250` |
| 300x600 | Google/Retargeting/Banners/HTML5/Wind_300x600.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=retargeting&utm_campaign=gruenstrom_mofu_retargeting&utm_content=banner_wind_300x600` |
| 320x50 | Google/Retargeting/Banners/HTML5/Wind_320x50.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=retargeting&utm_campaign=gruenstrom_mofu_retargeting&utm_content=banner_wind_320x50` |
| 336x280 | Google/Retargeting/Banners/HTML5/Wind_336x280.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=retargeting&utm_campaign=gruenstrom_mofu_retargeting&utm_content=banner_wind_336x280` |
| 728x90 | Google/Retargeting/Banners/HTML5/Wind_728x90.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=retargeting&utm_campaign=gruenstrom_mofu_retargeting&utm_content=banner_wind_728x90` |

**Theme: Licht (Sonne)**

| Size | File | UTM URL |
|------|------|---------|
| 300x250 | Google/Retargeting/Banners/HTML5/Licht_300x250.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=retargeting&utm_campaign=gruenstrom_mofu_retargeting&utm_content=banner_licht_300x250` |
| 300x600 | Google/Retargeting/Banners/HTML5/Licht_300x600.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=retargeting&utm_campaign=gruenstrom_mofu_retargeting&utm_content=banner_licht_300x600` |
| 320x50 | Google/Retargeting/Banners/HTML5/Licht_320x50.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=retargeting&utm_campaign=gruenstrom_mofu_retargeting&utm_content=banner_licht_320x50` |
| 336x280 | Google/Retargeting/Banners/HTML5/Licht_336x280.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=retargeting&utm_campaign=gruenstrom_mofu_retargeting&utm_content=banner_licht_336x280` |
| 728x90 | Google/Retargeting/Banners/HTML5/Licht_728x90.zip | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=retargeting&utm_campaign=gruenstrom_mofu_retargeting&utm_content=banner_licht_728x90` |

---

#### Ad Group 2: Genossenschaft Retargeting (HTML5 Banners)

**Theme: Stabilitaet**

| Size | File | UTM URL |
|------|------|---------|
| 160x600 | Google/Retargeting/Banners/HTML5/Stabilitaet_160x600.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=retargeting&utm_campaign=genossenschaft_mofu_retargeting&utm_content=banner_stabilitaet_160x600` |
| 300x250 | Google/Retargeting/Banners/HTML5/Stabilitaet_300x250.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=retargeting&utm_campaign=genossenschaft_mofu_retargeting&utm_content=banner_stabilitaet_300x250` |
| 300x600 | Google/Retargeting/Banners/HTML5/Stabilitaet_300x600.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=retargeting&utm_campaign=genossenschaft_mofu_retargeting&utm_content=banner_stabilitaet_300x600` |
| 320x50 | Google/Retargeting/Banners/HTML5/Stabilitaet_320x50.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=retargeting&utm_campaign=genossenschaft_mofu_retargeting&utm_content=banner_stabilitaet_320x50` |
| 320x100 | Google/Retargeting/Banners/HTML5/Stabilitaet_320X100.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=retargeting&utm_campaign=genossenschaft_mofu_retargeting&utm_content=banner_stabilitaet_320x100` |
| 336x280 | Google/Retargeting/Banners/HTML5/Stabilitaet_336x280.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=retargeting&utm_campaign=genossenschaft_mofu_retargeting&utm_content=banner_stabilitaet_336x280` |
| 728x90 | Google/Retargeting/Banners/HTML5/Stabilitaet_728x90.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=retargeting&utm_campaign=genossenschaft_mofu_retargeting&utm_content=banner_stabilitaet_728x90` |
| 970x250 | Google/Retargeting/Banners/HTML5/Stabilitaet_970x250.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=retargeting&utm_campaign=genossenschaft_mofu_retargeting&utm_content=banner_stabilitaet_970x250` |

**Theme: Zukunft**

| Size | File | UTM URL |
|------|------|---------|
| 300x250 | Google/Retargeting/Banners/HTML5/Zukunft_300x250.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=retargeting&utm_campaign=genossenschaft_mofu_retargeting&utm_content=banner_zukunft_300x250` |
| 300x600 | Google/Retargeting/Banners/HTML5/Zukunft_300x600.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=retargeting&utm_campaign=genossenschaft_mofu_retargeting&utm_content=banner_zukunft_300x600` |
| 320x50 | Google/Retargeting/Banners/HTML5/Zukunft_320x50.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=retargeting&utm_campaign=genossenschaft_mofu_retargeting&utm_content=banner_zukunft_320x50` |
| 336x280 | Google/Retargeting/Banners/HTML5/Zukunft_336x280.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=retargeting&utm_campaign=genossenschaft_mofu_retargeting&utm_content=banner_zukunft_336x280` |
| 728x90 | Google/Retargeting/Banners/HTML5/Zukunft_728x90.zip | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=retargeting&utm_campaign=genossenschaft_mofu_retargeting&utm_content=banner_zukunft_728x90` |

**Theme: Sarah (Testimonial - BOFU)**

| Size | File | UTM URL |
|------|------|---------|
| 300x250 | Google/Retargeting/Banners/HTML5/Sarah_300x250.zip | `https://www.regios.at/buerger?utm_source=google&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_retargeting&utm_content=banner_sarah_300x250` |
| 300x600 | Google/Retargeting/Banners/HTML5/Sarah_300x600.zip | `https://www.regios.at/buerger?utm_source=google&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_retargeting&utm_content=banner_sarah_300x600` |
| 320x50 | Google/Retargeting/Banners/HTML5/Sarah_320x50.zip | `https://www.regios.at/buerger?utm_source=google&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_retargeting&utm_content=banner_sarah_320x50` |
| 320x100 | Google/Retargeting/Banners/HTML5/Sarah_320x100.zip | `https://www.regios.at/buerger?utm_source=google&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_retargeting&utm_content=banner_sarah_320x100` |
| 336x280 | Google/Retargeting/Banners/HTML5/Sarah_336x280.zip | `https://www.regios.at/buerger?utm_source=google&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_retargeting&utm_content=banner_sarah_336x280` |
| 728x90 | Google/Retargeting/Banners/HTML5/Sarah_728X90.zip | `https://www.regios.at/buerger?utm_source=google&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_retargeting&utm_content=banner_sarah_728x90` |

---

## 5. Google YouTube Campaigns

### Recommendation on YouTube

**Cost Analysis:**
- Historical YouTube Non skippable CPM: €6.42 to €6.67
- With €100 budget: approximately 15,000 impressions expected
- Reach in Mühlviertel limited due to geo targeting

**Recommendation:** Include YouTube with limited budget (€100) for brand awareness. Use 15 second non skippable for cost efficiency.

### Campaign: YouTube Targeting Grünstrom

**Campaign:** `[Video > Non skippable > Muehviertel > 30+] 15 Sek Strom`

**Settings:**

| Setting | Value |
|---------|-------|
| Campaign Type | Video |
| Campaign Subtype | Video Reach |
| Goal | Brand Awareness and Reach |
| Bid Strategy | Target CPM (€8.00) |
| Daily Budget | €3.33 |
| Networks | YouTube Videos |
| Location | Upper Austria, Austria |
| Language | German |
| Frequency Cap | 3 per week |

**Audience Targeting:**
- Age: 30 to 65+
- Gender: All
- Detailed Demographics: Homeowners
- Affinity: Green Living, Home Improvement

**Ad Group 1: Sonne**

| Field | Content |
|-------|---------|
| Video | `15 Sek Strom - Sonne - Online - 16-9 - V1.mp4` |
| Final URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=video&utm_campaign=gruenstrom_tofu_sonne&utm_content=video15_sonne_16x9` |
| Display URL | regios.at |
| CTA | Mehr erfahren |
| Headline | Unsere Sonne, UNSERE ENERGIE REGIOS |

**Ad Group 2: Wasser**

| Field | Content |
|-------|---------|
| Video | `15 Sek Strom - Wasser - Online - 16-9 - V1.mp4` |
| Final URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=video&utm_campaign=gruenstrom_tofu_wasser&utm_content=video15_wasser_16x9` |
| Display URL | regios.at |
| CTA | Mehr erfahren |
| Headline | Unser Wasser, UNSERE ENERGIE REGIOS |

**Ad Group 3: Wind**

| Field | Content |
|-------|---------|
| Video | `15 Sek Strom - Wind - Online - 16-9 - V1.mp4` |
| Final URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=video&utm_campaign=gruenstrom_tofu_wind&utm_content=video15_wind_16x9` |
| Display URL | regios.at |
| CTA | Mehr erfahren |
| Headline | Unser Wind, UNSERE ENERGIE REGIOS |

---

## 6. Meta Facebook Campaigns

### Campaign A: Targeting Grünstrom

**Campaign:** `[Awareness > Auction > Muehviertel > 30+] Gruenstrom`

**Campaign Settings:**

| Setting | Value |
|---------|-------|
| Campaign Objective | Awareness |
| Buying Type | Auction |
| Campaign Budget Optimization | On |
| Campaign Budget | €150 (Lifetime) |
| Campaign Bid Strategy | Lowest cost |

**Ad Set Settings:**

| Setting | Value |
|---------|-------|
| Placements | Facebook Feed, Facebook Video Feeds, Facebook Stories, Facebook Reels |
| Location | Mühlviertel region (Freistadt, Perg, Rohrbach, Urfahr Umgebung districts) |
| Age | 30 to 65+ |
| Gender | All |
| Detailed Targeting | Interests: Renewable energy, Sustainability, Home ownership, Local community |
| Optimization Goal | Reach |
| Frequency Cap | 2 per week |
| Attribution | 7 day click, 1 day view |

**Ad 1: Sonne (Feed 1:1 + Story 9:16)**

| Field | Content |
|-------|---------|
| Video Feed (1:1) | `15 Sek Strom - Sonne - Online - 1-1 - V1.mp4` |
| Video Story (9:16) | `15 Sek Strom - Sonne - Online - 9-16 - V3.mp4` |
| Primary Text | ☀️ Unsere Sonne, Unser Mühlviertel, UNSERE ENERGIE REGIOS<br><br>Strom vom Mühlviertel: Fair, Regional und Grün.<br><br>Mia san ned Deppad! Über 2 Millionen Euro wurden schon in das Mühlviertel investiert. Stärken wir gemeinsam die Region!<br><br>🌱 Von Bürger:innen, für Bürger:innen. |
| Headline | Grünstrom aus dem Mühlviertel |
| CTA | Learn More |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=facebook&utm_medium=social&utm_campaign=gruenstrom_tofu_sonne&utm_content=video15_sonne_feed_story` |

**Ad 2: Wasser (Feed 1:1 + Story 9:16)**

| Field | Content |
|-------|---------|
| Video Feed (1:1) | `15 Sek Strom - Wasser - Online - 1-1 - V1.mp4` |
| Video Story (9:16) | `15 Sek Strom - Wasser - Online - 9-16 - V3.mp4` |
| Primary Text | 💧 Unser Wasser, Unser Mühlviertel, UNSERE ENERGIE REGIOS<br><br>Mia Mühlviertel san ned Deppad! Regionale Wasserkraft für eine nachhaltige Zukunft.<br><br>Über 18 Gemeinden aus dem Mühlviertel sind schon dabei!<br><br>🌱 Fair. Regional. Grün. |
| Headline | Wasserkraft aus dem Mühlviertel |
| CTA | Learn More |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=facebook&utm_medium=social&utm_campaign=gruenstrom_tofu_wasser&utm_content=video15_wasser_feed_story` |

**Ad 3: Wind (Feed 1:1 + Story 9:16)**

| Field | Content |
|-------|---------|
| Video Feed (1:1) | `15 Sek Strom - Wind - Online - 1-1 - V1.mp4` |
| Video Story (9:16) | `15 Sek Strom - Wind - Online - 9-16 - V3.mp4` |
| Primary Text | 🌬️ Unser Wind, Unser Mühlviertel, UNSERE ENERGIE REGIOS<br><br>Mia san ned Deppad! Windenergie aus der Region, für die Region.<br><br>Über 15 Leitbetriebe aus dem Mühlviertel sind schon dabei!<br><br>🌱 Gemeinsam stark. |
| Headline | Windenergie aus dem Mühlviertel |
| CTA | Learn More |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=facebook&utm_medium=social&utm_campaign=gruenstrom_tofu_wind&utm_content=video15_wind_feed_story` |

**Ad 4: Strom 30s (Feed 1:1 + Story 9:16)**

| Field | Content |
|-------|---------|
| Video Feed (1:1) | `30 Sek Kurz - Strom - TV - 1-1 - V1 ohne URL.mp4` |
| Video Story (9:16) | `30 Sek Kurz - Strom - TV - 9-16 - V1 ohne URL.mp4` |
| Primary Text | 🌱 Strom vom Mühlviertel: Fair, Regional und Grün<br><br>Mia Mühlviertel san ned Deppad! Regios Energiegenossenschaft steht für faire, sichere und nachhaltige Energieversorgung von Bürger:innen, für Bürger:innen.<br><br>✔ Über 2 Mio. € bereits in die Region investiert<br>✔ 18+ Gemeinden & 15 Leitbetriebe dabei<br><br>Stärken wir gemeinsam das Mühlviertel! |
| Headline | UNSERE ENERGIE REGIOS |
| CTA | Learn More |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=facebook&utm_medium=social&utm_campaign=gruenstrom_tofu_alle&utm_content=video30_strom_feed_story` |

---

### Campaign B: Targeting Genossenschaft

**Campaign:** `[Traffic > Auction > Muehviertel > 30+] Genossenschaft`

**Campaign Settings:**

| Setting | Value |
|---------|-------|
| Campaign Objective | Traffic |
| Buying Type | Auction |
| Campaign Budget Optimization | On |
| Campaign Budget | €150 (Lifetime) |
| Campaign Bid Strategy | Lowest cost |

**Ad 1: Genossenschaft 30s (Feed 1:1 + Story 9:16)**

| Field | Content |
|-------|---------|
| Video Feed (1:1) | `30 Sek Kurz - Genossenschaft - TV - 1-1 - V1 ohne URL.mp4` |
| Video Story (9:16) | `30 Sek Kurz - Genossenschaft - TV - 9-16 - V1 ohne URL.mp4` |
| Primary Text | 🤝 Unsere Stabilität, Unsere Sicherheit, Unsere Zukunft, UNSERE ENERGIE REGIOS<br><br>Mia Mühlviertel entscheiden selber wie es uns weitergeht! Regios ist mehr als Strom: Es ist ein Modell für regionale Selbstbestimmung und wirtschaftliche Stabilität.<br><br>✔ Investitionspakete<br>✔ Grünstrom<br>✔ Grüne Pacht<br><br>Mach jetzt gleich mit bei der Energiegenossenschaft! |
| Headline | Investiere in die Stabilität des Mühlviertel |
| CTA | Learn More |
| Website URL | `https://www.regios.at/beteiligung?utm_source=facebook&utm_medium=social&utm_campaign=genossenschaft_tofu_stabilitaet&utm_content=video30_genossenschaft_feed_story` |

---

### Campaign C: Targeting Carousels

**Campaign:** `[Traffic > Auction > Muehviertel > 30+] Carousels`

**Campaign Settings:**

| Setting | Value |
|---------|-------|
| Campaign Objective | Traffic |
| Campaign Budget | €100 (Lifetime) |

**Carousel Ad 1: Sonne**

| Field | Content |
|-------|---------|
| Images | Sonne_1080x1080_1.png through Sonne_1080x1080_5.png |
| Primary Text | ☀️ Unsere Sonne, Unser Mühlviertel, UNSERE ENERGIE REGIOS<br><br>Mia san ned Deppad! Entdecke, wie Sonnenenergie aus der Region unsere Zukunft gestaltet. |
| CTA | Learn More |

| Slide | Image | Headline | Description | URL |
|-------|-------|----------|-------------|-----|
| 1 | Sonne_1080x1080_1.png | Unsere Sonne | Sonnenenergie aus dem Mühlviertel | `...&utm_term=slide_1` |
| 2 | Sonne_1080x1080_2.png | Unser Mühlviertel | Fair, Regional und Grün | `...&utm_term=slide_2` |
| 3 | Sonne_1080x1080_3.png | Unsere Energie | Von Bürger:innen, für Bürger:innen | `...&utm_term=slide_3` |
| 4 | Sonne_1080x1080_4.png | Unsere Zukunft | Über 2 Mio. € investiert | `...&utm_term=slide_4` |
| 5 | Sonne_1080x1080_5.png | UNSERE ENERGIE REGIOS | Jetzt informieren | `...&utm_term=slide_5` |

Base URL: `https://www.regios.at/regionaler-gruenstrom?utm_source=facebook&utm_medium=social&utm_campaign=gruenstrom_tofu_sonne&utm_content=carousel_sonne`

**Carousel Ad 2: Wasser**

| Field | Content |
|-------|---------|
| Images | wasser_1080x1080_1.png through wasser_1080x1080_5.png |
| Primary Text | 💧 Unser Wasser, Unser Mühlviertel, UNSERE ENERGIE REGIOS<br><br>Mia Mühlviertel san ned Deppad! Wasserkraft aus der Region für eine nachhaltige Energiezukunft. |
| CTA | Learn More |

| Slide | Image | Headline | Description | URL |
|-------|-------|----------|-------------|-----|
| 1 | wasser_1080x1080_1.png | Unser Wasser | Wasserkraft aus dem Mühlviertel | `...&utm_term=slide_1` |
| 2 | wasser_1080x1080_2.png | Unser Mühlviertel | Fair, Regional und Grün | `...&utm_term=slide_2` |
| 3 | wasser_1080x1080_3.png | Unsere Energie | Von Bürger:innen, für Bürger:innen | `...&utm_term=slide_3` |
| 4 | wasser_1080x1080_4.png | Unsere Zukunft | 18+ Gemeinden dabei | `...&utm_term=slide_4` |
| 5 | wasser_1080x1080_5.png | UNSERE ENERGIE REGIOS | Jetzt informieren | `...&utm_term=slide_5` |

Base URL: `https://www.regios.at/regionaler-gruenstrom?utm_source=facebook&utm_medium=social&utm_campaign=gruenstrom_tofu_wasser&utm_content=carousel_wasser`

**Carousel Ad 3: Wind**

| Field | Content |
|-------|---------|
| Images | WInd_1080x1080_1.png through WInd_1080x1080_5.png |
| Primary Text | 🌬️ Unser Wind, Unser Mühlviertel, UNSERE ENERGIE REGIOS<br><br>Mia san ned Deppad! Windenergie aus dem Mühlviertel: regional und nachhaltig. |
| CTA | Learn More |

| Slide | Image | Headline | Description | URL |
|-------|-------|----------|-------------|-----|
| 1 | WInd_1080x1080_1.png | Unser Wind | Windenergie aus dem Mühlviertel | `...&utm_term=slide_1` |
| 2 | WInd_1080x1080_2.png | Unser Mühlviertel | Fair, Regional und Grün | `...&utm_term=slide_2` |
| 3 | WInd_1080x1080_3.png | Unsere Energie | Von Bürger:innen, für Bürger:innen | `...&utm_term=slide_3` |
| 4 | WInd_1080x1080_4.png | Unsere Zukunft | 15+ Leitbetriebe dabei | `...&utm_term=slide_4` |
| 5 | WInd_1080x1080_5.png | UNSERE ENERGIE REGIOS | Jetzt informieren | `...&utm_term=slide_5` |

Base URL: `https://www.regios.at/regionaler-gruenstrom?utm_source=facebook&utm_medium=social&utm_campaign=gruenstrom_tofu_wind&utm_content=carousel_wind`

**Carousel Ad 4: Stabilität**

| Field | Content |
|-------|---------|
| Images | Stabilitaet_1080x1080_1.png through Stabilitaet_1080x1080_5.png |
| Primary Text | 🤝 Unsere Stabilität, UNSERE ENERGIE REGIOS<br><br>Mia Mühlviertel entscheiden selber wie es uns weitergeht! Investiere in die wirtschaftliche Stabilität des Mühlviertels. Gemeinsam sind wir stark! |
| CTA | Learn More |

| Slide | Image | Headline | Description | URL |
|-------|-------|----------|-------------|-----|
| 1 | Stabilitaet_1080x1080_1.png | Unsere Stabilität | Wirtschaftliche Sicherheit | `...&utm_term=slide_1` |
| 2 | Stabilitaet_1080x1080_2.png | Unser Mühlviertel | Regionale Selbstbestimmung | `...&utm_term=slide_2` |
| 3 | Stabilitaet_1080x1080_3.png | Unsere Genossenschaft | Gemeinsames Eigentum | `...&utm_term=slide_3` |
| 4 | Stabilitaet_1080x1080_4.png | Unsere Zukunft | Über 2 Mio. € investiert | `...&utm_term=slide_4` |
| 5 | Stabilitaet_1080x1080_5.png | UNSERE ENERGIE REGIOS | Jetzt Mitglied werden | `...&utm_term=slide_5` |

Base URL: `https://www.regios.at/beteiligung?utm_source=facebook&utm_medium=social&utm_campaign=genossenschaft_tofu_stabilitaet&utm_content=carousel_stabilitaet`

**Carousel Ad 5: Zukunft**

| Field | Content |
|-------|---------|
| Images | Zukunft_1080x1080_1.png through Zukunft_1080x1080_5.png |
| Primary Text | 🌱 Unsere Zukunft, UNSERE ENERGIE REGIOS<br><br>Zeigen wir was unser kleines Bauernland drauf hat! Ein Modell für regionale Selbstbestimmung und eine lebenswerte Zukunft. |
| CTA | Learn More |

| Slide | Image | Headline | Description | URL |
|-------|-------|----------|-------------|-----|
| 1 | Zukunft_1080x1080_1.png | Unsere Zukunft | Lebenswerte Region | `...&utm_term=slide_1` |
| 2 | Zukunft_1080x1080_2.png | Unser Mühlviertel | Mia san ned Deppad | `...&utm_term=slide_2` |
| 3 | Zukunft_1080x1080_3.png | Unsere Genossenschaft | Nachhaltige Investition | `...&utm_term=slide_3` |
| 4 | Zukunft_1080x1080_4.png | Unsere Energie | Fair, Regional und Grün | `...&utm_term=slide_4` |
| 5 | Zukunft_1080x1080_5.png | UNSERE ENERGIE REGIOS | Jetzt Mitglied werden | `...&utm_term=slide_5` |

Base URL: `https://www.regios.at/beteiligung?utm_source=facebook&utm_medium=social&utm_campaign=genossenschaft_tofu_zukunft&utm_content=carousel_zukunft`

**Carousel Ad 6: Sicherheit**

| Field | Content |
|-------|---------|
| Images | Sicherheit_1080x1080_1.png through Sicherheit_1080x1080_5.png |
| Primary Text | 🛡️ Unsere Sicherheit, UNSERE ENERGIE REGIOS<br><br>Mia san ned Deppad! Sichere Energieversorgung durch gemeinsames Eigentum. |
| CTA | Learn More |

| Slide | Image | Headline | Description | URL |
|-------|-------|----------|-------------|-----|
| 1 | Sicherheit_1080x1080_1.png | Unsere Sicherheit | Sichere Energieversorgung | `...&utm_term=slide_1` |
| 2 | Sicherheit_1080x1080_2.png | Unser Mühlviertel | Regionale Unabhängigkeit | `...&utm_term=slide_2` |
| 3 | Sicherheit_1080x1080_3.png | Unsere Genossenschaft | Gemeinsames Eigentum | `...&utm_term=slide_3` |
| 4 | Sicherheit_1080x1080_4.png | Unsere Zukunft | Langfristige Stabilität | `...&utm_term=slide_4` |
| 5 | Sicherheit_1080x1080_5.png | UNSERE ENERGIE REGIOS | Jetzt Mitglied werden | `...&utm_term=slide_5` |

Base URL: `https://www.regios.at/beteiligung?utm_source=facebook&utm_medium=social&utm_campaign=genossenschaft_tofu_sicherheit&utm_content=carousel_sicherheit`

---

## 7. Meta Instagram Campaigns

### Campaign A: Targeting Grünstrom (Instagram)

**Campaign:** `[Awareness > Auction > Muehviertel > 30+] IG Gruenstrom`

**Campaign Settings:**

| Setting | Value |
|---------|-------|
| Campaign Objective | Awareness |
| Campaign Budget | €125 (Lifetime) |

**Ad Set Settings:**

| Setting | Value |
|---------|-------|
| Placements | Instagram Feed, Instagram Stories, Instagram Reels |
| Location | Mühlviertel region |
| Age | 30 to 65+ |
| Gender | All |

**Ad 1: Sonne (Feed 1:1 + Story 9:16)**

| Field | Content |
|-------|---------|
| Video Feed (1:1) | `15 Sek Strom - Sonne - Online - 1-1 - V1.mp4` |
| Video Story (9:16) | `15 Sek Strom - Sonne - Online - 9-16 - V3.mp4` |
| Caption | ☀️ Unsere Sonne, Unser Mühlviertel, UNSERE ENERGIE REGIOS<br><br>Strom vom Mühlviertel: Fair, Regional und Grün. 🌱<br><br>Mia san ned Deppad! Über 2 Millionen Euro wurden schon in das Mühlviertel investiert. Stärken wir gemeinsam die Region!<br><br>#regios #mühlviertel #grünstrom #energiegenossenschaft #nachhaltigkeit #sonnenenergie #oberösterreich #miasanneddeppad |
| CTA | Learn More |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=instagram&utm_medium=social&utm_campaign=gruenstrom_tofu_sonne&utm_content=video15_sonne_feed_story` |

**Ad 2: Wasser (Feed 1:1 + Story 9:16)**

| Field | Content |
|-------|---------|
| Video Feed (1:1) | `15 Sek Strom - Wasser - Online - 1-1 - V1.mp4` |
| Video Story (9:16) | `15 Sek Strom - Wasser - Online - 9-16 - V3.mp4` |
| Caption | 💧 Unser Wasser, Unser Mühlviertel, UNSERE ENERGIE REGIOS<br><br>Mia Mühlviertel san ned Deppad! Regionale Wasserkraft für eine nachhaltige Zukunft. 🌱<br><br>Über 18 Gemeinden sind schon dabei!<br><br>#regios #mühlviertel #wasserkraft #energiegenossenschaft #nachhaltigkeit #oberösterreich #miasanneddeppad |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=instagram&utm_medium=social&utm_campaign=gruenstrom_tofu_wasser&utm_content=video15_wasser_feed_story` |

**Ad 3: Wind (Feed 1:1 + Story 9:16)**

| Field | Content |
|-------|---------|
| Video Feed (1:1) | `15 Sek Strom - Wind - Online - 1-1 - V1.mp4` |
| Video Story (9:16) | `15 Sek Strom - Wind - Online - 9-16 - V3.mp4` |
| Caption | 🌬️ Unser Wind, Unser Mühlviertel, UNSERE ENERGIE REGIOS<br><br>Mia san ned Deppad! Windenergie aus der Region, für die Region. 🌱<br><br>15+ Leitbetriebe sind schon dabei!<br><br>#regios #mühlviertel #windenergie #energiegenossenschaft #nachhaltigkeit #oberösterreich #miasanneddeppad |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=instagram&utm_medium=social&utm_campaign=gruenstrom_tofu_wind&utm_content=video15_wind_feed_story` |

**Ad 4: Strom 30s (Feed 1:1 + Story 9:16)**

| Field | Content |
|-------|---------|
| Video Feed (1:1) | `30 Sek Kurz - Strom - TV - 1-1 - V1 ohne URL.mp4` |
| Video Story (9:16) | `30 Sek Kurz - Strom - TV - 9-16 - V1 ohne URL.mp4` |
| Caption | 🌱 UNSERE ENERGIE REGIOS<br><br>Strom vom Mühlviertel: Fair, Regional und Grün.<br><br>Mia Mühlviertel san ned Deppad! Von Bürger:innen, für Bürger:innen. ✔️ Über 2 Mio. € investiert ✔️ 18+ Gemeinden dabei<br><br>Stärken wir gemeinsam das Mühlviertel!<br><br>#regios #energiegenossenschaft #mühlviertel #grünstrom #nachhaltigkeit #miasanneddeppad |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=instagram&utm_medium=social&utm_campaign=gruenstrom_tofu_alle&utm_content=video30_strom_feed_story` |

---

### Campaign B: Targeting Genossenschaft (Instagram)

**Campaign:** `[Traffic > Auction > Muehviertel > 30+] IG Genossenschaft`

**Campaign Settings:**

| Setting | Value |
|---------|-------|
| Campaign Objective | Traffic |
| Campaign Budget | €125 (Lifetime) |

**Ad 1: Genossenschaft 30s (Feed 1:1 + Story 9:16)**

| Field | Content |
|-------|---------|
| Video Feed (1:1) | `30 Sek Kurz - Genossenschaft - TV - 1-1 - V1 ohne URL.mp4` |
| Video Story (9:16) | `30 Sek Kurz - Genossenschaft - TV - 9-16 - V1 ohne URL.mp4` |
| Caption | 🤝 UNSERE ENERGIE REGIOS<br><br>Unsere Stabilität. Unsere Sicherheit. Unsere Zukunft.<br><br>Mia Mühlviertel entscheiden selber wie es uns weitergeht! Regios ist mehr als Strom: Ein Modell für regionale Selbstbestimmung und wirtschaftliche Stabilität.<br><br>Mach jetzt gleich mit bei der Energiegenossenschaft! 🌱<br><br>#regios #genossenschaft #investieren #mühlviertel #nachhaltigkeit #miasanneddeppad |
| CTA | Learn More |
| Website URL | `https://www.regios.at/beteiligung?utm_source=instagram&utm_medium=social&utm_campaign=genossenschaft_tofu_stabilitaet&utm_content=video30_genossenschaft_feed_story` |

**Carousel Ad 1: Sarah (Bürger:in)**

| Field | Content |
|-------|---------|
| Images | Sarah_1080x1080_1.png through sarah_1080x1080_5.png |
| Caption | 👩 Unsere Sarah, Unsere Bürger:in, Unser Mühlviertel, UNSERE ENERGIE REGIOS<br><br>Mia san ned Deppad! Von Bürger:innen, für Bürger:innen. Gemeinsam schaffen wir Stabilität und Zukunft! 🌱<br><br>#regios #mühlviertel #gemeinschaft #energiegenossenschaft #miasanneddeppad |
| CTA | Learn More |

| Slide | Image | Headline | Description | URL |
|-------|-------|----------|-------------|-----|
| 1 | Sarah_1080x1080_1.png | Unsere Sarah | Bürger:in aus dem Mühlviertel | `...&utm_term=slide_1` |
| 2 | Sarah_1080x1080_2.png | Unsere Gemeinschaft | Von Bürger:innen, für Bürger:innen | `...&utm_term=slide_2` |
| 3 | Sarah_1080x1080_3.png | Unser Mühlviertel | Mia san ned Deppad | `...&utm_term=slide_3` |
| 4 | sarah_1080x1080_4.png | Unsere Zukunft | Gemeinsam stark | `...&utm_term=slide_4` |
| 5 | sarah_1080x1080_5.png | UNSERE ENERGIE REGIOS | Jetzt informieren | `...&utm_term=slide_5` |

Base URL: `https://www.regios.at/buerger?utm_source=instagram&utm_medium=social&utm_campaign=genossenschaft_tofu_testimonial&utm_content=carousel_sarah`

**Carousel Ad 2: Susanne (Gemeinde)**

| Field | Content |
|-------|---------|
| Images | susanne_1080x1080_1.png through susanne_1080x1080_5.png |
| Caption | 👩‍💼 Unsere Susanne, Unsere Gemeinde, Unser Mühlviertel, UNSERE ENERGIE REGIOS<br><br>Mia Mühlviertel san ned Deppad! Über 18 Gemeinden sind schon dabei! 🌱<br><br>#regios #mühlviertel #gemeinde #energiegenossenschaft #miasanneddeppad |
| CTA | Learn More |

| Slide | Image | Headline | Description | URL |
|-------|-------|----------|-------------|-----|
| 1 | susanne_1080x1080_1.png | Unsere Susanne | Gemeinde aus dem Mühlviertel | `...&utm_term=slide_1` |
| 2 | susanne_1080x1080_2.png | Unsere Gemeinden | 18+ Gemeinden dabei | `...&utm_term=slide_2` |
| 3 | susanne_1080x1080_3.png | Unser Mühlviertel | Regionale Partnerschaft | `...&utm_term=slide_3` |
| 4 | susanne_1080x1080_4.png | Unsere Zukunft | Gemeinsam stark | `...&utm_term=slide_4` |
| 5 | susanne_1080x1080_5.png | UNSERE ENERGIE REGIOS | Jetzt informieren | `...&utm_term=slide_5` |

Base URL: `https://www.regios.at/gemeinde?utm_source=instagram&utm_medium=social&utm_campaign=genossenschaft_tofu_testimonial&utm_content=carousel_susanne`

**Carousel Ad 3: Christian (Bank/Unternehmen)**

| Field | Content |
|-------|---------|
| Images | christain_1080x1080_1.png through christain_1080x1080_5.png |
| Caption | 🏦 Unser Christian, Unser Partner, Unser Mühlviertel, UNSERE ENERGIE REGIOS<br><br>Mia san ned Deppad! Banken und Unternehmen als starke Partner für die Region. 🌱<br><br>#regios #mühlviertel #partnerschaft #energiegenossenschaft #miasanneddeppad |
| CTA | Learn More |

| Slide | Image | Headline | Description | URL |
|-------|-------|----------|-------------|-----|
| 1 | christain_1080x1080_1.png | Unser Christian | Partner aus dem Mühlviertel | `...&utm_term=slide_1` |
| 2 | christain_1080x1080_2.png | Unsere Partner | Banken als Entwicklungspartner | `...&utm_term=slide_2` |
| 3 | christain_1080x1080_3.png | Unser Mühlviertel | Vertrauen und Transparenz | `...&utm_term=slide_3` |
| 4 | christain_1080x1080_4.png | Unsere Zukunft | Nachhaltige Investition | `...&utm_term=slide_4` |
| 5 | christain_1080x1080_5.png | UNSERE ENERGIE REGIOS | Jetzt informieren | `...&utm_term=slide_5` |

Base URL: `https://www.regios.at/bank?utm_source=instagram&utm_medium=social&utm_campaign=genossenschaft_tofu_testimonial&utm_content=carousel_christian`

**Carousel Ad 4: Martin (Grundbesitzer)**

| Field | Content |
|-------|---------|
| Images | Martin_1080x1080_1.png through Martin_1080x1080_5.png |
| Caption | 🌾 Unser Martin, Unser Grundbesitzer, Unser Mühlviertel, UNSERE ENERGIE REGIOS<br><br>Mia Mühlviertel san ned Deppad! Grüne Pacht für Grundbesitzer:innen! 🌱<br><br>#regios #mühlviertel #grundbesitzer #energiegenossenschaft #miasanneddeppad |
| CTA | Learn More |

| Slide | Image | Headline | Description | URL |
|-------|-------|----------|-------------|-----|
| 1 | Martin_1080x1080_1.png | Unser Martin | Grundbesitzer aus dem Mühlviertel | `...&utm_term=slide_1` |
| 2 | Martin_1080x1080_2.png | Unsere Grundbesitzer | Grüne Pacht | `...&utm_term=slide_2` |
| 3 | Martin_1080x1080_3.png | Unser Mühlviertel | Regionale Wertschöpfung | `...&utm_term=slide_3` |
| 4 | Martin_1080x1080_4.png | Unsere Zukunft | Gemeinsam stark | `...&utm_term=slide_4` |
| 5 | Martin_1080x1080_5.png | UNSERE ENERGIE REGIOS | Jetzt informieren | `...&utm_term=slide_5` |

Base URL: `https://www.regios.at/grundbesitzer?utm_source=instagram&utm_medium=social&utm_campaign=genossenschaft_tofu_testimonial&utm_content=carousel_martin`

**Carousel Ad 5: Klaus (Unternehmer)**

| Field | Content |
|-------|---------|
| Images | Klaus_1080x1080_1.png through Klaus_1080x1080_5.png |
| Caption | 👨‍💼 Unser Klaus, Unser Unternehmer, Unser Mühlviertel, UNSERE ENERGIE REGIOS<br><br>Mia san ned Deppad! Regionale Wertschöpfung und stabile Preisentwicklung. 🌱<br><br>#regios #mühlviertel #unternehmer #energiegenossenschaft #miasanneddeppad |
| CTA | Learn More |

| Slide | Image | Headline | Description | URL |
|-------|-------|----------|-------------|-----|
| 1 | Klaus_1080x1080_1.png | Unser Klaus | Unternehmer aus dem Mühlviertel | `...&utm_term=slide_1` |
| 2 | Klaus_1080x1080_2.png | Unsere Unternehmer | Regionale Wertschöpfung | `...&utm_term=slide_2` |
| 3 | Klaus_1080x1080_3.png | Unser Mühlviertel | Stabile Preisentwicklung | `...&utm_term=slide_3` |
| 4 | Klaus_1080x1080_4.png | Unsere Zukunft | Unabhängigkeit & Selbstgestaltung | `...&utm_term=slide_4` |
| 5 | Klaus_1080x1080_5.png | UNSERE ENERGIE REGIOS | Jetzt informieren | `...&utm_term=slide_5` |

Base URL: `https://www.regios.at/unternehmer?utm_source=instagram&utm_medium=social&utm_campaign=genossenschaft_tofu_testimonial&utm_content=carousel_klaus`

---

## 8. Meta Retargeting Campaigns

**Note:** Google Display Retargeting is covered in Section 4 with all HTML5 banner assets and UTM URLs.

### Campaign: Meta Retargeting
`[Leads > Auction > Retargeting] Meta Retargeting`

**Campaign Settings:**

| Setting | Value |
|---------|-------|
| Campaign Objective | Leads |
| Conversion Location | Website |
| Conversion Event | FormSubmitBeteiligung (Custom Event) |
| Campaign Budget | €310 (Lifetime) Split: €200 Facebook, €110 Instagram |
| Bid Strategy | Lowest cost per lead |

**⚠️ Conversion Event Note:**
Use **FormSubmitBeteiligung** as the primary conversion event. Form submissions are clearer intent signals than clicks. We exclude EmailClick and ClickOurPower events because these lead users off-site and we cannot verify if they actually convert on external platforms (email client, OurPower website).

**Custom Audiences to Use:**
1. Engagement: Paid Meta Ads (180 days)
2. Engagement: Meta Organic (180 days)
3. Engagement: Instagram/Facebook Subscription
4. Engagement: Messenger Contact
5. Website Visitors (via Pixel) 30 days

---


## FACEBOOK RETARGETING ADS

**Asset Base Path:** `Final Assets/Social Media/Retargeting/Video/Retargeting/Meta All/`

### Ad Set 1a: Facebook - Testimonial Videos (Feed + Story)

**Placements:** Facebook Feed, Facebook Stories, Facebook Reels

**Purpose:** Individual testimonial videos with Feed (1:1) + Story (9:16) format combinations.

**UTM Structure:** `utm_source=facebook&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial&utm_content=[name]&utm_term=[topic]`

---

#### Sarah (Bürger:in) - 11 Ads

**Asset Paths:**
- Feed (1:1): `Testimonial - Sarah/Sarah 1_1 mit Abbinder/`
- Story (9:16): `Testimonial - Sarah/Sarah 9_16 mit Abbinder/`

| Ad | Topic | Video Feed (1:1) | Video Story (9:16) | utm_term |
|----|-------|------------------|-------------------|----------|
| 1 | Vorstellung | `Testimonial - Sarah - 1-1 - Short - mit Abbinder - Vorstellung.mp4` | `Testimonial - Sarah - 9-16 - Short - mit Abbinder - Vorstellung.mp4` | `vorstellung` |
| 2 | Warum Regios | `Testimonial - Sarah - 1-1 - Short - mit Abbinder - Warum Regios.mp4` | `Testimonial - Sarah - 9-16 - Short - mit Abbinder - Warum Regios.mp4` | `warum_regios` |
| 3 | Wertschöpfung in der Region | `Testimonial - Sarah - 1-1 - Short - mit Abbinder - Wertschöpfung in der Region.mp4` | `Testimonial - Sarah - 9-16 - Short - mit Abbinder - Wertschöpfung in der Region.mp4` | `wertschoepfung` |
| 4 | Gemeinsam Stark | `Testimonial - Sarah - 1-1 - Short - mit Abbinder - Gemeinsam Stark.mp4` | `Testimonial - Sarah - 9-16 - Short - mit Abbinder - Gemeinsam Stark.mp4` | `gemeinsam_stark` |
| 5 | Produkte | `Testimonial - Sarah - 1-1 - Short - mit Abbinder - Produkte.mp4` | `Testimonial - Sarah - 9-16 - Short - mit Abbinder - Produkte.mp4` | `produkte` |
| 6 | Persönlicher Ansprechpartner | `Testimonial - Sarah - 1-1 - Short - mit Abbinder - Persönlicher Ansprechpartner.mp4` | `Testimonial - Sarah - 9-16 - Short - mit Abbinder - Persönlicher Ansprechpartner.mp4` | `ansprechpartner` |
| 7 | Wirkungskraft | `Testimonial - Sarah - 1-1 - Short - mit Abbinder - Wirkungskraft.mp4` | `Testimonial - Sarah - 9-16 - Short - mit Abbinder - Wirkungskraft.mp4` | `wirkungskraft` |
| 8 | Wie auf Regios gekommen | `Testimonial - Sarah - 1-1 - Short - mit Abbinder - Wie auf Regios gekommen.mp4` | `Testimonial - Sarah - 9-16 - Short - mit Abbinder - Wie auf Regios gekommen.mp4` | `wie_gekommen` |
| 9 | Risiko oder Chance | `Testimonial - Sarah - 1-1 - Short - mit Abbinder - Risiko oder Chance.mp4` | `Testimonial - Sarah - 9-16 - Short - mit Abbinder - Risiko oder Chance.mp4` | `risiko_chance` |
| 10 | Zweifel | `Testimonial - Sarah - 1-1 - Short - mit Abbinder - Zweifel.mp4` | `Testimonial - Sarah - 9-16 - Short - mit Abbinder - Zweifel.mp4` | `zweifel` |
| 11 | Was ist wichtig | `Testimonial - Sarah - 1-1 - Short  - mit Abbinder- ws ist wichtig.mp4` | `Testimonial - Sarah - 9-16 - Short - mit Abbinder - ws ist wichtig.mp4` | `was_wichtig` |

**Primary Text:** 👩 Sarah aus dem Mühlviertel erzählt: „[Topic]"<br><br>Unsere Sarah, Unsere Gemeinschaft, UNSERE ENERGIE REGIOS<br><br>Mia san ned Deppad!

**Base URL:** `https://www.regios.at/buerger?utm_source=facebook&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial&utm_content=sarah`

**CTA:** Learn More

---

#### Peter (Grundbesitzer) - 7 Ads

**Asset Paths:**
- Feed (1:1): `Testimonial - Peter/Peter 1_1 mit Abbinder/`
- Story (9:16): `Testimonial - Peter/Peter 9_16 mit Abbinder/`

| Ad | Topic | Video Feed (1:1) | Video Story (9:16) | utm_term |
|----|-------|------------------|-------------------|----------|
| 1 | Vorstellung | `Testimonial - Peter - 1-1 - Short - mit Abbinder - Vorstellung.mp4` | `Testimonial - Peter - 9-16 - Short - mit Abbinder - Vorstellung.mp4` | `vorstellung` |
| 2 | Wie kennengelernt | `Testimonial - Peter - 1-1 - Short - mit Abbinder - wie kennengelernt.mp4` | `Testimonial - Peter - 9-16 - Short - mit Abbinder - wie kennengelernt.mp4` | `kennengelernt` |
| 3 | Doppelnutzung | `Testimonial - Peter - 1-1 - Short - mit Abbinder - Doppelnutzung.mp4` | `Testimonial - Peter - 9-16 - Short - mit Abbinder - Doppelnutzung.mp4` | `doppelnutzung` |
| 4 | Selbstversorger | `Testimonial - Peter - 1-1 - Short - mit Abbinder - Selbstversorger.mp4` | `Testimonial - Peter - 9-16 - Short - mit Abbinder - Selbstversorger.mp4` | `selbstversorger` |
| 5 | Weiteres Standbein | `Testimonial - Peter - 1-1 - Short - mit Abbinder - weiteres Standbein.mp4` | `Testimonial - Peter - 9-16 - Short - mit Abbinder - weiteres Standbein.mp4` | `standbein` |
| 6 | Regionale Energieversorgung | `Testimonial - Peter - 1-1 - Short - mit Abbinder - regionale Energieversorgung.mp4` | `Testimonial - Peter - 9-16 - Short - mit Abbinder - regionale Energieversorgung.mp4` | `energieversorgung` |
| 7 | Risiko oder Chance | `Testimonial - Peter - 1-1 - Short - mit Abbinder - Risiko oder Chance.mp4` | `Testimonial - Peter - 9-16 - Short - mit Abbinder - Risiko oder Chance.mp4` | `risiko_chance` |

**Primary Text:** 👨‍🌾 Peter, Grundbesitzer aus dem Mühlviertel: „[Topic]"<br><br>Unser Peter, Unsere Bauern, UNSERE ENERGIE REGIOS<br><br>Zeigen wir was unser kleines Bauernland drauf hat!

**Base URL:** `https://www.regios.at/grundbesitzer?utm_source=facebook&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial&utm_content=peter`

**CTA:** Learn More

---

#### Susanne (Gemeinde) - 10 Ads

**Asset Paths:**
- Feed (1:1): `Testimonial - Susanne/Susanne 1_1 mit Abbinder/`
- Story (9:16): `Testimonial - Susanne/Susanne 9_16 mit Abbinder/`

| Ad | Topic | Video Feed (1:1) | Video Story (9:16) | utm_term |
|----|-------|------------------|-------------------|----------|
| 1 | Vorstellung | `Testimonial - Susanne - 1-1 - Short - mit Abbinder - Vorstellung.mp4` | `Testimonial - Susanne - 9-16 - Short - mit Abbinder - Vorstellung.mp4` | `vorstellung` |
| 2 | Warum Regios | `Testimonial - Susanne - 1-1 - Short - mit Abbinder - Warum Regios.mp4` | `Testimonial - Susanne - 9-16 - Short - mit Abbinder - Warum Regios.mp4` | `warum_regios` |
| 3 | USP | `Testimonial - Susanne - 1-1 - Short - mit Abbinder - USP.mp4` | `Testimonial - Susanne - 9-16 - Short - mit Abbinder - USP.mp4` | `usp` |
| 4 | Sichtbare Veränderung | `Testimonial - Susanne - 1-1 - Short - mit Abbinder - Sichtbare Veränderung.mp4` | `Testimonial - Susanne - 9-16 - Short - mit Abbinder - Sichtbare Veränderung.mp4` | `veraenderung` |
| 5 | Gemeinsames Eigentum | `Testimonial - Susanne - 1-1 - Short - mit Abbinder - gemeinsames Eigentum.mp4` | `Testimonial - Susanne - 9-16 - Short - mit Abbinder - gemeinsames Eigentum.mp4` | `eigentum` |
| 6 | Regios wichtiger Partner | `Testimonial - Susanne - 1-1 - Short - mit Abbinder - Regios wichtiger Partner für Energie.mp4` | `Testimonial - Susanne - 9-16 - Short - mit Abbinder - Regios wichtiger Partner für Energie.mp4` | `partner` |
| 7 | Erreichbarkeit | `Testimonial - Susanne - 1-1 - Short - mit Abbinder - Erreichbarkeit.mp4` | `Testimonial - Susanne - 9-16 - Short - mit Abbinder - Erreichbarkeit.mp4` | `erreichbarkeit` |
| 8 | Risiko oder Chance | `Testimonial - Susanne - 1-1 - Short - mit Abbinder - Riskio oder Chance.mp4` | `Testimonial - Susanne - 9-16 - Short - mit Abbinder - Riskio oder Chance.mp4` | `risiko_chance` |
| 9 | Vertrauen | `Testimonial - Susanne - 1-1 - Short  - mit Abbinder - Vertrauen.mp4` | `Testimonial - Susanne - 9-16 - Short - mit Abbinder - Vertrauen.mp4` | `vertrauen` |
| 10 | Danke | `Testimonial - Susanne - 1-1 - Short - mit Abbinder - Danke.mp4` | `Testimonial - Susanne - 9-16 - Short - mit Abbinder - Danke.mp4` | `danke` |

**Primary Text:** 👩‍💼 Susanne, Gemeindevertreterin: „[Topic]"<br><br>Unsere Susanne, Unsere Gemeinden, UNSERE ENERGIE REGIOS<br><br>Über 18 Gemeinden sind schon dabei!

**Base URL:** `https://www.regios.at/gemeinde?utm_source=facebook&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial&utm_content=susanne`

**CTA:** Learn More

---

#### Norbert (Bürger) - 10 Ads

**Asset Paths:**
- Feed (1:1): `Testimonial - Norbert/Norbert 1_1 mit Abbinder/`
- Story (9:16): `Testimonial - Norbert/Norbert 9_16 mit Abbinder/`

| Ad | Topic | Video Feed (1:1) | Video Story (9:16) | utm_term |
|----|-------|------------------|-------------------|----------|
| 1 | Vorstellung | `Testimonial - Norbert - 1-1 - Short - mit Abbinder - Vorstellung.mp4` | `Testimonial - Norbert - 9-16 - Short - mit Abbinder - Vorstellung.mp4` | `vorstellung` |
| 2 | Sicherheit | `Testimonial - Norbert - 1-1 - Short - mit Abbinder - Sicherheit.mp4` | `Testimonial - Norbert - 9-16 - Short - mit Abbinder - Sicherheit.mp4` | `sicherheit` |
| 3 | Transparenz | `Testimonial - Norbert - 1-1 - Short - mit Abbinder - Transparenz.mp4` | `Testimonial - Norbert - 9-16 - Short - mit Abbinder - Transparenz.mp4` | `transparenz` |
| 4 | Vertrauen | `Testimonial - Norbert - 1-1 - Short - mit Abbinder - Vertrauen.mp4` | `Testimonial - Norbert - 9-16 - Short - mit Abbinder - Vertrauen.mp4` | `vertrauen` |
| 5 | Nachhaltigkeit | `Testimonial - Norbert - 1-1 - Short - mit Abbinder - Nachhaltigkeit.mp4` | `Testimonial - Norbert - 9-16 - Short - mit Abbinder - Nachhaltigkeit.mp4` | `nachhaltigkeit` |
| 6 | Banken als Partner | `Testimonial - Norbert - 1-1 - Short - mit Abbinder - Banken als Partner.mp4` | `Testimonial - Norbert - 9-16 - Short - mit Abbinder - Banken als Partner.mp4` | `banken_partner` |
| 7 | Wirkungskraft | `Testimonial - Norbert - 1-1 - Short - mit Abbinder - Wirkungskraft.mp4` | `Testimonial - Norbert - 9-16 - Short - mit Abbinder - Wirkungskraft.mp4` | `wirkungskraft` |
| 8 | Erreichbarkeit | `Testimonial - Norbert - 1-1 - Short - mit Abbinder - Erreichbarkeit.mp4` | `Testimonial - Norbert - 9-16 - Short - mit Abbinder - Erreichbarkeit.mp4` | `erreichbarkeit` |
| 9 | Risiko | `Testimonial - Norbert - 1-1 - Short - mit Abbinder - Risiko.mp4` | `Testimonial - Norbert - 9-16 - Short - mit Abbinder - Risiko.mp4` | `risiko` |
| 10 | Risiko oder Chance | `Testimonial - Norbert - 1-1 - Short - mit Abbinder - Risiko oder Chance.mp4` | `Testimonial - Norbert - 9-16 - Short - mit Abbinder - Risiko oder Chance.mp4` | `risiko_chance` |

**Primary Text:** 👨 Norbert aus dem Mühlviertel: „[Topic]"<br><br>Unser Norbert, Unsere Sicherheit, UNSERE ENERGIE REGIOS<br><br>Mia san ned Deppad!

**Base URL:** `https://www.regios.at/buerger?utm_source=facebook&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial&utm_content=norbert`

**CTA:** Learn More

---

#### Christian (Bank) - 19 Ads

**Asset Paths:**
- Feed (1:1): `Testimonial - Christian/1_1/`
- Story (9:16): `Testimonial - Christian/9_16/`

| Ad | Topic | Video Feed (1:1) | Video Story (9:16) | utm_term |
|----|-------|------------------|-------------------|----------|
| 1 | Vorstellung | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Vorstellung.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Vorstellung.mp4` | `vorstellung` |
| 2 | Bank als Entwicklungspartner | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Bank als Entwicklungspartner.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Bank als Entwicklungspartner.mp4` | `entwicklungspartner` |
| 3 | Banken und öffentliche Hand | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Banken und öffentliche Hand.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Banken und öffentliche Hand.mp4` | `oeffentliche_hand` |
| 4 | Fossiler zu erneuerbar | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Fossiler zu erneuerbar.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Fossiler zu erneuerbar.mp4` | `erneuerbar` |
| 5 | Gfrei und Sichtbar | `Testimonial - Christian - 1-1 - Short - mit Abbinder- Gfrei- und Sichtbar.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Gfrei- und Sichtbar.mp4` | `gfrei_sichtbar` |
| 6 | Integration | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Integration.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Integration.mp4` | `integration` |
| 7 | Investition Energie | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Investition Energie.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Investition Energie.mp4` | `investition` |
| 8 | Langfristigkeit als Erfolgsmodell | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Langfristigkei als Erfolgsmodell.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Langfristigkei als Erfolgsmodell.mp4` | `erfolgsmodell` |
| 9 | Langfristigkeit | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Langfristigkeit.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Langfristigkeit.mp4` | `langfristigkeit` |
| 10 | Nachhaltigkeit | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Nachhaltigkeit.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Nachhaltigkeit.mp4` | `nachhaltigkeit` |
| 11 | Prinzip Genossenschaft | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Prinzip Genossenschaft.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Prinzip Genossenschaft.mp4` | `prinzip` |
| 12 | Regios als langfristiges Modell | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Regios als langfristiges Modell.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Regios als langfristiges Modell.mp4` | `langfristiges_modell` |
| 13 | Sicherheit Stabilität | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Sicherheit Stabilität.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Sicherheit Stabilität.mp4` | `sicherheit_stabilitaet` |
| 14 | Struktur Aufstellung | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Struktur Aufstellung.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Struktur Aufstellung.mp4` | `struktur` |
| 15 | Transparenz | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Transparenz.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Transparenz.mp4` | `transparenz` |
| 16 | Vertrauen | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Vertrauen.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Vertrauen.mp4` | `vertrauen` |
| 17 | Wirkungskraft | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Wirkungskraft.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Wirkungskraft.mp4` | `wirkungskraft` |
| 18 | Geprüfte Produkte | `Testimonial - Christian - 1-1 - Short - mit Abbinder - geprüfte Produkte.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - geprüfte Produkte.mp4` | `produkte` |
| 19 | Greifbare Kommunikation | `Testimonial - Christian - 1-1 - Short - mit Abbinder - greifbare Kommunikation.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - greifbare Kommunikation.mp4` | `kommunikation` |

**Primary Text:** 🏦 Christian, Bankpartner: „[Topic]"<br><br>Unser Christian, Unsere Partner, UNSERE ENERGIE REGIOS<br><br>Banken als Entwicklungspartner!

**Base URL:** `https://www.regios.at/bank?utm_source=facebook&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial&utm_content=christian`

**CTA:** Learn More

---

#### Klaus (Unternehmer) - 12 Ads

**Asset Paths:**
- Feed (1:1): `Testimonial - Klaus/Klaus 1_1 mit Abbinder/`
- Story (9:16): `Testimonial - Klaus/Klaus 9_16 mit Abbinder/`

| Ad | Topic | Video Feed (1:1) | Video Story (9:16) | utm_term |
|----|-------|------------------|-------------------|----------|
| 1 | Vorstellung | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - Vorstellung.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - Vorstellung.mp4` | `vorstellung` |
| 2 | Kompetenz Regios | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - Kompetenz Regios.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - Kompetenz Regios.mp4` | `kompetenz` |
| 3 | Regionale Wertschöpfung | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - regionale Wertschöpfung.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - regionale Wertschöpfung.mp4` | `wertschoepfung` |
| 4 | Stabile Preisentwicklung | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - stabile Preisentwicklung.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - stabile Preisentwicklung.mp4` | `preisentwicklung` |
| 5 | Unabhängigkeit Selbstgestaltung | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - Unabhängigkeit Selbstgestaltung.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - Unabhängigkeit Selbstgestaltung.mp4` | `unabhaengigkeit` |
| 6 | Verantwortung der Region | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - Verantwortung der Region.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - Verantwortung der Region.mp4` | `verantwortung` |
| 7 | Vertrauen | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - Vertrauen.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - Vertrauen.mp4` | `vertrauen` |
| 8 | Transparenz | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - Transparenz.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - Transparenz.mp4` | `transparenz` |
| 9 | Langfristigkeit | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - Langfristigkeit.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - Langfristigkeit.mp4` | `langfristigkeit` |
| 10 | Wirkungskraft | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - Wirkungskraft.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - Wirkungskraft.mp4` | `wirkungskraft` |
| 11 | Energiekosten | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - Energiekosten.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - Energiekosten.mp4` | `energiekosten` |
| 12 | Vorbild Regios | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - Vorbild Regios.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - Vorbild Regios.mp4` | `vorbild` |

**Primary Text:** 👨‍💼 Klaus, Unternehmer: „[Topic]"<br><br>Unser Klaus, Unsere Unternehmer, UNSERE ENERGIE REGIOS<br><br>Regionale Wertschöpfung!

**Base URL:** `https://www.regios.at/unternehmer?utm_source=facebook&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial&utm_content=klaus`

**CTA:** Learn More

---

### Ad Set 2a: Facebook - Long Videos

**Placements:** Facebook Feed, Facebook Video Feeds

**Purpose:** Full-length interviews for users who prefer complete stories.

**Asset Path:** `Final Assets/Social Media/Retargeting/Video/Retargeting/Meta All/`

| Ad | Person | Video (16:9) | Landing Page | Full URL |
|----|--------|--------------|--------------|----------|
| 1 | Sarah | `Testimonial - Sarah/Sarah 16_9 mit Abbinder/Testimonial - Sarah - Long - V1.mp4` | /buerger | `https://www.regios.at/buerger?utm_source=facebook&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial&utm_content=sarah&utm_term=long` |
| 2 | Peter | `Testimonial - Peter/Peter 16_9 mit Abbinder/Testimonial - Peter - Long - V1.mp4` | /grundbesitzer | `https://www.regios.at/grundbesitzer?utm_source=facebook&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial&utm_content=peter&utm_term=long` |
| 3 | Susanne | `Testimonial - Susanne/Susanne 16_9 mit Abbinder/Testimonial - Susanne - Long - mit Abbinder - V1.mp4` | /gemeinde | `https://www.regios.at/gemeinde?utm_source=facebook&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial&utm_content=susanne&utm_term=long` |
| 4 | Klaus | `Testimonial - Klaus/Klaus 16_9 mit Abbinder/Testimonial - Klaus - Long - mit Abbinder - V1.mp4` | /unternehmer | `https://www.regios.at/unternehmer?utm_source=facebook&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial&utm_content=klaus&utm_term=long` |

**Primary Text Template:** 👤 [Name] aus dem Mühlviertel: Das ganze Interview<br><br>UNSERE ENERGIE REGIOS<br><br>Mia san ned Deppad! Erfahre die komplette Geschichte.

**CTA:** Learn More

---

### Ad Set 3a: Facebook - Image Carousels

**Placements:** Facebook Feed

**Purpose:** Static image carousels for users who engaged but haven't converted.

---

**Carousel 1: Grünstrom Elements**

| Field | Content |
|-------|---------|
| Images | Sonne, Wasser, Wind carousels mixed |
| Primary Text | 🌱 Du hast dich schon über Regios informiert. Jetzt ist der richtige Zeitpunkt!<br><br>Unser Wasser, Unsere Sonne, Unser Wind, UNSERE ENERGIE REGIOS<br><br>Mia san ned Deppad! |
| CTA | Learn More |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=facebook&utm_medium=retargeting&utm_campaign=gruenstrom_mofu_retargeting&utm_content=carousel&utm_term=elements` |

---

**Carousel 2: Genossenschaft Values**

| Field | Content |
|-------|---------|
| Images | Stabilitaet, Zukunft, Sicherheit carousels mixed |
| Primary Text | 🤝 Bereit für den nächsten Schritt?<br><br>Unsere Stabilität, Unsere Sicherheit, Unsere Zukunft, UNSERE ENERGIE REGIOS<br><br>Mia Mühlviertel entscheiden selber wie es uns weitergeht! Investiere in die Stabilität des Mühlviertel! |
| CTA | Learn More |
| Website URL | `https://www.regios.at/beteiligung?utm_source=facebook&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_retargeting&utm_content=carousel&utm_term=values` |

---

## INSTAGRAM RETARGETING ADS

**Asset Base Path:** `Final Assets/Social Media/Retargeting/Video/Retargeting/Meta All/`

### Ad Set 1b: Instagram - Testimonial Videos (Feed + Story/Reels)

**Placements:** Instagram Feed, Instagram Stories, Instagram Reels

**Purpose:** Individual testimonial videos with Feed (1:1) + Story/Reels (9:16) format combinations.

**UTM Structure:** `utm_source=instagram&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial&utm_content=[name]&utm_term=[topic]`

---

#### Sarah (Bürger:in) - 11 Ads

**Asset Paths:**
- Feed (1:1): `Testimonial - Sarah/Sarah 1_1 mit Abbinder/`
- Story (9:16): `Testimonial - Sarah/Sarah 9_16 mit Abbinder/`

| Ad | Topic | Video Feed (1:1) | Video Story (9:16) | utm_term |
|----|-------|------------------|-------------------|----------|
| 1 | Vorstellung | `Testimonial - Sarah - 1-1 - Short - mit Abbinder - Vorstellung.mp4` | `Testimonial - Sarah - 9-16 - Short - mit Abbinder - Vorstellung.mp4` | `vorstellung` |
| 2 | Warum Regios | `Testimonial - Sarah - 1-1 - Short - mit Abbinder - Warum Regios.mp4` | `Testimonial - Sarah - 9-16 - Short - mit Abbinder - Warum Regios.mp4` | `warum_regios` |
| 3 | Wertschöpfung in der Region | `Testimonial - Sarah - 1-1 - Short - mit Abbinder - Wertschöpfung in der Region.mp4` | `Testimonial - Sarah - 9-16 - Short - mit Abbinder - Wertschöpfung in der Region.mp4` | `wertschoepfung` |
| 4 | Gemeinsam Stark | `Testimonial - Sarah - 1-1 - Short - mit Abbinder - Gemeinsam Stark.mp4` | `Testimonial - Sarah - 9-16 - Short - mit Abbinder - Gemeinsam Stark.mp4` | `gemeinsam_stark` |
| 5 | Produkte | `Testimonial - Sarah - 1-1 - Short - mit Abbinder - Produkte.mp4` | `Testimonial - Sarah - 9-16 - Short - mit Abbinder - Produkte.mp4` | `produkte` |
| 6 | Persönlicher Ansprechpartner | `Testimonial - Sarah - 1-1 - Short - mit Abbinder - Persönlicher Ansprechpartner.mp4` | `Testimonial - Sarah - 9-16 - Short - mit Abbinder - Persönlicher Ansprechpartner.mp4` | `ansprechpartner` |
| 7 | Wirkungskraft | `Testimonial - Sarah - 1-1 - Short - mit Abbinder - Wirkungskraft.mp4` | `Testimonial - Sarah - 9-16 - Short - mit Abbinder - Wirkungskraft.mp4` | `wirkungskraft` |
| 8 | Wie auf Regios gekommen | `Testimonial - Sarah - 1-1 - Short - mit Abbinder - Wie auf Regios gekommen.mp4` | `Testimonial - Sarah - 9-16 - Short - mit Abbinder - Wie auf Regios gekommen.mp4` | `wie_gekommen` |
| 9 | Risiko oder Chance | `Testimonial - Sarah - 1-1 - Short - mit Abbinder - Risiko oder Chance.mp4` | `Testimonial - Sarah - 9-16 - Short - mit Abbinder - Risiko oder Chance.mp4` | `risiko_chance` |
| 10 | Zweifel | `Testimonial - Sarah - 1-1 - Short - mit Abbinder - Zweifel.mp4` | `Testimonial - Sarah - 9-16 - Short - mit Abbinder - Zweifel.mp4` | `zweifel` |
| 11 | Was ist wichtig | `Testimonial - Sarah - 1-1 - Short  - mit Abbinder- ws ist wichtig.mp4` | `Testimonial - Sarah - 9-16 - Short - mit Abbinder - ws ist wichtig.mp4` | `was_wichtig` |

**Caption:** 👩 Sarah aus dem Mühlviertel erzählt: „[Topic]"<br><br>Unsere Sarah, Unsere Gemeinschaft, UNSERE ENERGIE REGIOS 🌱<br><br>#regios #mühlviertel #testimonial #energiegenossenschaft #miasanneddeppad

**Base URL:** `https://www.regios.at/buerger?utm_source=instagram&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial&utm_content=sarah`

**CTA:** Learn More

---

#### Peter (Grundbesitzer) - 7 Ads

**Asset Paths:**
- Feed (1:1): `Testimonial - Peter/Peter 1_1 mit Abbinder/`
- Story (9:16): `Testimonial - Peter/Peter 9_16 mit Abbinder/`

| Ad | Topic | Video Feed (1:1) | Video Story (9:16) | utm_term |
|----|-------|------------------|-------------------|----------|
| 1 | Vorstellung | `Testimonial - Peter - 1-1 - Short - mit Abbinder - Vorstellung.mp4` | `Testimonial - Peter - 9-16 - Short - mit Abbinder - Vorstellung.mp4` | `vorstellung` |
| 2 | Wie kennengelernt | `Testimonial - Peter - 1-1 - Short - mit Abbinder - wie kennengelernt.mp4` | `Testimonial - Peter - 9-16 - Short - mit Abbinder - wie kennengelernt.mp4` | `kennengelernt` |
| 3 | Doppelnutzung | `Testimonial - Peter - 1-1 - Short - mit Abbinder - Doppelnutzung.mp4` | `Testimonial - Peter - 9-16 - Short - mit Abbinder - Doppelnutzung.mp4` | `doppelnutzung` |
| 4 | Selbstversorger | `Testimonial - Peter - 1-1 - Short - mit Abbinder - Selbstversorger.mp4` | `Testimonial - Peter - 9-16 - Short - mit Abbinder - Selbstversorger.mp4` | `selbstversorger` |
| 5 | Weiteres Standbein | `Testimonial - Peter - 1-1 - Short - mit Abbinder - weiteres Standbein.mp4` | `Testimonial - Peter - 9-16 - Short - mit Abbinder - weiteres Standbein.mp4` | `standbein` |
| 6 | Regionale Energieversorgung | `Testimonial - Peter - 1-1 - Short - mit Abbinder - regionale Energieversorgung.mp4` | `Testimonial - Peter - 9-16 - Short - mit Abbinder - regionale Energieversorgung.mp4` | `energieversorgung` |
| 7 | Risiko oder Chance | `Testimonial - Peter - 1-1 - Short - mit Abbinder - Risiko oder Chance.mp4` | `Testimonial - Peter - 9-16 - Short - mit Abbinder - Risiko oder Chance.mp4` | `risiko_chance` |

**Caption:** 👨‍🌾 Peter, Grundbesitzer aus dem Mühlviertel: „[Topic]"<br><br>Unser Peter, Unsere Bauern, UNSERE ENERGIE REGIOS 🌱<br><br>#regios #mühlviertel #landwirtschaft #energiegenossenschaft #miasanneddeppad

**Base URL:** `https://www.regios.at/grundbesitzer?utm_source=instagram&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial&utm_content=peter`

**CTA:** Learn More

---

#### Susanne (Gemeinde) - 10 Ads

**Asset Paths:**
- Feed (1:1): `Testimonial - Susanne/Susanne 1_1 mit Abbinder/`
- Story (9:16): `Testimonial - Susanne/Susanne 9_16 mit Abbinder/`

| Ad | Topic | Video Feed (1:1) | Video Story (9:16) | utm_term |
|----|-------|------------------|-------------------|----------|
| 1 | Vorstellung | `Testimonial - Susanne - 1-1 - Short - mit Abbinder - Vorstellung.mp4` | `Testimonial - Susanne - 9-16 - Short - mit Abbinder - Vorstellung.mp4` | `vorstellung` |
| 2 | Warum Regios | `Testimonial - Susanne - 1-1 - Short - mit Abbinder - Warum Regios.mp4` | `Testimonial - Susanne - 9-16 - Short - mit Abbinder - Warum Regios.mp4` | `warum_regios` |
| 3 | USP | `Testimonial - Susanne - 1-1 - Short - mit Abbinder - USP.mp4` | `Testimonial - Susanne - 9-16 - Short - mit Abbinder - USP.mp4` | `usp` |
| 4 | Sichtbare Veränderung | `Testimonial - Susanne - 1-1 - Short - mit Abbinder - Sichtbare Veränderung.mp4` | `Testimonial - Susanne - 9-16 - Short - mit Abbinder - Sichtbare Veränderung.mp4` | `veraenderung` |
| 5 | Gemeinsames Eigentum | `Testimonial - Susanne - 1-1 - Short - mit Abbinder - gemeinsames Eigentum.mp4` | `Testimonial - Susanne - 9-16 - Short - mit Abbinder - gemeinsames Eigentum.mp4` | `eigentum` |
| 6 | Regios wichtiger Partner | `Testimonial - Susanne - 1-1 - Short - mit Abbinder - Regios wichtiger Partner für Energie.mp4` | `Testimonial - Susanne - 9-16 - Short - mit Abbinder - Regios wichtiger Partner für Energie.mp4` | `partner` |
| 7 | Erreichbarkeit | `Testimonial - Susanne - 1-1 - Short - mit Abbinder - Erreichbarkeit.mp4` | `Testimonial - Susanne - 9-16 - Short - mit Abbinder - Erreichbarkeit.mp4` | `erreichbarkeit` |
| 8 | Risiko oder Chance | `Testimonial - Susanne - 1-1 - Short - mit Abbinder - Riskio oder Chance.mp4` | `Testimonial - Susanne - 9-16 - Short - mit Abbinder - Riskio oder Chance.mp4` | `risiko_chance` |
| 9 | Vertrauen | `Testimonial - Susanne - 1-1 - Short  - mit Abbinder - Vertrauen.mp4` | `Testimonial - Susanne - 9-16 - Short - mit Abbinder - Vertrauen.mp4` | `vertrauen` |
| 10 | Danke | `Testimonial - Susanne - 1-1 - Short - mit Abbinder - Danke.mp4` | `Testimonial - Susanne - 9-16 - Short - mit Abbinder - Danke.mp4` | `danke` |

**Caption:** 👩‍💼 Susanne, Gemeindevertreterin: „[Topic]"<br><br>Unsere Susanne, Unsere Gemeinden, UNSERE ENERGIE REGIOS 🌱<br><br>#regios #mühlviertel #gemeinde #energiegenossenschaft #miasanneddeppad

**Base URL:** `https://www.regios.at/gemeinde?utm_source=instagram&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial&utm_content=susanne`

**CTA:** Learn More

---

#### Norbert (Bürger) - 10 Ads

**Asset Paths:**
- Feed (1:1): `Testimonial - Norbert/Norbert 1_1 mit Abbinder/`
- Story (9:16): `Testimonial - Norbert/Norbert 9_16 mit Abbinder/`

| Ad | Topic | Video Feed (1:1) | Video Story (9:16) | utm_term |
|----|-------|------------------|-------------------|----------|
| 1 | Vorstellung | `Testimonial - Norbert - 1-1 - Short - mit Abbinder - Vorstellung.mp4` | `Testimonial - Norbert - 9-16 - Short - mit Abbinder - Vorstellung.mp4` | `vorstellung` |
| 2 | Sicherheit | `Testimonial - Norbert - 1-1 - Short - mit Abbinder - Sicherheit.mp4` | `Testimonial - Norbert - 9-16 - Short - mit Abbinder - Sicherheit.mp4` | `sicherheit` |
| 3 | Transparenz | `Testimonial - Norbert - 1-1 - Short - mit Abbinder - Transparenz.mp4` | `Testimonial - Norbert - 9-16 - Short - mit Abbinder - Transparenz.mp4` | `transparenz` |
| 4 | Vertrauen | `Testimonial - Norbert - 1-1 - Short - mit Abbinder - Vertrauen.mp4` | `Testimonial - Norbert - 9-16 - Short - mit Abbinder - Vertrauen.mp4` | `vertrauen` |
| 5 | Nachhaltigkeit | `Testimonial - Norbert - 1-1 - Short - mit Abbinder - Nachhaltigkeit.mp4` | `Testimonial - Norbert - 9-16 - Short - mit Abbinder - Nachhaltigkeit.mp4` | `nachhaltigkeit` |
| 6 | Banken als Partner | `Testimonial - Norbert - 1-1 - Short - mit Abbinder - Banken als Partner.mp4` | `Testimonial - Norbert - 9-16 - Short - mit Abbinder - Banken als Partner.mp4` | `banken_partner` |
| 7 | Wirkungskraft | `Testimonial - Norbert - 1-1 - Short - mit Abbinder - Wirkungskraft.mp4` | `Testimonial - Norbert - 9-16 - Short - mit Abbinder - Wirkungskraft.mp4` | `wirkungskraft` |
| 8 | Erreichbarkeit | `Testimonial - Norbert - 1-1 - Short - mit Abbinder - Erreichbarkeit.mp4` | `Testimonial - Norbert - 9-16 - Short - mit Abbinder - Erreichbarkeit.mp4` | `erreichbarkeit` |
| 9 | Risiko | `Testimonial - Norbert - 1-1 - Short - mit Abbinder - Risiko.mp4` | `Testimonial - Norbert - 9-16 - Short - mit Abbinder - Risiko.mp4` | `risiko` |
| 10 | Risiko oder Chance | `Testimonial - Norbert - 1-1 - Short - mit Abbinder - Risiko oder Chance.mp4` | `Testimonial - Norbert - 9-16 - Short - mit Abbinder - Risiko oder Chance.mp4` | `risiko_chance` |

**Caption:** 👨 Norbert aus dem Mühlviertel: „[Topic]"<br><br>Unser Norbert, Unsere Sicherheit, UNSERE ENERGIE REGIOS 🌱<br><br>#regios #mühlviertel #testimonial #energiegenossenschaft #miasanneddeppad

**Base URL:** `https://www.regios.at/buerger?utm_source=instagram&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial&utm_content=norbert`

**CTA:** Learn More

---

#### Christian (Bank) - 19 Ads

**Asset Paths:**
- Feed (1:1): `Testimonial - Christian/1_1/`
- Story (9:16): `Testimonial - Christian/9_16/`

| Ad | Topic | Video Feed (1:1) | Video Story (9:16) | utm_term |
|----|-------|------------------|-------------------|----------|
| 1 | Vorstellung | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Vorstellung.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Vorstellung.mp4` | `vorstellung` |
| 2 | Bank als Entwicklungspartner | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Bank als Entwicklungspartner.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Bank als Entwicklungspartner.mp4` | `entwicklungspartner` |
| 3 | Banken und öffentliche Hand | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Banken und öffentliche Hand.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Banken und öffentliche Hand.mp4` | `oeffentliche_hand` |
| 4 | Fossiler zu erneuerbar | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Fossiler zu erneuerbar.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Fossiler zu erneuerbar.mp4` | `erneuerbar` |
| 5 | Gfrei und Sichtbar | `Testimonial - Christian - 1-1 - Short - mit Abbinder- Gfrei- und Sichtbar.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Gfrei- und Sichtbar.mp4` | `gfrei_sichtbar` |
| 6 | Integration | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Integration.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Integration.mp4` | `integration` |
| 7 | Investition Energie | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Investition Energie.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Investition Energie.mp4` | `investition` |
| 8 | Langfristigkeit als Erfolgsmodell | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Langfristigkei als Erfolgsmodell.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Langfristigkei als Erfolgsmodell.mp4` | `erfolgsmodell` |
| 9 | Langfristigkeit | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Langfristigkeit.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Langfristigkeit.mp4` | `langfristigkeit` |
| 10 | Nachhaltigkeit | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Nachhaltigkeit.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Nachhaltigkeit.mp4` | `nachhaltigkeit` |
| 11 | Prinzip Genossenschaft | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Prinzip Genossenschaft.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Prinzip Genossenschaft.mp4` | `prinzip` |
| 12 | Regios als langfristiges Modell | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Regios als langfristiges Modell.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Regios als langfristiges Modell.mp4` | `langfristiges_modell` |
| 13 | Sicherheit Stabilität | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Sicherheit Stabilität.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Sicherheit Stabilität.mp4` | `sicherheit_stabilitaet` |
| 14 | Struktur Aufstellung | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Struktur Aufstellung.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Struktur Aufstellung.mp4` | `struktur` |
| 15 | Transparenz | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Transparenz.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Transparenz.mp4` | `transparenz` |
| 16 | Vertrauen | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Vertrauen.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Vertrauen.mp4` | `vertrauen` |
| 17 | Wirkungskraft | `Testimonial - Christian - 1-1 - Short - mit Abbinder - Wirkungskraft.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - Wirkungskraft.mp4` | `wirkungskraft` |
| 18 | Geprüfte Produkte | `Testimonial - Christian - 1-1 - Short - mit Abbinder - geprüfte Produkte.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - geprüfte Produkte.mp4` | `produkte` |
| 19 | Greifbare Kommunikation | `Testimonial - Christian - 1-1 - Short - mit Abbinder - greifbare Kommunikation.mp4` | `Testimonial - Christian - 9-16 - Short - mit Abbinder - greifbare Kommunikation.mp4` | `kommunikation` |

**Caption:** 🏦 Christian, Bankpartner: „[Topic]"<br><br>Unser Christian, Unsere Partner, UNSERE ENERGIE REGIOS 🌱<br><br>#regios #mühlviertel #bank #energiegenossenschaft #miasanneddeppad

**Base URL:** `https://www.regios.at/bank?utm_source=instagram&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial&utm_content=christian`

**CTA:** Learn More

---

#### Klaus (Unternehmer) - 12 Ads

**Asset Paths:**
- Feed (1:1): `Testimonial - Klaus/Klaus 1_1 mit Abbinder/`
- Story (9:16): `Testimonial - Klaus/Klaus 9_16 mit Abbinder/`

| Ad | Topic | Video Feed (1:1) | Video Story (9:16) | utm_term |
|----|-------|------------------|-------------------|----------|
| 1 | Vorstellung | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - Vorstellung.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - Vorstellung.mp4` | `vorstellung` |
| 2 | Kompetenz Regios | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - Kompetenz Regios.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - Kompetenz Regios.mp4` | `kompetenz` |
| 3 | Regionale Wertschöpfung | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - regionale Wertschöpfung.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - regionale Wertschöpfung.mp4` | `wertschoepfung` |
| 4 | Stabile Preisentwicklung | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - stabile Preisentwicklung.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - stabile Preisentwicklung.mp4` | `preisentwicklung` |
| 5 | Unabhängigkeit Selbstgestaltung | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - Unabhängigkeit Selbstgestaltung.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - Unabhängigkeit Selbstgestaltung.mp4` | `unabhaengigkeit` |
| 6 | Verantwortung der Region | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - Verantwortung der Region.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - Verantwortung der Region.mp4` | `verantwortung` |
| 7 | Vertrauen | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - Vertrauen.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - Vertrauen.mp4` | `vertrauen` |
| 8 | Transparenz | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - Transparenz.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - Transparenz.mp4` | `transparenz` |
| 9 | Langfristigkeit | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - Langfristigkeit.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - Langfristigkeit.mp4` | `langfristigkeit` |
| 10 | Wirkungskraft | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - Wirkungskraft.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - Wirkungskraft.mp4` | `wirkungskraft` |
| 11 | Energiekosten | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - Energiekosten.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - Energiekosten.mp4` | `energiekosten` |
| 12 | Vorbild Regios | `Testimonial - Klaus - 1-1 - Short - mit Abbinder - Vorbild Regios.mp4` | `Testimonial - Klaus - 9-16 - Short - mit Abbinder - Vorbild Regios.mp4` | `vorbild` |

**Caption:** 👨‍💼 Klaus, Unternehmer: „[Topic]"<br><br>Unser Klaus, Unsere Unternehmer, UNSERE ENERGIE REGIOS 🌱<br><br>#regios #mühlviertel #unternehmer #energiegenossenschaft #miasanneddeppad

**Base URL:** `https://www.regios.at/unternehmer?utm_source=instagram&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial&utm_content=klaus`

**CTA:** Learn More

---

### Ad Set 2b: Instagram - Long Videos

**Placements:** Instagram Feed, Instagram Reels

**Asset Path:** `Final Assets/Social Media/Retargeting/Video/Retargeting/Meta All/`

| Ad | Person | Video (16:9) | Landing Page | Full URL |
|----|--------|--------------|--------------|----------|
| 1 | Sarah | `Testimonial - Sarah/Sarah 16_9 mit Abbinder/Testimonial - Sarah - Long - V1.mp4` | /buerger | `https://www.regios.at/buerger?utm_source=instagram&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial&utm_content=sarah&utm_term=long` |
| 2 | Peter | `Testimonial - Peter/Peter 16_9 mit Abbinder/Testimonial - Peter - Long - V1.mp4` | /grundbesitzer | `https://www.regios.at/grundbesitzer?utm_source=instagram&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial&utm_content=peter&utm_term=long` |
| 3 | Susanne | `Testimonial - Susanne/Susanne 16_9 mit Abbinder/Testimonial - Susanne - Long - mit Abbinder - V1.mp4` | /gemeinde | `https://www.regios.at/gemeinde?utm_source=instagram&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial&utm_content=susanne&utm_term=long` |
| 4 | Klaus | `Testimonial - Klaus/Klaus 16_9 mit Abbinder/Testimonial - Klaus - Long - mit Abbinder - V1.mp4` | /unternehmer | `https://www.regios.at/unternehmer?utm_source=instagram&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial&utm_content=klaus&utm_term=long` |

**Caption Template:** 👤 [Name] aus dem Mühlviertel: Das ganze Interview<br><br>UNSERE ENERGIE REGIOS 🌱<br><br>Mia san ned Deppad! Erfahre die komplette Geschichte.<br><br>#regios #mühlviertel #testimonial #energiegenossenschaft #miasanneddeppad

**CTA:** Learn More

---

### Ad Set 3b: Instagram - Image Carousels

**Placements:** Instagram Feed

**Purpose:** Static image carousels for users who engaged but haven't converted.

---

**Carousel 1: Grünstrom Elements**

| Field | Content |
|-------|---------|
| Images | Sonne, Wasser, Wind carousels mixed |
| Caption | 🌱 Du hast dich schon über Regios informiert. Jetzt ist der richtige Zeitpunkt!<br><br>Unser Wasser, Unsere Sonne, Unser Wind, UNSERE ENERGIE REGIOS<br><br>Mia san ned Deppad! 🌱<br><br>#regios #mühlviertel #grünstrom #energiegenossenschaft #miasanneddeppad |
| CTA | Learn More |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=instagram&utm_medium=retargeting&utm_campaign=gruenstrom_mofu_retargeting&utm_content=carousel&utm_term=elements` |

---

**Carousel 2: Genossenschaft Values**

| Field | Content |
|-------|---------|
| Images | Stabilitaet, Zukunft, Sicherheit carousels mixed |
| Caption | 🤝 Bereit für den nächsten Schritt?<br><br>Unsere Stabilität, Unsere Sicherheit, Unsere Zukunft, UNSERE ENERGIE REGIOS<br><br>Mia Mühlviertel entscheiden selber wie es uns weitergeht! 🌱<br><br>#regios #mühlviertel #genossenschaft #energiegenossenschaft #miasanneddeppad |
| CTA | Learn More |
| Website URL | `https://www.regios.at/beteiligung?utm_source=instagram&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_retargeting&utm_content=carousel&utm_term=values` |

---

### Retargeting Ad Count Summary

| Person | Role | Landing Page | Short Videos | Long Video | Total |
|--------|------|--------------|--------------|------------|-------|
| Sarah | Bürger:in | /buerger | 11 | 1 | 12 |
| Peter | Grundbesitzer | /grundbesitzer | 7 | 1 | 8 |
| Susanne | Gemeinde | /gemeinde | 10 | 1 | 11 |
| Norbert | Bürger | /buerger | 10 | 0 | 10 |
| Christian | Bank | /bank | 19 | 0 | 19 |
| Klaus | Unternehmer | /unternehmer | 12 | 1 | 13 |
| **Total per platform** | | | **69** | **4** | **73 video ads** |
| **Image Carousels** | | | | | **2 per platform** |
| **Total (FB + IG)** | | | **138** | **8** | **150 ads total** |

---

### YouTube Retargeting Note

**Can you retarget YouTube viewers?**

Yes, you can create audiences based on:
- People who viewed any video from your channel
- People who viewed certain videos
- People who subscribed to your channel
- People who visited your channel page
- People who liked/commented/shared videos
- People who viewed ads (TrueView)

**Recommendation:** Create a "Video Viewers" audience in Google Ads:
1. Go to Tools & Settings > Audience Manager
2. Create Custom Audience > YouTube users
3. Select: "Viewed any video from a channel" + your channel
4. Use this audience for Display/Search retargeting

---

## 9. Landing Pages & URLs

### Primary Landing Pages

| Product | URL | Purpose |
|---------|-----|---------|
| Grünstrom | `https://www.regios.at/regionaler-gruenstrom` | Green electricity information |
| Beteiligung | `https://www.regios.at/beteiligung` | Cooperative membership/investment |
| Bürger | `https://www.regios.at/buerger` | Citizen focused landing page |
| Homepage | `https://www.regios.at` | Brand searches |

---

## 10. Audience Setup

### Google Audiences

**Remarketing Lists to Create:**

| Audience Name | Definition | Membership Duration |
|---------------|------------|---------------------|
| `Bürger` | Visitors to /buerger page | 90 days |
| `Genossenschaft` | Visitors to /beteiligung page | 90 days |
| `Grünstrom` | Visitors to /regionaler gruenstrom page | 90 days |
| `All Website Visitors` | All visitors | 30 days |
| `YouTube Viewers` | Viewed any video from channel | 90 days |
| `Converters` | Completed form submission | 540 days |

**Custom Intent Audiences:**

| Audience Name | Keywords/URLs |
|---------------|---------------|
| `Green Energy Seekers` | ökostrom, grünstrom, erneuerbare energie, nachhaltige energie |
| `Investors Local` | investieren oberösterreich, genossenschaft, beteiligung energie |
| `Property Owners` | hauseigentümer, immobilie, grundstück mühlviertel |

### Meta Audiences

**Custom Audiences to Create:**

| Audience Name | Source | Duration |
|---------------|--------|----------|
| `Engagement: Paid Ads` | People who engaged with paid ads | 180 days |
| `Engagement: Organic` | People who engaged with organic content | 180 days |
| `Engagement: IG/FB Followers` | Current followers | All |
| `Engagement: Messenger` | People who sent message | 180 days |
| `Website: All Visitors` | Pixel All visitors | 30 days |
| `Website: Grünstrom` | Pixel /regionaler gruenstrom | 60 days |
| `Website: Beteiligung` | Pixel /beteiligung | 60 days |
| `Website: Bürger` | Pixel /buerger | 60 days |
| `Video: 50% Viewed` | People who watched 50%+ of videos | 90 days |
| `Video: 75% Viewed` | People who watched 75%+ of videos | 90 days |

---

## 11. Asset Mapping by Campaign

This section maps every available asset to its specific campaign, ad group, and placement.

---

### GOOGLE DISPLAY CAMPAIGNS

---

#### Campaign A: Display Targeting Grünstrom (Classic HTML5)
`[Display > Classic > Targeting > Upper Austria > 30+] Gruenstrom`

**Ad Format:** HTML5 Banners

| Ad Group | Theme | HTML5 Banner Files | Sizes |
|----------|-------|-------------------|-------|
| Ad Group 1 | Wasser | `Google/Retargeting/Banners/HTML5/Wasser_[SIZE].zip` | 300x250, 300x600, 320x50, 336x280, 728x90 |
| Ad Group 2 | Wind | `Google/Retargeting/Banners/HTML5/Wind_[SIZE].zip` | 300x250, 300x600, 320x50, 336x280, 728x90 |
| Ad Group 3 | Licht (Sonne) | `Google/Retargeting/Banners/HTML5/Licht_[SIZE].zip` | 300x250, 300x600, 320x50, 336x280, 728x90 |

---

#### Campaign A2: Display Targeting Grünstrom (Responsive)
`[Display > Responsive > Targeting > Upper Austria > 30+] Gruenstrom`

**Ad Format:** Responsive Display Ads

| Ad | Theme | Landscape Image (1200x628) | Square Image (1080x1080) |
|----|-------|---------------------------|-------------------------|
| RDA 1 | Sonne | `Google/RAW/[Sonne cropped]` ⚠️ TEMPORARY | `Social Media/Targeting/Posts/Carousels/1080x1080/sonne/Sonne_1080x1080_1.png` |
| RDA 2 | Wasser | `Google/RAW/[Wasser cropped]` ⚠️ TEMPORARY | `Social Media/Targeting/Posts/Carousels/1080x1080/wasser/wasser_1080x1080_1.png` |
| RDA 3 | Wind | `Google/RAW/[Wind cropped]` ⚠️ TEMPORARY | `Social Media/Targeting/Posts/Carousels/1080x1080/wind/WInd_1080x1080_1.png` |

---

#### Campaign B: Display Targeting Genossenschaft (Classic HTML5)
`[Display > Classic > Targeting > Upper Austria > 30+] Genossenschaft`

**Ad Format:** HTML5 Banners

| Ad Group | Theme | HTML5 Banner Files | Sizes |
|----------|-------|-------------------|-------|
| Ad Group 1 | Stabilitaet | `Google/Retargeting/Banners/HTML5/Stabilitaet_[SIZE].zip` | 160x600, 300x250, 300x600, 320x50, 320x100, 336x280, 728x90, 970x250 |
| Ad Group 2 | Zukunft | `Google/Retargeting/Banners/HTML5/Zukunft_[SIZE].zip` | 300x250, 300x600, 320x50, 336x280, 728x90 |

---

#### Campaign B2: Display Targeting Genossenschaft (Responsive)
`[Display > Responsive > Targeting > Upper Austria > 30+] Genossenschaft`

**Ad Format:** Responsive Display Ads

| Ad | Theme | Landscape Image (1200x628) | Square Image (1080x1080) |
|----|-------|---------------------------|-------------------------|
| RDA 1 | Stabilitaet | `Google/RAW/[Stabilitaet cropped]` ⚠️ TEMPORARY | `Social Media/Targeting/Posts/Carousels/1080x1080/Stabilitaet/Stabilitaet_1080x1080_1.png` |
| RDA 2 | Zukunft | `Google/RAW/[Zukunft cropped]` ⚠️ TEMPORARY | `Social Media/Targeting/Posts/Carousels/1080x1080/Zukunft/Zukunft_1080x1080_1.png` |

---

#### Campaign C: Display Retargeting (Classic HTML5 ONLY)
`[Display > Classic > Retargeting > Upper Austria > 30+] Retargeting`

**Ad Format:** HTML5 Banners ONLY (no Responsive for Retargeting)

**Ad Group 1: Grünstrom Retargeting**

| Theme | HTML5 Banner Files | Sizes |
|-------|-------------------|-------|
| Wasser | `Google/Retargeting/Banners/HTML5/Wasser_[SIZE].zip` | 300x250, 300x600, 320x50, 336x280, 728x90 |
| Wind | `Google/Retargeting/Banners/HTML5/Wind_[SIZE].zip` | 300x250, 300x600, 320x50, 336x280, 728x90 |
| Licht (Sonne) | `Google/Retargeting/Banners/HTML5/Licht_[SIZE].zip` | 300x250, 300x600, 320x50, 336x280, 728x90 |

**Ad Group 2: Genossenschaft Retargeting**

| Theme | HTML5 Banner Files | Sizes |
|-------|-------------------|-------|
| Stabilitaet | `Google/Retargeting/Banners/HTML5/Stabilitaet_[SIZE].zip` | 160x600, 300x250, 300x600, 320x50, 320x100, 336x280, 728x90, 970x250 |
| Zukunft | `Google/Retargeting/Banners/HTML5/Zukunft_[SIZE].zip` | 300x250, 300x600, 320x50, 336x280, 728x90 |
| Sarah (BOFU) | `Google/Retargeting/Banners/HTML5/Sarah_[SIZE].zip` | 300x250, 300x600, 320x50, 320x100, 336x280, 728x90 |

---

### COMPLETE HTML5 BANNER FILE LIST

**Grünstrom Themes:**

```
Google/Retargeting/Banners/HTML5/Wasser_300x250.zip
Google/Retargeting/Banners/HTML5/Wasser_300x600.zip
Google/Retargeting/Banners/HTML5/Wasser_320x50.zip
Google/Retargeting/Banners/HTML5/Wasser_336x280.zip
Google/Retargeting/Banners/HTML5/Wasser_728x90.zip

Google/Retargeting/Banners/HTML5/Wind_300x250.zip
Google/Retargeting/Banners/HTML5/Wind_300x600.zip
Google/Retargeting/Banners/HTML5/Wind_320x50.zip
Google/Retargeting/Banners/HTML5/Wind_336x280.zip
Google/Retargeting/Banners/HTML5/Wind_728x90.zip

Google/Retargeting/Banners/HTML5/Licht_300x250.zip
Google/Retargeting/Banners/HTML5/Licht_300x600.zip
Google/Retargeting/Banners/HTML5/Licht_320x50.zip
Google/Retargeting/Banners/HTML5/Licht_336x280.zip
Google/Retargeting/Banners/HTML5/Licht_728x90.zip
```

**Genossenschaft Themes:**

```
Google/Retargeting/Banners/HTML5/Stabilitaet_160x600.zip
Google/Retargeting/Banners/HTML5/Stabilitaet_300x250.zip
Google/Retargeting/Banners/HTML5/Stabilitaet_300x600.zip
Google/Retargeting/Banners/HTML5/Stabilitaet_320x50.zip
Google/Retargeting/Banners/HTML5/Stabilitaet_320X100.zip
Google/Retargeting/Banners/HTML5/Stabilitaet_336x280.zip
Google/Retargeting/Banners/HTML5/Stabilitaet_728x90.zip
Google/Retargeting/Banners/HTML5/Stabilitaet_970x250.zip

Google/Retargeting/Banners/HTML5/Zukunft_300x250.zip
Google/Retargeting/Banners/HTML5/Zukunft_300x600.zip
Google/Retargeting/Banners/HTML5/Zukunft_320x50.zip
Google/Retargeting/Banners/HTML5/Zukunft_336x280.zip
Google/Retargeting/Banners/HTML5/Zukunft_728x90.zip

Google/Retargeting/Banners/HTML5/Sarah_300x250.zip
Google/Retargeting/Banners/HTML5/Sarah_300x600.zip
Google/Retargeting/Banners/HTML5/Sarah_320x50.zip
Google/Retargeting/Banners/HTML5/Sarah_320x100.zip
Google/Retargeting/Banners/HTML5/Sarah_336x280.zip
Google/Retargeting/Banners/HTML5/Sarah_728X90.zip
```

---

### RESPONSIVE DISPLAY AD IMAGE SOURCES

**⚠️ LANDSCAPE IMAGES (1200x628) - TEMPORARY CROPS FROM:**
`Google/RAW/`

These must be replaced with properly designed landscape assets when the design team delivers them.

**SQUARE IMAGES (1080x1080) - FROM:**
`Social Media/Targeting/Posts/Carousels/1080x1080/`

| Theme | Square Image File |
|-------|------------------|
| Sonne | `Social Media/Targeting/Posts/Carousels/1080x1080/sonne/Sonne_1080x1080_1.png` |
| Wasser | `Social Media/Targeting/Posts/Carousels/1080x1080/wasser/wasser_1080x1080_1.png` |
| Wind | `Social Media/Targeting/Posts/Carousels/1080x1080/wind/WInd_1080x1080_1.png` |
| Stabilitaet | `Social Media/Targeting/Posts/Carousels/1080x1080/Stabilitaet/Stabilitaet_1080x1080_1.png` |
| Zukunft | `Social Media/Targeting/Posts/Carousels/1080x1080/Zukunft/Zukunft_1080x1080_1.png` |
| Sicherheit | `Social Media/Targeting/Posts/Carousels/1080x1080/Sicherheit/Sicherheit_1080x1080_1.png` |
| Sarah | `Social Media/Targeting/Posts/Carousels/1080x1080/sarah/Sarah_1080x1080_1.png` |
| Susanne | `Social Media/Targeting/Posts/Carousels/1080x1080/susanne/susanne_1080x1080_1.png` |

---

### GOOGLE YOUTUBE CAMPAIGN

#### Campaign: YouTube Targeting Grünstrom
`[Video > Non skippable > Muehviertel > 30+] 15 Sek Strom`

| Ad Group | Theme | Video File |
|----------|-------|------------|
| Ad Group 1 | Sonne | `Google/Targeting/Strom/15 Sek Strom - Sonne - Online - 16-9 - V1.mp4` |
| Ad Group 2 | Wasser | `Google/Targeting/Strom/15 Sek Strom - Wasser - Online - 16-9 - V1.mp4` |
| Ad Group 3 | Wind | `Google/Targeting/Strom/15 Sek Strom - Wind - Online - 16-9 - V1.mp4` |

---

### META CAMPAIGNS

#### Facebook Targeting: Grünstrom
`[Awareness > Auction > Muehviertel > 30+] Gruenstrom`

**Note:** Each ad combines Feed (1:1) + Story (9:16) placements with a single UTM.

| Ad | Theme | Video Feed (1:1) | Video Story (9:16) |
|----|-------|-----------------|-------------------|
| Ad 1 | Sonne | `Social Media/Targeting/Video/15 Sek - Strom/15 Sek Strom - Sonne - Online - 1-1 - V1.mp4` | `Social Media/Retargeting/Video/Targeting/FB/Story/15 Sek Strom - Sonne - Online - 9-16 - V3.mp4` |
| Ad 2 | Wasser | `Social Media/Targeting/Video/15 Sek - Strom/15 Sek Strom - Wasser - Online - 1-1 - V1.mp4` | `Social Media/Retargeting/Video/Targeting/FB/Story/15 Sek Strom - Wasser - Online - 9-16 - V3.mp4` |
| Ad 3 | Wind | `Social Media/Targeting/Video/15 Sek - Strom/15 Sek Strom - Wind - Online - 1-1 - V1.mp4` | `Social Media/Retargeting/Video/Targeting/FB/Story/15 Sek Strom - Wind - Online - 9-16 - V3.mp4` |
| Ad 4 | Strom 30s | `Social Media/Retargeting/Video/Targeting/Instagram/Post/30 Sek Kurz - Strom - TV - 1-1 - V1 ohne URL.mp4` | `Social Media/Retargeting/Video/Targeting/FB/Story/30 Sek Kurz - Strom - TV - 9-16 - V1 ohne URL.mp4` |

---

#### Facebook Targeting: Genossenschaft
`[Traffic > Auction > Muehviertel > 30+] Genossenschaft`

**Note:** Each ad combines Feed (1:1) + Story (9:16) placements with a single UTM.

| Ad | Theme | Video Feed (1:1) | Video Story (9:16) |
|----|-------|-----------------|-------------------|
| Ad 1 | Genossenschaft 30s | `Social Media/Retargeting/Video/Targeting/Instagram/Post/30 Sek Kurz - Genossenschaft - TV - 1-1 - V1 ohne URL.mp4` | `Social Media/Retargeting/Video/Targeting/FB/Story/30 Sek Kurz - Genossenschaft - TV - 9-16 - V1 ohne URL.mp4` |

---

#### Facebook Targeting: Carousels
`[Traffic > Auction > Muehviertel > 30+] Carousels`

| Carousel | Theme | Image Files (5 cards each) |
|----------|-------|---------------------------|
| Carousel 1 | Sonne | `Social Media/Targeting/Posts/Carousels/1080x1080/sonne/Sonne_1080x1080_[1-5].png` |
| Carousel 2 | Wasser | `Social Media/Targeting/Posts/Carousels/1080x1080/wasser/wasser_1080x1080_[1-5].png` |
| Carousel 3 | Wind | `Social Media/Targeting/Posts/Carousels/1080x1080/wind/WInd_1080x1080_[1-5].png` |
| Carousel 4 | Stabilitaet | `Social Media/Targeting/Posts/Carousels/1080x1080/Stabilitaet/Stabilitaet_1080x1080_[1-5].png` |
| Carousel 5 | Zukunft | `Social Media/Targeting/Posts/Carousels/1080x1080/Zukunft/Zukunft_1080x1080_[1-5].png` |
| Carousel 6 | Sicherheit | `Social Media/Targeting/Posts/Carousels/1080x1080/Sicherheit/Sicherheit_1080x1080_[1-5].png` |

---

#### Instagram Targeting
`[Awareness > Auction > Muehviertel > 30+] IG Gruenstrom`
`[Traffic > Auction > Muehviertel > 30+] IG Genossenschaft`

**Note:** Each ad combines Feed (1:1) + Story (9:16) placements with a single UTM. Same video assets as Facebook.

| Carousel | Theme | Image Files |
|----------|-------|-------------|
| Sarah | Testimonial | `Social Media/Targeting/Posts/Carousels/1080x1080/sarah/Sarah_1080x1080_[1-5].png` |
| Susanne | Testimonial | `Social Media/Targeting/Posts/Carousels/1080x1080/susanne/susanne_1080x1080_[1-5].png` |

---

#### Meta Retargeting
`[Traffic > Auction > Retargeting] Meta Retargeting`

**Testimonial Videos (Priority Order):**

| Priority | Testimonial | Video Files |
|----------|-------------|-------------|
| 1 | Sarah | `Social Media/Retargeting/Video/Retargeting/FB Feed/Retargeting/Testimonial - Sarah/Testimonial - Sarah - Short - Warum Regios.mp4` |
| 1 | Sarah | `Social Media/Retargeting/Video/Retargeting/FB Feed/Retargeting/Testimonial - Sarah/Testimonial - Sarah - Short - Wertschöpfung in der Region.mp4` |
| 1 | Sarah | `Social Media/Retargeting/Video/Retargeting/FB Feed/Retargeting/Testimonial - Sarah/Testimonial - Sarah - Short - Gemeinsam Stark.mp4` |
| 1 | Sarah | `Social Media/Retargeting/Video/Retargeting/FB Feed/Retargeting/Testimonial - Sarah/Testimonial - Sarah - Long - V1.mp4` |
| 2 | Peter | `Social Media/Retargeting/Video/Retargeting/FB Feed/Retargeting/Testimonial - Peter/Testimonial - Peter - Short - Doppelnutzung.mp4` |
| 2 | Peter | `Social Media/Retargeting/Video/Retargeting/FB Feed/Retargeting/Testimonial - Peter/Testimonial - Peter - Long - V1.mp4` |
| 3 | Susanne | `Social Media/Retargeting/Video/Retargeting/FB Feed/Retargeting/Testimonial - Susanne/Testimonial - Susanne - Short - Warum Regios.mp4` |
| 3 | Susanne | `Social Media/Retargeting/Video/Retargeting/FB Feed/Retargeting/Testimonial - Susanne/Testimonial - Susanne - Long - mit Abbinder - V1.mp4` |
| 4 | Norbert | `Social Media/Retargeting/Video/Retargeting/FB Feed/Retargeting/Testimonial - Norbert/Testimonial - Norbert - Short - Sicherheit.mp4` |
| 4 | Norbert | `Social Media/Retargeting/Video/Retargeting/FB Feed/Retargeting/Testimonial - Norbert/Testimonial - Norbert - Long - mit Abbinder - V1.mp4` |

---

### ADDITIONAL AVAILABLE ASSETS (Not Currently Mapped)

**Christian Testimonials:**
`Social Media/Retargeting/Video/Retargeting/FB Feed/Retargeting/Testimonial - Christian/`

**Klaus Testimonials:**
`Social Media/Retargeting/Video/Retargeting/FB Feed/Retargeting/Testimonial - Klaus/`

**Additional Carousel Formats:**
- 1080x1350 (Instagram Portrait): `Social Media/Targeting/Posts/Carousels/1080x1350/`
- 1080x1920 (Stories/Reels): `Social Media/Targeting/Posts/Carousels/1080x1920/`
- 1200x628 (Facebook Link): `Social Media/Targeting/Posts/Carousels/1200x628/`

---

## 12. Looker Studio Requirements

### Data Sources to Connect

| Platform | Data Source | Connection Method |
|----------|-------------|-------------------|
| Google Ads | Google Ads Connector | Native Looker Studio connector |
| Google Analytics 4 | GA4 Connector | Native Looker Studio connector |
| Meta Ads | Facebook Ads Connector | Supermetrics or native connector |

### Required Dimensions for Consistency

**From UTM Parameters (via GA4):**

| Dimension | UTM Parameter | Example Values |
|-----------|---------------|----------------|
| Source | utm_source | google, facebook, instagram |
| Medium | utm_medium | cpc, display, video, social, retargeting |
| Campaign | utm_campaign | gruenstrom_tofu_sonne, genossenschaft_bofu_testimonial_sarah |
| Content | utm_content | video15_sonne_1x1, banner_stabilitaet_300x250 |

**Derived Dimensions (create calculated fields):**

| Calculated Field | Formula | Purpose |
|------------------|---------|---------|
| Product | REGEXP_EXTRACT(Campaign, "^(gruenstrom\|genossenschaft\|brand)") | Segment by product |
| Funnel Stage | REGEXP_EXTRACT(Campaign, "_(tofu\|mofu\|bofu\|search)_") | Segment by funnel |
| Creative Theme | REGEXP_EXTRACT(Campaign, "_([^_]+)$") | Segment by theme |

### Recommended Report Pages

1. **Executive Summary** Total Spend, Impressions, Clicks, Conversions
2. **Platform Performance** Google vs Meta comparison
3. **Funnel Analysis** TOFU/MOFU/BOFU metrics
4. **Product Performance** Grünstrom vs Genossenschaft
5. **Creative Analysis** Performance by theme
6. **Retargeting Analysis** Testimonial performance

### Key Metrics to Track

| Metric | Target |
|--------|--------|
| Reach | 50,000+ |
| Frequency | 3 to 5x |
| CTR | 1%+ |
| CPC | less than €0.50 |
| CPM | less than €10 |
| Video Completion | 30%+ |
| CPA | less than €25 |

---

## 13. Campaign Checklist

### Pre Launch Checklist

**Google Ads:**
- [ ] Conversion tracking configured
- [ ] Remarketing lists created
- [ ] YouTube channel linked
- [ ] HTML5 banners uploaded
- [ ] All UTM URLs tested

**Meta Ads:**
- [ ] Facebook Pixel installed
- [ ] Custom Audiences created
- [ ] Video assets uploaded
- [ ] All UTM URLs tested

**Tracking & Reporting:**
- [ ] GA4 receiving data
- [ ] Looker Studio connected
- [ ] Calculated fields created

---

## 14. Quick Reference All Campaign Names

### Google Campaigns

| Campaign Name | Type | Daily Budget |
|---------------|------|--------------|
| `[Search > Brand+Generic > Upper Austria > 30+] Regios` | Search | €5.00 |
| `[Display > Classic > Targeting > Upper Austria > 30+] Gruenstrom` | Classic HTML5 | €2.00 |
| `[Display > Classic > Targeting > Upper Austria > 30+] Genossenschaft` | Classic HTML5 | €2.00 |
| `[Display > Responsive > Targeting > Upper Austria > 30+] Gruenstrom` | Responsive | €2.00 |
| `[Display > Responsive > Targeting > Upper Austria > 30+] Genossenschaft` | Responsive | €2.00 |
| `[Display > Classic > Retargeting > Upper Austria > 30+] Retargeting` | Classic HTML5 | €5.00 |
| `[Video > Non skippable > Muehviertel > 30+] 15 Sek Strom` | YouTube | €3.33 |

**Note:** Retargeting uses Classic HTML5 ONLY. No Responsive Display for Retargeting.

### Meta Campaigns

| Campaign Name | Platform | Objective | Lifetime Budget |
|---------------|----------|-----------|-----------------|
| `[Awareness > Auction > Muehviertel > 30+] Gruenstrom` | Facebook | Awareness | €300 |
| `[Traffic > Auction > Muehviertel > 30+] Genossenschaft` | Facebook | Traffic | (part of above) |
| `[Traffic > Auction > Muehviertel > 30+] Carousels` | Facebook | Traffic | (part of above) |
| `[Traffic > Auction > Retargeting] FB Retargeting` | Facebook | Traffic | €200 |
| `[Awareness > Auction > Muehviertel > 30+] IG Gruenstrom` | Instagram | Awareness | €250 |
| `[Traffic > Auction > Muehviertel > 30+] IG Genossenschaft` | Instagram | Traffic | (part of above) |
| `[Traffic > Auction > Retargeting] IG Retargeting` | Instagram | Traffic | €110 |

---

## 15. Key Messages Reference

### Testimonial Priority for Bürger Target Group
1. Sarah (Bürger:in) Primary
2. Peter (Landwirtschaft) Secondary
3. Susanne (Gemeinde) Tertiary
4. Norbert (Alle) Quaternary

### Landing Page URLs
- Homepage: https://www.regios.at
- Grünstrom: https://www.regios.at/regionaler-gruenstrom
- Beteiligung: https://www.regios.at/beteiligung
- Bürger: https://www.regios.at/buerger

### Key Branded Messages (MUST USE)
- **Main Tagline:** Strom vom Mühlviertel: Fair, Regional und Grün
- **Dialect Slogan 1:** Mia san ned Deppad
- **Dialect Slogan 2:** Mia Mühlviertel san ned Deppad
- **Dialect CTA:** Mia Mühlviertel entscheiden selber wie es uns weitergeht
- **Regional Pride:** Zeigen wir was unser kleines Bauernland drauf hat!
- **Energy Elements:** Unser Wasser, Unsere Sonne, Unser Wind, UNSERE ENERGIE REGIOS
- **Values:** Unsere Stabilität, Unsere Sicherheit, Unsere Zukunft, UNSERE ENERGIE REGIOS
- **Regional Identity:** UNSER MÜHLVIERTEL, UNSERE ENERGIE REGIOS
- **CTA 1:** Stärken wir gemeinsam das Mühlviertel
- **CTA 2:** Investiere in die Stabilität des Mühlviertel
- **CTA 3:** Mach jetzt gleich mit bei der Energiegenossenschaft
- **Social Proof:** Über 2 Millionen Euro wurden schon in das Mühlviertel investiert
- **Social Proof:** Über 18 Gemeinden aus dem Mühlviertel sind schon dabei
- **Social Proof:** Über 15 Leitbetriebe aus dem Mühlviertel sind schon dabei

### Testimonial Slogans
- Unsere Sarah, Unsere Bürger:in, Unser Mühlviertel, UNSERE ENERGIE REGIOS
- Unsere Sarah, Unsere Gemeinschaft, UNSERE ENERGIE REGIOS
- Unsere Susanne, Unsere Gemeinde, Unser Mühlviertel, UNSERE ENERGIE REGIOS
- Unsere Susanne, Unsere Lebensqualität, UNSERE ENERGIE REGIOS
- Unsere Jakob, Unsere Bauern, Unser Mühlviertel, UNSERE ENERGIE REGIOS
- Unsere Norbert, Unsere Unabhängigkeit, UNSERE ENERGIE REGIOS
- Unser Christian, Unsere Stabilität, UNSERE ENERGIE REGIOS

---

*Document Version: 3.0*  
*Created: December 2024*  
*Updated: Fixed Display campaigns (HTML5 for retargeting only), reallocated budget, added asset mapping*  
*Campaign Period: 30 Days*  
*Total Budget: EUR 1,500*

---

## Contact

This campaign setup was created by:

**Keferboeck Ltd.**

For questions or support, please contact: 📧 **georg@keferboeck.com**
