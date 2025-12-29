# Regios Energiegenossenschaft - Campaign Setup Documentation

**Campaign Period:** 30 Days  
**Total Budget:** EUR 1,500  
**Target Region:** Mühlviertel (Meta) / Upper Austria (Google)  
**Target Audience:** Male & Female, 30+, Property Owners  
**Products:** Beteiligung (Genossenschaft) & Regionaler Grünstrom

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
| **Google** | Display Targeting | €8.00 | €240 | 16% |
| **Google** | Display Retargeting | €5.00 | €150 | 10% |
| **Google** | YouTube (Optional) | €3.33 | €100 | 7% |
| **Meta** | Facebook Targeting | €10.00 | €300 | 20% |
| **Meta** | Facebook Retargeting | €6.67 | €200 | 13% |
| **Meta** | Instagram Targeting | €8.33 | €250 | 17% |
| **Meta** | Instagram Retargeting | €3.67 | €110 | 7% |
| **Total** | | **€50.00** | **€1,500** | **100%** |

### Budget Rationale (Based on Historical Performance)

- Meta campaigns showed best Cost per Result: €0.22-0.34 per link click
- Google Display CPM: €1.13-7.98 (variable)
- YouTube Non-skippable CPM: €6.42-6.67
- Prioritize Meta for volume, Google for reach/retargeting

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
- Age: 30-65+
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
| Headline 3 | Strom aus dem Mühlviertel |
| Headline 4 | Von Bürger:innen für Bürger:innen |
| Headline 5 | Jetzt Mitglied werden |
| Headline 6 | 18+ Gemeinden dabei |
| Headline 7 | Über 2 Mio. € investiert |
| Headline 8 | Regionale Energieversorgung |
| Description 1 | Regios steht für faire, sichere und nachhaltige Energieversorgung im Mühlviertel. Jetzt informieren und Teil der Bewegung werden! |
| Description 2 | Stärken wir gemeinsam das Mühlviertel. Über 15 Leitbetriebe und 18 Gemeinden sind bereits dabei. Investiere in Stabilität. |
| Description 3 | Grüne Energie aus Sonne, Wind und Wasser. Ein Modell für regionale Selbstbestimmung und wirtschaftliche Stabilität. |
| Description 4 | Von Bürger:innen, für Bürger:innen. Gemeinsam schaffen wir Unabhängigkeit und eine nachhaltige Zukunft fürs Mühlviertel. |

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
-job
-jobs
-karriere
-arbeit
-praktikum
-kostenlos
-gratis
-preis
-vergleich
-billig
-günstig
-wechsel
-kündigen
```

**Responsive Search Ad:**

| Field | Content |
|-------|---------|
| Final URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=cpc&utm_campaign=gruenstrom_search_generic&utm_content=rsa_generic&utm_term={keyword}` |
| Headline 1 | Grünstrom aus dem Mühlviertel |
| Headline 2 | Regionale Energiegenossenschaft |
| Headline 3 | Fair, Regional & Nachhaltig |
| Headline 4 | Strom aus Sonne, Wind & Wasser |
| Headline 5 | Energieversorgung von hier |
| Headline 6 | Jetzt Teil werden |
| Headline 7 | Stabilität für die Region |
| Headline 8 | Von Bürger:innen getragen |
| Description 1 | Regionaler Grünstrom aus dem Mühlviertel. Faire Energie aus Sonnen-, Wind- und Wasserkraft. Von Bürger:innen, für Bürger:innen. |
| Description 2 | Investiere in die Stabilität des Mühlviertels. Über 2 Mio. € wurden bereits in die Region investiert. Jetzt informieren! |
| Description 3 | Die Energiegenossenschaft fürs Mühlviertel. Selbstbestimmung, Stabilität und eine unabhängige Zukunft. Mach jetzt mit! |

---

## 4. Google Display Campaigns

### Campaign A: Targeting - Grünstrom

**Campaign:** `[Display > Classic > Targeting > Upper Austria > 30+] Gruenstrom`

**Settings:**

| Setting | Value |
|---------|-------|
| Campaign Type | Display |
| Campaign Subtype | Standard Display |
| Goal | Website Traffic |
| Network | Display Network |
| Location | Upper Austria, Austria |
| Language | German |
| Bid Strategy | Target CPM (€3.00) |
| Daily Budget | €4.00 |
| Frequency Cap | 5 impressions per user per day |

**Audience Targeting:**
- Age: 30-65+
- Gender: All
- Household Income: Top 50%
- Affinity Audiences: Green Living Enthusiasts, Home & Garden/Home Improvement
- In-Market: Business Services/Utilities, Real Estate/Residential Properties

**Ad Group 1: Sonne**

**Responsive Display Ad:**

| Field | Content |
|-------|---------|
| Final URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=display&utm_campaign=gruenstrom_tofu_sonne&utm_content=responsive_display` |
| Headline 1 | Sonnenenergie aus dem Mühlviertel |
| Headline 2 | Unsere Sonne – UNSERE ENERGIE |
| Headline 3 | Regional. Fair. Grün. |
| Long Headline | Unsere Sonne, Unser Mühlviertel – Grüne Energie von Bürger:innen für Bürger:innen |
| Description 1 | Stärken wir gemeinsam das Mühlviertel. Investiere in die Stabilität der Region. |
| Description 2 | Über 2 Millionen Euro wurden schon in das Mühlviertel investiert. Jetzt mitmachen! |
| Business Name | Regios Energiegenossenschaft |

**Ad Group 2: Wasser**

**Responsive Display Ad:**

| Field | Content |
|-------|---------|
| Final URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=display&utm_campaign=gruenstrom_tofu_wasser&utm_content=responsive_display` |
| Headline 1 | Wasserkraft aus dem Mühlviertel |
| Headline 2 | Unser Wasser – UNSERE ENERGIE |
| Headline 3 | Regional. Fair. Grün. |
| Long Headline | Unser Wasser, Unser Mühlviertel – Grüne Energie von Bürger:innen für Bürger:innen |
| Description 1 | Stärken wir gemeinsam das Mühlviertel. Investiere in die Stabilität der Region. |
| Description 2 | Über 18 Gemeinden aus dem Mühlviertel sind schon dabei. Werde Teil der Bewegung! |
| Business Name | Regios Energiegenossenschaft |

**Ad Group 3: Wind**

**Responsive Display Ad:**

| Field | Content |
|-------|---------|
| Final URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=display&utm_campaign=gruenstrom_tofu_wind&utm_content=responsive_display` |
| Headline 1 | Windenergie aus dem Mühlviertel |
| Headline 2 | Unser Wind – UNSERE ENERGIE |
| Headline 3 | Regional. Fair. Grün. |
| Long Headline | Unser Wind, Unser Mühlviertel – Grüne Energie von Bürger:innen für Bürger:innen |
| Description 1 | Stärken wir gemeinsam das Mühlviertel. Investiere in die Stabilität der Region. |
| Description 2 | Über 15 Leitbetriebe aus dem Mühlviertel sind schon dabei. Jetzt informieren! |
| Business Name | Regios Energiegenossenschaft |

---

### Campaign B: Targeting - Genossenschaft

**Campaign:** `[Display > Classic > Targeting > Upper Austria > 30+] Genossenschaft`

**Settings:**

| Setting | Value |
|---------|-------|
| Campaign Type | Display |
| Campaign Subtype | Standard Display |
| Goal | Website Traffic |
| Network | Display Network |
| Location | Upper Austria, Austria |
| Language | German |
| Bid Strategy | Target CPM (€3.00) |
| Daily Budget | €4.00 |
| Frequency Cap | 5 impressions per user per day |

**Ad Group 1: Stabilität**

**Responsive Display Ad:**

| Field | Content |
|-------|---------|
| Final URL | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=display&utm_campaign=genossenschaft_tofu_stabilitaet&utm_content=responsive_display` |
| Headline 1 | Stabilität fürs Mühlviertel |
| Headline 2 | Unsere Stabilität – UNSERE ENERGIE |
| Headline 3 | Investiere in die Region |
| Long Headline | Unsere Stabilität, Unsere Sicherheit, Unsere Zukunft – UNSERE ENERGIE REGIOS |
| Description 1 | Investiere in die Stabilität des Mühlviertels. Über 2 Mio. € bereits in die Region investiert. |
| Description 2 | Regios – das Energiemodell für regionale Stabilität, Unabhängigkeit und Zukunft. |
| Business Name | Regios Energiegenossenschaft |

**Ad Group 2: Zukunft**

**Responsive Display Ad:**

| Field | Content |
|-------|---------|
| Final URL | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=display&utm_campaign=genossenschaft_tofu_zukunft&utm_content=responsive_display` |
| Headline 1 | Zukunft fürs Mühlviertel |
| Headline 2 | Unsere Zukunft – UNSERE ENERGIE |
| Headline 3 | Gemeinsam stark |
| Long Headline | Ein Modell für regionale Selbstbestimmung, Stabilität und eine lebenswerte Zukunft |
| Description 1 | Mach jetzt mit bei der Energiegenossenschaft. Über 18 Gemeinden sind schon dabei! |
| Description 2 | Von Bürger:innen, für Bürger:innen. Gemeinsam schaffen wir Unabhängigkeit. |
| Business Name | Regios Energiegenossenschaft |

**Ad Group 3: Mitgliedschaft**

**Responsive Display Ad:**

| Field | Content |
|-------|---------|
| Final URL | `https://www.regios.at/beteiligung?utm_source=google&utm_medium=display&utm_campaign=genossenschaft_tofu_mitgliedschaft&utm_content=responsive_display` |
| Headline 1 | Werde Mitglied bei Regios |
| Headline 2 | Gemeinsames Eigentum |
| Headline 3 | Die Genossenschaft fürs Mühlviertel |
| Long Headline | Selbstbestimmung über die regionale Energieversorgung durch gemeinsames Eigentum |
| Description 1 | Stärken wir gemeinsam das Mühlviertel. Jetzt Teil der Energiegenossenschaft werden! |
| Description 2 | 250.000 Bürger:innen im Mühlviertel. Zeigen wir, was wir gemeinsam schaffen können! |
| Business Name | Regios Energiegenossenschaft |

---

## 5. Google YouTube Campaigns

### Recommendation on YouTube

**Cost Analysis:**
- Historical YouTube Non-skippable CPM: €6.42-€6.67
- With €100 budget: ~15,000 impressions expected
- Reach in Mühlviertel limited due to geo-targeting

**Recommendation:** Include YouTube with limited budget (€100) for brand awareness. Use 15-second non-skippable for cost efficiency.

### Campaign: YouTube Targeting - Grünstrom

**Campaign:** `[Video > Non-skippable > Muehviertel > 30+] 15 Sek Strom`

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
- Age: 30-65+
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
| Headline | Sonnenenergie aus dem Mühlviertel |

**Ad Group 2: Wasser**

| Field | Content |
|-------|---------|
| Video | `15 Sek Strom - Wasser - Online - 16-9 - V1.mp4` |
| Final URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=video&utm_campaign=gruenstrom_tofu_wasser&utm_content=video15_wasser_16x9` |
| Display URL | regios.at |
| CTA | Mehr erfahren |
| Headline | Wasserkraft aus dem Mühlviertel |

**Ad Group 3: Wind**

| Field | Content |
|-------|---------|
| Video | `15 Sek Strom - Wind - Online - 16-9 - V1.mp4` |
| Final URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=video&utm_campaign=gruenstrom_tofu_wind&utm_content=video15_wind_16x9` |
| Display URL | regios.at |
| CTA | Mehr erfahren |
| Headline | Windenergie aus dem Mühlviertel |

---

## 6. Meta Facebook Campaigns

### Campaign A: Targeting - Grünstrom

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
| Location | Mühlviertel region (Freistadt, Perg, Rohrbach, Urfahr-Umgebung districts) |
| Age | 30-65+ |
| Gender | All |
| Detailed Targeting | Interests: Renewable energy, Sustainability, Home ownership, Local community |
| Optimization Goal | Reach |
| Frequency Cap | 2 per week |
| Attribution | 7-day click, 1-day view |

**Ad 1: Sonne - Post (1:1)**

| Field | Content |
|-------|---------|
| Video | `15 Sek Strom - Sonne - Online - 1-1 - V1.mp4` |
| Primary Text | ☀️ Unsere Sonne, Unser Mühlviertel – UNSERE ENERGIE REGIOS<br><br>Strom vom Mühlviertel: Fair, Regional und Grün.<br><br>Über 2 Millionen Euro wurden schon in das Mühlviertel investiert. Stärken wir gemeinsam die Region!<br><br>🌱 Von Bürger:innen, für Bürger:innen. |
| Headline | Grünstrom aus dem Mühlviertel |
| CTA | Learn More |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=facebook&utm_medium=social&utm_campaign=gruenstrom_tofu_sonne&utm_content=video15_sonne_1x1` |

**Ad 2: Wasser - Post (1:1)**

| Field | Content |
|-------|---------|
| Video | `15 Sek Strom - Wasser - Online - 1-1 - V1.mp4` |
| Primary Text | 💧 Unser Wasser, Unser Mühlviertel – UNSERE ENERGIE REGIOS<br><br>Regionale Wasserkraft für eine nachhaltige Zukunft.<br><br>Über 18 Gemeinden aus dem Mühlviertel sind schon dabei!<br><br>🌱 Fair. Regional. Grün. |
| Headline | Wasserkraft aus dem Mühlviertel |
| CTA | Learn More |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=facebook&utm_medium=social&utm_campaign=gruenstrom_tofu_wasser&utm_content=video15_wasser_1x1` |

**Ad 3: Wind - Post (1:1)**

| Field | Content |
|-------|---------|
| Video | `15 Sek Strom - Wind - Online - 1-1 - V1.mp4` |
| Primary Text | 🌬️ Unser Wind, Unser Mühlviertel – UNSERE ENERGIE REGIOS<br><br>Windenergie aus der Region, für die Region.<br><br>Über 15 Leitbetriebe aus dem Mühlviertel sind schon dabei!<br><br>🌱 Gemeinsam stark. |
| Headline | Windenergie aus dem Mühlviertel |
| CTA | Learn More |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=facebook&utm_medium=social&utm_campaign=gruenstrom_tofu_wind&utm_content=video15_wind_1x1` |

**Ad 4: Sonne - Story (9:16)**

| Field | Content |
|-------|---------|
| Video | `15 Sek Strom - Sonne - Online - 9-16 - V3.mp4` |
| Primary Text | ☀️ Unsere Sonne – UNSERE ENERGIE |
| CTA | Swipe Up |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=facebook&utm_medium=social&utm_campaign=gruenstrom_tofu_sonne&utm_content=story15_sonne_9x16` |

**Ad 5: Wasser - Story (9:16)**

| Field | Content |
|-------|---------|
| Video | `15 Sek Strom - Wasser - Online - 9-16 - V3.mp4` |
| Primary Text | 💧 Unser Wasser – UNSERE ENERGIE |
| CTA | Swipe Up |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=facebook&utm_medium=social&utm_campaign=gruenstrom_tofu_wasser&utm_content=story15_wasser_9x16` |

**Ad 6: Wind - Story (9:16)**

| Field | Content |
|-------|---------|
| Video | `15 Sek Strom - Wind - Online - 9-16 - V3.mp4` |
| Primary Text | 🌬️ Unser Wind – UNSERE ENERGIE |
| CTA | Swipe Up |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=facebook&utm_medium=social&utm_campaign=gruenstrom_tofu_wind&utm_content=story15_wind_9x16` |

**Ad 7: Strom 30s - Post (1:1)**

| Field | Content |
|-------|---------|
| Video | `30 Sek Kurz - Strom - TV - 1-1 - V1 ohne URL.mp4` |
| Primary Text | 🌱 Strom vom Mühlviertel: Fair, Regional und Grün<br><br>Regios Energiegenossenschaft steht für faire, sichere und nachhaltige Energieversorgung – von Bürger:innen, für Bürger:innen.<br><br>✔ Über 2 Mio. € bereits in die Region investiert<br>✔ 18+ Gemeinden & 15 Leitbetriebe dabei<br><br>Stärken wir gemeinsam das Mühlviertel! |
| Headline | UNSERE ENERGIE REGIOS |
| CTA | Learn More |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=facebook&utm_medium=social&utm_campaign=gruenstrom_tofu_alle&utm_content=video30_strom_1x1` |

---

### Campaign B: Targeting - Genossenschaft

**Campaign:** `[Traffic > Auction > Muehviertel > 30+] Genossenschaft`

**Campaign Settings:**

| Setting | Value |
|---------|-------|
| Campaign Objective | Traffic |
| Buying Type | Auction |
| Campaign Budget Optimization | On |
| Campaign Budget | €150 (Lifetime) |
| Campaign Bid Strategy | Lowest cost |

**Ad 1: Genossenschaft - Post (1:1)**

| Field | Content |
|-------|---------|
| Video | `30 Sek Kurz - Genossenschaft - TV - 1-1 - V1 ohne URL.mp4` |
| Primary Text | 🤝 Unsere Stabilität, Unsere Sicherheit, Unsere Zukunft – UNSERE ENERGIE REGIOS<br><br>Regios ist mehr als Strom: Es ist ein Modell für regionale Selbstbestimmung und wirtschaftliche Stabilität.<br><br>✔ Investitionspakete<br>✔ Grünstrom<br>✔ Grüne Pacht<br><br>Mach jetzt mit bei der Energiegenossenschaft! |
| Headline | Investiere in die Stabilität des Mühlviertels |
| CTA | Learn More |
| Website URL | `https://www.regios.at/beteiligung?utm_source=facebook&utm_medium=social&utm_campaign=genossenschaft_tofu_stabilitaet&utm_content=video30_genossenschaft_1x1` |

**Ad 2: Genossenschaft - Story (9:16)**

| Field | Content |
|-------|---------|
| Video | `30 Sek Kurz - Genossenschaft - TV - 9-16 - V1 ohne URL.mp4` |
| Primary Text | 🤝 UNSERE ENERGIE REGIOS |
| CTA | Swipe Up |
| Website URL | `https://www.regios.at/beteiligung?utm_source=facebook&utm_medium=social&utm_campaign=genossenschaft_tofu_stabilitaet&utm_content=story30_genossenschaft_9x16` |

**Ad 3: Genossenschaft Sonne - Post (1:1)**

| Field | Content |
|-------|---------|
| Video | `15 Sek Genossenschaft - Sonne - Online - 1-1 - V1.mp4` |
| Primary Text | ☀️ Investiere in Sonnenenergie aus dem Mühlviertel<br><br>Werde Teil der Regios Energiegenossenschaft und profitiere von nachhaltigen Investitionspaketen.<br><br>🌱 Von Bürger:innen, für Bürger:innen. |
| Headline | Beteiligung an Sonnenenergie |
| CTA | Learn More |
| Website URL | `https://www.regios.at/beteiligung?utm_source=facebook&utm_medium=social&utm_campaign=genossenschaft_tofu_sonne&utm_content=video15_genossenschaft_sonne_1x1` |

---

### Campaign C: Targeting - Carousels

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
| Primary Text | ☀️ Unsere Sonne, Unser Mühlviertel – UNSERE ENERGIE REGIOS<br><br>Entdecke, wie Sonnenenergie aus der Region unsere Zukunft gestaltet. |
| Card Headlines | 1: Unsere Sonne / 2: Unser Mühlviertel / 3: Unsere Energie / 4: Unsere Zukunft / 5: REGIOS |
| CTA | Learn More |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=facebook&utm_medium=social&utm_campaign=gruenstrom_tofu_sonne&utm_content=carousel_sonne_1080x1080` |

**Carousel Ad 2: Wasser**

| Field | Content |
|-------|---------|
| Images | wasser_1080x1080_1.png through wasser_1080x1080_5.png |
| Primary Text | 💧 Unser Wasser, Unser Mühlviertel – UNSERE ENERGIE REGIOS<br><br>Wasserkraft aus der Region für eine nachhaltige Energiezukunft. |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=facebook&utm_medium=social&utm_campaign=gruenstrom_tofu_wasser&utm_content=carousel_wasser_1080x1080` |

**Carousel Ad 3: Wind**

| Field | Content |
|-------|---------|
| Images | WInd_1080x1080_1.png through WInd_1080x1080_5.png |
| Primary Text | 🌬️ Unser Wind, Unser Mühlviertel – UNSERE ENERGIE REGIOS<br><br>Windenergie aus dem Mühlviertel – regional und nachhaltig. |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=facebook&utm_medium=social&utm_campaign=gruenstrom_tofu_wind&utm_content=carousel_wind_1080x1080` |

**Carousel Ad 4: Stabilität**

| Field | Content |
|-------|---------|
| Images | Stabilitaet_1080x1080_1.png through Stabilitaet_1080x1080_5.png |
| Primary Text | 🤝 Unsere Stabilität – UNSERE ENERGIE REGIOS<br><br>Investiere in die wirtschaftliche Stabilität des Mühlviertels. Gemeinsam sind wir stark! |
| Website URL | `https://www.regios.at/beteiligung?utm_source=facebook&utm_medium=social&utm_campaign=genossenschaft_tofu_stabilitaet&utm_content=carousel_stabilitaet_1080x1080` |

**Carousel Ad 5: Zukunft**

| Field | Content |
|-------|---------|
| Images | Zukunft_1080x1080_1.png through Zukunft_1080x1080_5.png |
| Primary Text | 🌱 Unsere Zukunft – UNSERE ENERGIE REGIOS<br><br>Ein Modell für regionale Selbstbestimmung und eine lebenswerte Zukunft. |
| Website URL | `https://www.regios.at/beteiligung?utm_source=facebook&utm_medium=social&utm_campaign=genossenschaft_tofu_zukunft&utm_content=carousel_zukunft_1080x1080` |

---

## 7. Meta Instagram Campaigns

### Campaign A: Targeting - Grünstrom (Instagram)

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
| Age | 30-65+ |
| Gender | All |

**Ad 1: Sonne - Post**

| Field | Content |
|-------|---------|
| Video | `15 Sek Strom - Sonne - Online - 1-1 - V1.mp4` |
| Caption | ☀️ Unsere Sonne, Unser Mühlviertel – UNSERE ENERGIE REGIOS<br><br>Strom vom Mühlviertel: Fair, Regional und Grün. 🌱<br><br>Über 2 Millionen Euro wurden schon in das Mühlviertel investiert. Stärken wir gemeinsam die Region!<br><br>#regios #mühlviertel #grünstrom #energiegenossenschaft #nachhaltigkeit #sonnenenergie #oberösterreich |
| CTA | Learn More |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=instagram&utm_medium=social&utm_campaign=gruenstrom_tofu_sonne&utm_content=video15_sonne_1x1` |

**Ad 2: Wasser - Post**

| Field | Content |
|-------|---------|
| Video | `15 Sek Strom - Wasser - Online - 1-1 - V1.mp4` |
| Caption | 💧 Unser Wasser, Unser Mühlviertel – UNSERE ENERGIE REGIOS<br><br>Regionale Wasserkraft für eine nachhaltige Zukunft. 🌱<br><br>Über 18 Gemeinden sind schon dabei!<br><br>#regios #mühlviertel #wasserkraft #energiegenossenschaft #nachhaltigkeit #oberösterreich |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=instagram&utm_medium=social&utm_campaign=gruenstrom_tofu_wasser&utm_content=video15_wasser_1x1` |

**Ad 3: Wind - Post**

| Field | Content |
|-------|---------|
| Video | `15 Sek Strom - Wind - Online - 1-1 - V1.mp4` |
| Caption | 🌬️ Unser Wind, Unser Mühlviertel – UNSERE ENERGIE REGIOS<br><br>Windenergie aus der Region, für die Region. 🌱<br><br>15+ Leitbetriebe sind schon dabei!<br><br>#regios #mühlviertel #windenergie #energiegenossenschaft #nachhaltigkeit #oberösterreich |
| Website URL | `https://www.regios.at/regionaler-gruenstrom?utm_source=instagram&utm_medium=social&utm_campaign=gruenstrom_tofu_wind&utm_content=video15_wind_1x1` |

**Ad 4-6: Stories (9:16)** - Same as Facebook Stories with Instagram URLs

---

### Campaign B: Targeting - Genossenschaft (Instagram)

**Campaign:** `[Traffic > Auction > Muehviertel > 30+] IG Genossenschaft`

**Campaign Settings:**

| Setting | Value |
|---------|-------|
| Campaign Objective | Traffic |
| Campaign Budget | €125 (Lifetime) |

**Ad 1: Genossenschaft - Post (1:1)**

| Field | Content |
|-------|---------|
| Video | `30 Sek Kurz - Genossenschaft - TV - 1-1 - V1 ohne URL.mp4` |
| Caption | 🤝 UNSERE ENERGIE REGIOS<br><br>Unsere Stabilität. Unsere Sicherheit. Unsere Zukunft.<br><br>Regios ist mehr als Strom: Ein Modell für regionale Selbstbestimmung und wirtschaftliche Stabilität.<br><br>Mach jetzt mit bei der Energiegenossenschaft! 🌱<br><br>#regios #genossenschaft #investieren #mühlviertel #nachhaltigkeit |
| CTA | Learn More |
| Website URL | `https://www.regios.at/beteiligung?utm_source=instagram&utm_medium=social&utm_campaign=genossenschaft_tofu_stabilitaet&utm_content=video30_genossenschaft_1x1` |

**Carousel Ad: Sarah (Bürger:in)**

| Field | Content |
|-------|---------|
| Images | Sarah_1080x1080_1.png through sarah_1080x1080_5.png |
| Caption | 👩 Unsere Sarah, Unsere Bürger:in, Unser Mühlviertel – UNSERE ENERGIE REGIOS<br><br>Von Bürger:innen, für Bürger:innen. Gemeinsam schaffen wir Stabilität und Zukunft! 🌱<br><br>#regios #mühlviertel #gemeinschaft #energiegenossenschaft |
| Website URL | `https://www.regios.at/buerger?utm_source=instagram&utm_medium=social&utm_campaign=genossenschaft_tofu_testimonial&utm_content=carousel_sarah_1080x1080` |

---

## 8. Retargeting Campaigns

### Google Display Retargeting

**Campaign:** `[Display > Classic > Retargeting > Upper Austria > 30+] Retargeting`

**Settings:**

| Setting | Value |
|---------|-------|
| Campaign Type | Display |
| Goal | Website Traffic |
| Bid Strategy | Target CPA (€2.00) |
| Daily Budget | €5.00 |
| Frequency Cap | 3 impressions per user per day |

**Audience Targeting:**
- Website Visitors (All) - Past 30 days
- Audience: Bürger
- Audience: Genossenschaft
- Audience: Grünstrom

**Ad Group 1: Grünstrom Retargeting**

**HTML5 Banners Available:**

| Theme | Sizes |
|-------|-------|
| Wasser | 300x250, 300x600, 320x50, 336x280, 728x90 |
| Wind | 300x250, 300x600, 320x50, 336x280, 728x90 |
| Licht (Sonne) | 300x250, 300x600, 320x50, 336x280, 728x90 |

**UTM URLs for Grünstrom Retargeting:**
```
https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=retargeting&utm_campaign=gruenstrom_mofu_retargeting&utm_content=banner_wasser_300x250
https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=retargeting&utm_campaign=gruenstrom_mofu_retargeting&utm_content=banner_wind_300x600
https://www.regios.at/regionaler-gruenstrom?utm_source=google&utm_medium=retargeting&utm_campaign=gruenstrom_mofu_retargeting&utm_content=banner_licht_728x90
```

**Ad Group 2: Genossenschaft Retargeting**

**HTML5 Banners Available:**

| Theme | Sizes |
|-------|-------|
| Stabilitaet | 160x600, 300x250, 300x600, 320x50, 320x100, 336x280, 728x90, 970x250 |
| Zukunft | 300x250, 300x600, 320x50, 336x280, 728x90 |
| Sarah | 300x250, 300x600, 320x50, 320x100, 336x280, 728x90 |

**UTM URLs for Genossenschaft Retargeting:**
```
https://www.regios.at/beteiligung?utm_source=google&utm_medium=retargeting&utm_campaign=genossenschaft_mofu_retargeting&utm_content=banner_stabilitaet_300x250
https://www.regios.at/beteiligung?utm_source=google&utm_medium=retargeting&utm_campaign=genossenschaft_mofu_retargeting&utm_content=banner_zukunft_728x90
https://www.regios.at/beteiligung?utm_source=google&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_retargeting&utm_content=banner_sarah_300x600
```

---

### Meta Retargeting Campaigns

**Campaign:** `[Traffic > Auction > Retargeting] Meta Retargeting`

**Campaign Settings:**

| Setting | Value |
|---------|-------|
| Campaign Objective | Traffic |
| Campaign Budget | €310 (Lifetime) |

**Custom Audiences to Use:**
1. Engagement: Paid Meta Ads (180 days)
2. Engagement: Meta Organic (180 days)
3. Engagement: Instagram/Facebook Subscription
4. Engagement: Messenger Contact
5. Website Visitors (via Pixel) - 30 days

**Ad Set 1: Testimonial Videos - Sarah (Priority 1)**

**Ad 1: Sarah - Warum Regios**

| Field | Content |
|-------|---------|
| Video | `Testimonial - Sarah - Short - Warum Regios.mp4` |
| Primary Text | 👩 „Warum Regios?" – Sarah aus dem Mühlviertel erzählt<br><br>Unsere Sarah, Unsere Gemeinschaft – UNSERE ENERGIE REGIOS<br><br>Erfahre, warum immer mehr Bürger:innen Teil der Energiegenossenschaft werden. |
| Headline | Sarah empfiehlt Regios |
| CTA | Learn More |
| Website URL | `https://www.regios.at/buerger?utm_source=facebook&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial_sarah&utm_content=testimonial_sarah_warum` |

**Ad 2: Sarah - Wertschöpfung**

| Field | Content |
|-------|---------|
| Video | `Testimonial - Sarah - Short - Wertschöpfung in der Region.mp4` |
| Primary Text | 👩 „Wertschöpfung in der Region" – Sarah aus dem Mühlviertel<br><br>Über 2 Millionen Euro wurden schon in das Mühlviertel investiert. Stärken wir gemeinsam die Region! |
| Website URL | `https://www.regios.at/buerger?utm_source=facebook&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial_sarah&utm_content=testimonial_sarah_wertschoepfung` |

**Ad 3: Sarah - Gemeinsam Stark**

| Field | Content |
|-------|---------|
| Video | `Testimonial - Sarah - Short - Gemeinsam Stark.mp4` |
| Primary Text | 👩 „Gemeinsam Stark" – Sarah aus dem Mühlviertel<br><br>Von Bürger:innen, für Bürger:innen. Gemeinsam schaffen wir Stabilität und Zukunft! |
| Website URL | `https://www.regios.at/buerger?utm_source=facebook&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial_sarah&utm_content=testimonial_sarah_gemeinsam` |

**Ad 4: Sarah - Long Version**

| Field | Content |
|-------|---------|
| Video | `Testimonial - Sarah - Long - V1.mp4` |
| Primary Text | 👩 Sarah aus dem Mühlviertel – Die ganze Geschichte<br><br>Unsere Sarah, Unsere Bürger:in, Unser Mühlviertel – UNSERE ENERGIE REGIOS |
| Website URL | `https://www.regios.at/buerger?utm_source=facebook&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial_sarah&utm_content=testimonial_sarah_long` |

**Ad Set 2: Testimonial Videos - Peter (Priority 2 - Landwirtschaft)**

**Ad 5: Peter - Doppelnutzung**

| Field | Content |
|-------|---------|
| Video | `Testimonial - Peter - Short - Doppelnutzung.mp4` |
| Primary Text | 👨‍🌾 „Doppelnutzung" – Peter, Landwirt aus dem Mühlviertel<br><br>Erfahre, wie Landwirte von der Energiegenossenschaft profitieren. |
| Website URL | `https://www.regios.at/buerger?utm_source=facebook&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial_peter&utm_content=testimonial_peter_doppelnutzung` |

**Ad 6: Peter - Long Version**

| Field | Content |
|-------|---------|
| Video | `Testimonial - Peter - Long - V1.mp4` |
| Primary Text | 👨‍🌾 Peter aus dem Mühlviertel – Die ganze Geschichte<br><br>Unsere Jakob, Unsere Bauern, Unser Mühlviertel – UNSERE ENERGIE REGIOS |
| Website URL | `https://www.regios.at/buerger?utm_source=facebook&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial_peter&utm_content=testimonial_peter_long` |

**Ad Set 3: Testimonial Videos - Susanne (Priority 3 - Gemeinde)**

**Ad 7: Susanne - Warum Regios**

| Field | Content |
|-------|---------|
| Video | `Testimonial - Susanne - Short - Warum Regios.mp4` |
| Primary Text | 👩‍💼 „Warum Regios?" – Susanne, Gemeindevertreterin<br><br>Unsere Susanne, Unsere Gemeinde, Unser Mühlviertel – UNSERE ENERGIE REGIOS<br><br>Über 18 Gemeinden aus dem Mühlviertel sind schon dabei! |
| Website URL | `https://www.regios.at/buerger?utm_source=facebook&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial_susanne&utm_content=testimonial_susanne_warum` |

**Ad 8: Susanne - Long Version**

| Field | Content |
|-------|---------|
| Video | `Testimonial - Susanne - Long - mit Abbinder - V1.mp4` |
| Primary Text | 👩‍💼 Susanne – Die ganze Geschichte<br><br>Unsere Susanne, Unsere Lebensqualität – UNSERE ENERGIE REGIOS |
| Website URL | `https://www.regios.at/buerger?utm_source=facebook&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial_susanne&utm_content=testimonial_susanne_long` |

**Ad Set 4: Testimonial Videos - Norbert (Priority 4 - Alle)**

**Ad 9: Norbert - Sicherheit**

| Field | Content |
|-------|---------|
| Video | `Testimonial - Norbert - Short - Sicherheit.mp4` |
| Primary Text | 👨 „Sicherheit" – Norbert aus dem Mühlviertel<br><br>Unsere Norbert, Unsere Unabhängigkeit – UNSERE ENERGIE REGIOS |
| Website URL | `https://www.regios.at/buerger?utm_source=facebook&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial_norbert&utm_content=testimonial_norbert_sicherheit` |

**Ad 10: Norbert - Long Version**

| Field | Content |
|-------|---------|
| Video | `Testimonial - Norbert - Long - mit Abbinder - V1.mp4` |
| Primary Text | 👨 Norbert aus dem Mühlviertel – Die ganze Geschichte<br><br>UNSERE ENERGIE REGIOS |
| Website URL | `https://www.regios.at/buerger?utm_source=facebook&utm_medium=retargeting&utm_campaign=genossenschaft_bofu_testimonial_norbert&utm_content=testimonial_norbert_long` |

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
| Bürger | `https://www.regios.at/buerger` | Citizen-focused landing page |
| Homepage | `https://www.regios.at` | Brand searches |

---

## 10. Audience Setup

### Google Audiences

**Remarketing Lists to Create:**

| Audience Name | Definition | Membership Duration |
|---------------|------------|---------------------|
| `Bürger` | Visitors to /buerger page | 90 days |
| `Genossenschaft` | Visitors to /beteiligung page | 90 days |
| `Grünstrom` | Visitors to /regionaler-gruenstrom page | 90 days |
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
| `Website: All Visitors` | Pixel - All visitors | 30 days |
| `Website: Grünstrom` | Pixel - /regionaler-gruenstrom | 60 days |
| `Website: Beteiligung` | Pixel - /beteiligung | 60 days |
| `Website: Bürger` | Pixel - /buerger | 60 days |
| `Video: 50% Viewed` | People who watched 50%+ of videos | 90 days |
| `Video: 75% Viewed` | People who watched 75%+ of videos | 90 days |

---

## 11. Asset Mapping

### Video Assets - Targeting

| Platform | Placement | Product | Theme | Duration | Aspect | File Path |
|----------|-----------|---------|-------|----------|--------|-----------|
| Meta | Post | Grünstrom | Sonne | 15s | 1:1 | Social Media/Targeting/Video/15 Sek - Strom/15 Sek Strom - Sonne - Online - 1-1 - V1.mp4 |
| Meta | Post | Grünstrom | Wasser | 15s | 1:1 | Social Media/Targeting/Video/15 Sek - Strom/15 Sek Strom - Wasser - Online - 1-1 - V1.mp4 |
| Meta | Post | Grünstrom | Wind | 15s | 1:1 | Social Media/Targeting/Video/15 Sek - Strom/15 Sek Strom - Wind - Online - 1-1 - V1.mp4 |
| Meta | Story | Grünstrom | Sonne | 15s | 9:16 | Social Media/Targeting/Video/15 Sek - Strom/15 Sek Strom - Sonne - Online - 9-16 - V3.mp4 |
| Meta | Story | Grünstrom | Wasser | 15s | 9:16 | Social Media/Targeting/Video/15 Sek - Strom/15 Sek Strom - Wasser - Online - 9-16 - V3.mp4 |
| Meta | Story | Grünstrom | Wind | 15s | 9:16 | Social Media/Targeting/Video/15 Sek - Strom/15 Sek Strom - Wind - Online - 9-16 - V3.mp4 |
| Google | YouTube | Grünstrom | Sonne | 15s | 16:9 | Google/Targeting/Strom/15 Sek Strom - Sonne - Online - 16-9 - V1.mp4 |
| Google | YouTube | Grünstrom | Wasser | 15s | 16:9 | Google/Targeting/Strom/15 Sek Strom - Wasser - Online - 16-9 - V1.mp4 |
| Google | YouTube | Grünstrom | Wind | 15s | 16:9 | Google/Targeting/Strom/15 Sek Strom - Wind - Online - 16-9 - V1.mp4 |

### Testimonial Videos - Retargeting (Priority Order)

| Priority | Testimonial | Type | File Path |
|----------|-------------|------|-----------|
| 1 | Sarah | Short - Warum Regios | Testimonial - Sarah/Testimonial - Sarah - Short - Warum Regios.mp4 |
| 1 | Sarah | Short - Wertschöpfung | Testimonial - Sarah/Testimonial - Sarah - Short - Wertschöpfung in der Region.mp4 |
| 1 | Sarah | Short - Gemeinsam Stark | Testimonial - Sarah/Testimonial - Sarah - Short - Gemeinsam Stark.mp4 |
| 1 | Sarah | Long | Testimonial - Sarah/Testimonial - Sarah - Long - V1.mp4 |
| 2 | Peter | Short - Doppelnutzung | Testimonial - Peter/Testimonial - Peter - Short - Doppelnutzung.mp4 |
| 2 | Peter | Long | Testimonial - Peter/Testimonial - Peter - Long - V1.mp4 |
| 3 | Susanne | Short - Warum Regios | Testimonial - Susanne/Testimonial - Susanne - Short - Warum Regios.mp4 |
| 3 | Susanne | Long | Testimonial - Susanne/Testimonial - Susanne - Long - mit Abbinder - V1.mp4 |
| 4 | Norbert | Short - Sicherheit | Testimonial - Norbert/Testimonial - Norbert - Short - Sicherheit.mp4 |
| 4 | Norbert | Long | Testimonial - Norbert/Testimonial - Norbert - Long - mit Abbinder - V1.mp4 |

### HTML5 Banner Assets - Retargeting

| Theme | Sizes Available | Path |
|-------|-----------------|------|
| Stabilitaet | 160x600, 300x250, 300x600, 320x50, 320x100, 336x280, 728x90, 970x250 | Google/Retargeting/Banners/HTML5/Stabilitaet_*.zip |
| Zukunft | 300x250, 300x600, 320x50, 336x280, 728x90 | Google/Retargeting/Banners/HTML5/Zukunft_*.zip |
| Sarah | 300x250, 300x600, 320x50, 320x100, 336x280, 728x90 | Google/Retargeting/Banners/HTML5/Sarah_*.zip |
| Wasser | 300x250, 300x600, 320x50, 336x280, 728x90 | Google/Retargeting/Banners/HTML5/Wasser_*.zip |
| Wind | 300x250, 300x600, 320x50, 336x280, 728x90 | Google/Retargeting/Banners/HTML5/Wind_*.zip |
| Licht | 300x250, 300x600, 320x50, 336x280, 728x90 | Google/Retargeting/Banners/HTML5/Licht_*.zip |

### Carousel Image Assets

| Theme | Sizes | Cards | Path |
|-------|-------|-------|------|
| Sonne | 1080x1080 | 5 | Social Media/Targeting/Posts/Carousels/1080x1080/sonne/ |
| Wasser | 1080x1080 | 5 | Social Media/Targeting/Posts/Carousels/1080x1080/wasser/ |
| Wind | 1080x1080 | 5 | Social Media/Targeting/Posts/Carousels/1080x1080/wind/ |
| Stabilitaet | 1080x1080 | 5 | Social Media/Targeting/Posts/Carousels/1080x1080/Stabilitaet/ |
| Zukunft | 1080x1080 | 5 | Social Media/Targeting/Posts/Carousels/1080x1080/Zukunft/ |
| Sicherheit | 1080x1080 | 5 | Social Media/Targeting/Posts/Carousels/1080x1080/Sicherheit/ |
| Sarah | 1080x1080 | 5 | Social Media/Targeting/Posts/Carousels/1080x1080/sarah/ |
| Susanne | 1080x1080 | 5 | Social Media/Targeting/Posts/Carousels/1080x1080/susanne/ |

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

1. **Executive Summary** - Total Spend, Impressions, Clicks, Conversions
2. **Platform Performance** - Google vs Meta comparison
3. **Funnel Analysis** - TOFU/MOFU/BOFU metrics
4. **Product Performance** - Grünstrom vs Genossenschaft
5. **Creative Analysis** - Performance by theme
6. **Retargeting Analysis** - Testimonial performance

### Key Metrics to Track

| Metric | Target |
|--------|--------|
| Reach | 50,000+ |
| Frequency | 3-5x |
| CTR | 1%+ |
| CPC | < €0.50 |
| CPM | < €10 |
| Video Completion | 30%+ |
| CPA | < €25 |

---

## 13. Campaign Checklist

### Pre-Launch Checklist

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

## 14. Quick Reference - All Campaign Names

### Google Campaigns

| Campaign Name | Type | Daily Budget |
|---------------|------|--------------|
| `[Search > Brand+Generic > Upper Austria > 30+] Regios` | Search | €5.00 |
| `[Display > Classic > Targeting > Upper Austria > 30+] Gruenstrom` | Display | €4.00 |
| `[Display > Classic > Targeting > Upper Austria > 30+] Genossenschaft` | Display | €4.00 |
| `[Video > Non-skippable > Muehviertel > 30+] 15 Sek Strom` | YouTube | €3.33 |
| `[Display > Classic > Retargeting > Upper Austria > 30+] Retargeting` | Display RT | €5.00 |

### Meta Campaigns

| Campaign Name | Platform | Objective | Lifetime Budget |
|---------------|----------|-----------|-----------------|
| `[Awareness > Auction > Muehviertel > 30+] Gruenstrom` | Facebook | Awareness | €150 |
| `[Traffic > Auction > Muehviertel > 30+] Genossenschaft` | Facebook | Traffic | €150 |
| `[Traffic > Auction > Muehviertel > 30+] Carousels` | Facebook | Traffic | €100 |
| `[Awareness > Auction > Muehviertel > 30+] IG Gruenstrom` | Instagram | Awareness | €125 |
| `[Traffic > Auction > Muehviertel > 30+] IG Genossenschaft` | Instagram | Traffic | €125 |
| `[Traffic > Auction > Retargeting] Meta Retargeting` | FB + IG | Traffic | €310 |

---

## 15. Key Messages Reference

**Testimonial Priority for Bürger Target Group:**
1. Sarah (Bürger:in) - Primary
2. Peter (Landwirtschaft) - Secondary
3. Susanne (Gemeinde) - Tertiary
4. Norbert (Alle) - Quaternary

**Landing Page URLs:**
- Homepage: https://www.regios.at
- Grünstrom: https://www.regios.at/regionaler-gruenstrom
- Beteiligung: https://www.regios.at/beteiligung
- Bürger: https://www.regios.at/buerger

**Key Messages:**
- "Strom vom Mühlviertel: Fair, Regional und Grün"
- "Unsere Stabilität, Unsere Sicherheit, Unsere Zukunft – UNSERE ENERGIE REGIOS"
- "Von Bürger:innen, für Bürger:innen"
- "Stärken wir gemeinsam das Mühlviertel"

---

*Document Version: 1.0*  
*Created: December 2024*  
*Campaign Period: 30 Days*  
*Total Budget: EUR 1,500*
