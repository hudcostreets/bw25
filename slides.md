---
# You can also start simply with 'default'
theme: ./theme
title: data @ hudcostreets
info: |
  ## NJ Bike Walk Summit – 3/29/25
  Ryan Williams, Hudson County Complete Streets
selectable: true
# apply unocss classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# background: #00793e
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
# transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
layout: section
---

# Data @ Hudson County Complete Streets

[NJ Bike Walk Summit], 3/29/25

Ryan Williams

[NJ Bike Walk Summit]: https://njbwc.org/summit-2025/

---
class: hccs
---
# Hudson County Complete Streets
> Our mission is to improve connectivity and transportation equity in Hudson County by advocating for safe streets, pedestrian and cycling infrastructure, and access to transit in each community.

Campaigns:
- [Improving PATH service][PATH]
- [Supporting congestion pricing][CP]
- [Opposing $11BN Turnpike-widening][TA]
- [Hudson County Vision Zero Action Plan][VZ]

👉 [hudcostreets.org]

<style>
.slidev-layout.hccs {
  h1 { margin-bottom: 0 }
  p { margin: 0.4rem 0; }
  li { line-height: 2rem }
  blockquote { width: 75% }
  img {
    position: absolute;
    object-fit: cover;
    object-position: top center;
    /*TODO: put these in an actual grid*/
    &[src="/vz.png"] {
      right: 1.3%;
      /*top: 15%;*/
      bottom: 36%;
      width: 22.5%;
      /*height: 50%;*/
    }
    &[src="/path.jpg"] {
      width: 27%;
      height: 36.5%;
      bottom: 36%;
      right: 25%;
      object-fit: cover;
      object-position: top center;
    }
  }

  .imgs {
    display: flex;
    height: 32%;
    position: absolute;
    bottom: 2%;
    width: 100%;
    gap: 1.5%;
    & > div {
      flex: 0 0 auto; /* Don't grow or shrink */
      height: 100%;
      position: relative;
    }
    img {
      height: 100%;
      object-fit: contain;
      position: static;
      left: auto;
    }
  }
}
/* TODO: theme var */
.dark img { border: 1px solid white }
.light img { border: 3px solid #00793f }
</style>

<div class="imgs">
  <div><a href="https://turnpiketrap.org/"><img src="/tt.png"/></a></div>
  <div><a href="https://newsletter.hudcostreets.org/archive/save-our-hudson-county-buses-deadline-august-16/"><img src="/bus.jpeg"/></a></div>
  <div><a href="https://newsletter.hudcostreets.org/archive/action-alert-tell-gov-murphy-142m-for-nj-transit/"><img src="/njt.jpeg"/></a></div>
</div>
<a href="https://hudcostreets.org/panynj"><img src="/path.jpg"/></a>
<a href="https://newsletter.hudcostreets.org/archive/january-2025-vision-zero-plan-launch-jan-11/"><img src="/vz.png"/></a>

[PATH]: https://hudcostreets.org/panynj
[CP]: https://nyc.streetsblog.org/2025/03/21/advocates-demand-new-jersey-agencies-cough-up-congestion-pricing-data
[TA]: https://www.nj.com/traffic/2025/03/nj-turnpike-widening-opponents-demand-fresh-cost-and-traffic-numbers-for-107-b-project.html?gift=81525149-0b28-4c98-bd63-b6241996fd00
[VZ]: https://newsletter.hudcostreets.org/archive/january-2025-vision-zero-plan-launch-jan-11/

[hudcostreets.org]: https://hudcostreets.org/
[tt]: https://turnpiketrap.org/
[bus]: https://newsletter.hudcostreets.org/archive/save-our-hudson-county-buses-deadline-august-16/
[njt]: https://newsletter.hudcostreets.org/archive/action-alert-tell-gov-murphy-142m-for-nj-transit/
[vzi]: https://newsletter.hudcostreets.org/archive/january-2025-vision-zero-plan-launch-jan-11/

---
class: us
---
# Big picture – US transportation sector is broken
≈100% car-dependence:

- [\$TNs][IMF] of subsidies, [\$TNs][debt] of auto debt, [\$TNs][insurance] of auto insurance (other people's crashes)
- [MMs][deaths] of violent deaths, [10MMs][injuries] of injuries, [10MMs][disease] of respiratory diseases / cognitive impairments
- [MMmts][CO2] of CO₂; pollution / particulates / noise
- [Worse mobility][cn hsr], no childhood autonomy, hollowed-out cities, less community

[IMF]: https://www.imf.org/en/Topics/climate-change/energy-subsidies
[debt]: https://www.lendingtree.com/auto/debt-statistics/
[insurance]: https://www.statista.com/outlook/fmo/insurances/non-life-insurances/motor-vehicle-insurance/united-states
[deaths]: https://en.wikipedia.org/wiki/Motor_vehicle_fatality_rate_in_U.S._by_year#By_year
[injuries]: https://crashstats.nhtsa.dot.gov/Api/Public/ViewPublication/813560#:~:text=In%202022%20an%20estimated%202.38,injured%20from%202020%20to%202021.
[disease]: https://www.who.int/data/gho/data/themes/topics/indicator-groups/indicator-group-details/GHO/ambient-air-pollution
[CO2]: https://www.eia.gov/tools/faqs/faq.php?id=307&t=10

[shinkansen]: https://en.wikipedia.org/wiki/Shinkansen#Safety_record
[cn hsr]: https://www.threads.net/@thetransitguy/post/DGY0GP6B3hD/video-this-is-the-beijing-shanghai-corridor-which-takes-4-hours-and-18-minutes-to-cove
[world transit]: https://www.thetransportpolitic.com/2023/06/07/once-a-leader-in-urban-rail-investment-the-united-states-now-trails/

**Unprecedented, civilization-scale disaster**, entirely a policy choice. We have the technology to do better.

<style>
.slidev-layout.us {
  h2 {
    margin-top: 1.7rem;
    margin-bottom: 0.5rem;
  }
}</style>
## Theory of change
- **Internet / Social Media**: shows people what's possible, enables organizing
- **Data for decision-making**: proliferation of sensors/data and tools for analyzing/responding
- **New technology**: ebikes/micromobility, better/faster/quieter transit, app-cars / AVs help reduce <br/>car ownership

---
class: proving-it
dragPos:
  jc: 724,18,241,302
  cb: 355,18,390,282
  path: 432,276,416,257
  xbl: 46,74,435,266
  hom: 46,300,427,233
---

<style>
.slidev-layout.proving-it {
  padding-top: 1.6rem;
  h1 {
    /*position: relative;*/
    /*z-index: 200;*/
  }
  img {
    width: 100%;
    height: 100%;
  }
}
</style>

<!--
<div v-drag="'jc'"><img src="/pbls-roads.gif" class="jc" /></div>
<div v-drag="'cb'"><img src="/g2410.png" class="cb"/></div>
<div v-drag="'path'"><img src="/path-vs19.png" class="path"/></div>
<div v-drag="'xbl'"><img src="/xbl2.png" class="xbl"/></div>
<div v-drag="'hom'"><img class="hom" src="/hom.png"/></div>
-->

<div v-drag="'jc'"><a target="_blank" href="https://map.bikejc.org/?ll=40.720_-74.068&z=14"><img src="/pbls-roads.gif" class="jc" /></a></div>
<div v-drag="'cb'"><a target="_blank" href="https://ctbk.dev/stations?ll=40.717-74.045&z=15&ss=JC115&ym=2410"><img src="/g2410.png" class="cb"/></a></div>
<div v-drag="'path'"><a target="_blank" href="https://path.hudcostreets.org/#vs-2019"><img src="/path-vs19.png" class="path"/></a></div>
<div v-drag="'xbl'"><a target="_blank" href="https://github.com/hudcostreets/hudson-transit"><img src="/xbl2.png" class="xbl"/></a></div>
<div v-drag="'hom'"><a target="_blank" href="https://crashes.hudcostreets.org/#vs-homicides"><img class="hom" src="/hom.png"/></a></div>

# Proving it, locally

[hom-cmp]: https://crashes.hudcostreets.org/#vs-homicides
[xbl]: https://github.com/hudcostreets/hudson-transit
[grove-2410]: https://ctbk.dev/stations?ll=40.717-74.045&z=15&ss=JC115&ym=2410
[path]: https://path.hudcostreets.org/#vs-2019

---
layout: two-cols
layoutClass: nymtc
---

<style>
.slidev-layout.nymtc {
  padding: 2rem 2.5rem 2rem 1.5rem;
  grid-template-columns: 70% 30%;
  gap: 1rem;
  img {
    position: absolute;
    bottom: 0;
  }
  .col-left, .col-right {
    position: relative;
  }
}
</style>

# BRT / Lincoln Tunnel Bus Lane

<a href="https://github.com/hudcostreets/hudson-transit" target="_blank"><img src="/xbl.png"/></a>

::right::

<h4>
  <a href="https://www.nymtc.org/en-us/Data-and-Modeling/Transportation-Data-and-Statistics/Publications/Hub-Bound-Travel" target="_blank">
    NYMTC Hub-Bound Travel
  </a>
</h4>
<p>Annual study of modes / vehicles in/out of Manhattan CBD</p>
<a href="https://www.nymtc.org/Portals/0/Pdf/Hub%20Bound/2023%20Hub%20Bound/2023%20Hub%20Bound%20Report-%203.18.25.pdf?ver=7S_sDok5O_aw9bEN3A-NjA%3d%3d" target="_blank">
  <img src="/nymtc-hbt.png"/>
</a>

---
layout: iframe-right
url: https://ctbk.dev
scale: 0.8
---
<style>
  .slidev-page-6 .slidev-layout {
    padding: 2rem 1rem 0 2rem;
    img {
      height: 13.5rem;
      position: absolute;
      padding-left: 1rem;
      bottom: 2%;
    }
    img[src*="cb-hc"] {
      z-index: 10;
      right: 0;
      top: 0;
      height: 100%;
      /* border: 2px solid black; */
      margin: auto;
    }
  }
</style>

# [ctbk.dev]
Citi Bike dashboard

- Est. Oct '20, Updates ≈automatically each month
- Cleaned data at [`s3://ctbk`], code [on &nbsp;<logos-github-icon color="white" />][ctbk gh]
- 3.8MM rides/mo (86k/mo in JC+HOB)
- 67% ebike share, 82% annual subscribers
- Grove St (≈2 parking spots): 90-180 ride ends / day ([Feb '25][2502], [Oct '24][2410])

[![](/g2410.png)][2410]

<img v-click src="/cb-hc-opp.png" />

<!--
Show JC+HOB plateau, ebike share over time, Grove St 80/day in Feb '25
-->

[ctbk.dev]: https://ctbk.dev
[`s3://ctbk`]: https://ctbk.s3.amazonaws.com/index.html
[ctbk gh]: https://github.com/neighbor-ryan/ctbk.dev
[2410]: https://ctbk.dev/stations?ll=40.717-74.045&z=15&ss=JC115&ym=2410
[2502]: https://ctbk.dev/stations?ll=40.717-74.045&z=15&ss=JC115&ym=2502

---
layout: iframe-right
url: https://crashes.hudcostreets.org#vs-homicides
scale: 0.8
---
# [crashes.hudcostreets.org]
NJ crash data
- Fatal crashes, updated daily ([NJSP])
- All crashes, 2-3yr lag ([NJDOT])
- <logos-bluesky/> &nbsp;[@crashes.hudcostreets.org]
- <logos-slack-icon/> &nbsp;#crash-bot

<style>
p {
  margin-bottom: 0.5rem;
}
img {
  width: 30%;
  height: 49%;
  object-fit: cover;
  object-position: top left;
  position: absolute;
  bottom: 2.8%;
}
</style>

<img src="/crash-bot.png"/>

[NJSP]: https://www.nj.gov/njsp/info/fatalacc/index.shtml
[NJDOT]: https://www.nj.gov/transportation/refdata/accident/rawdata01-current.shtm
[crashes.hudcostreets.org]: https://crashes.hudcostreets.org
[@crashes.hudcostreets.org]: https://bsky.app/profile/crashes.hudcostreets.org

---
layout: iframe-right
url: https://path.hudcostreets.org#vs-2019
scale: 0.7
---
# [path.hudcostreets.org]
PATH ridership data
- Weekend ridership exceeding pre-COVID levels (despite worse service)

[path.hudcostreets.org]: https://path.hudcostreets.org

---
layout: iframe-right
url: /bh24.pdf
---
<style>.slidev-page-9 h1 { line-height: 3.3rem; }</style>

# [2024 Bike Hoboken Traffic Injury Report][bh24]
- [Bike Hoboken] OPRA'd all 2024 crash records
- Data entry from PDFs (100's of volunteer-hours)
- [NJTR-1] forms (crashes involving autos) and "incident reports" (ped and/or bike only)

**0 pedestrian injuries involving bicycles or e-bikes on a sidewalk** (despite brouhaha / "test+vest" ordinance)

[bh24]: https://www.bikehoboken.org/articles/2024-bike-hoboken-traffic-injury-report
[Bike Hoboken]: https://www.bikehoboken.org/
[NJTR-1]: https://www.nj.gov/transportation/refdata/accident/pdf/NJTR-1CrashReportManual2023.pdf

---
---

# Data projects, sources

- [ctbk.dev]: Citi Bike dashboard
- [crashes.hudcostreets.org]: NJ crash data
- [path.hudcostreets.org]: PATH ridership data
- [hudcostreets/hudson-transit]: NYMTC Hudson River crossing data

<div style="font-size:0.5em">&nbsp;</div>

| Source   | Data                   | Frequency | Delay       | HCCS Mirror                                                                                 |
|----------|------------------------|----------|-------------|---------------------------------------------------------------------------------------------|
| [NJSP]   | Crashes (fatal)        | Daily    | 1d – 3mos   | [<logos-github-icon/>][hudcostreets/nj-crashes] [<logos-aws-s3 />][`s3://nj-crashes/njsp`]  |
| [NJ DOT] | Crashes (all)          | Annually | 2-3yrs ('22) | [<logos-github-icon/>][hudcostreets/nj-crashes] [<logos-aws-s3 />][`s3://nj-crashes/njdot`] |
| [Lyft] | Citi Bike ridership    | Monthly  | ≈1wk        | [<logos-github-icon/>][hudcostreets/ctbk.dev] [<logos-aws-s3 />][`s3://ctbk`]               |
| [PANYNJ] | PATH Ridership         | Monthly  | 1-2mos      | [<logos-github-icon/>][hudcostreets/path]                                                   |
| [NYMTC]  | Hudson River crossings | Annually | 1-2yrs ('23) | [<logos-google-drive />][HCCS NYMTC]                                                        |
| NJ Transit | Rides per station/line | OPRA     | -           | [<logos-google-drive />][HCCS NJT]                                                          |
| NJ Turnpike | Exits x Veh types      | OPRA         | -           | [<logos-google-drive />][HCCS NJTA]                                                         |

[ctbk.dev]: https://ctbk.dev
[crashes.hudcostreets.org]: https://crashes.hudcostreets.org
[path.hudcostreets.org]: https://path.hudcostreets.org
[hudcostreets/hudson-transit]: https://github.com/hudcostreets/hudson-transit

[NJSP]: https://www.nj.gov/njsp/info/fatalacc/index.shtml
[NJ DOT]: https://www.nj.gov/transportation/refdata/accident/rawdata01-current.shtm
[PANYNJ]: https://www.panynj.gov/path/en/about/stats.html
[NYMTC]: https://www.nymtc.org/en-us/Data-and-Modeling/Transportation-Data-and-Statistics/Publications/Hub-Bound-Travel
[Lyft]: https://citibikenyc.com/system-data

[`s3://nj-crashes/njsp`]: https://nj-crashes.s3.amazonaws.com/index.html#/njsp/data
[`s3://nj-crashes/njdot`]: https://nj-crashes.s3.amazonaws.com/index.html#/njdot/data
[hudcostreets/path]: https://github.com/hudcostreets/path
[hudcostreets/nj-crashes]: https://github.com/hudcostreets/nj-crashes
[hudcostreets/ctbk.dev]: https://github.com/neighbor-ryan/ctbk.dev
[HCCS NYMTC]: https://drive.google.com/drive/folders/1Dm-ZBYxWaOaGgm08XCGOZCuvU2IQaPLN
[HCCS NJTA]: https://drive.google.com/drive/folders/1Ff4TUP6MmuoGvE0qTE2cgBukoxstB-93
[HCCS NJT]: https://drive.google.com/drive/folders/1IkeX8EOavWC1uUa1eHIIbVmE8i5tDuwE
[`s3://ctbk`]: https://ctbk.s3.amazonaws.com/index.html

[gbfs]: https://github.com/MobilityData/gbfs
[cb gbfs]: https://gbfs.citibikenyc.com/gbfs/2.3/gbfs.json
[cb gbfs stations]: https://gbfs.lyft.com/gbfs/2.3/bkn/en/station_information.json
[cb gbfs status]: https://gbfs.lyft.com/gbfs/2.3/bkn/en/station_status.json
