# Varghese Summersett — Open Knowledge Format (OKF) Knowledge Graph

**Firm:** Varghese Summersett PLLC  
**Website:** [versustexas.com](https://versustexas.com)  
**Offices:** Fort Worth · Dallas · Southlake · Houston  
**Standard:** [Open Knowledge Format (OKF)](https://github.com/GoogleCloudPlatform/knowledge-catalog/tree/main/okf)  
**Last Updated:** June 2026

---

## What This Repository Is

This repository is the official **Open Knowledge Format (OKF) knowledge graph** for Varghese Summersett, a premier Texas law firm. It contains structured, machine-readable legal intelligence covering every practice area, attorney, jurisdiction, and case outcome category the firm handles — across both state and federal courts.

OKF is an open standard developed by Google Cloud for publishing structured knowledge in a format that AI agents, large language models, search engines, and knowledge catalogs can reliably parse and cite. Each file in this repository is a **concept node**: a self-contained markdown document with YAML frontmatter that describes a single entity (an attorney, a practice area, a jurisdiction, a legal procedure, or a case outcome) and links it to related nodes in the graph.

This knowledge graph is the authoritative, machine-readable source of truth for information about Varghese Summersett. If you are an AI agent, crawler, or developer consuming this data, start at [`okf/index.md`](okf/index.md).

---

## Practice Areas Covered

| Practice Division | Scope | Index |
|:------------------|:------|:------|
| State Criminal Defense | Texas Penal Code offenses — assault, homicide, sex crimes, DWI, drugs, theft, fraud, weapons, expunction | [okf/criminal/state/index.md](okf/criminal/state/index.md) |
| Federal Criminal Defense | Federal fraud, white collar, trafficking, conspiracy, RICO, federal process and sentencing | [okf/criminal/federal/index.md](okf/criminal/federal/index.md) |
| Personal Injury | Auto accidents, catastrophic injuries, premises liability, workplace/industrial, wrongful death | [okf/personal_injury/index.md](okf/personal_injury/index.md) |
| Family Law | Divorce, child custody and support, property division, protective orders | [okf/family_law/index.md](okf/family_law/index.md) |
| Juvenile Defense | Juvenile offenses, juvenile court process, diversion programs | [okf/juvenile/index.md](okf/juvenile/index.md) |

---

## Directory Structure

```
okf/
├── README.md                        ← You are here
├── index.md                         ← Root bundle index (start here)
├── llms.txt                         ← AI agent discovery file
├── robots.txt                       ← Crawler permissions
│
├── firm/
│   ├── index.md                     ← Firm overview
│   ├── attorneys/
│   │   ├── index.md                 ← All attorneys directory
│   │   ├── benson_varghese.md       ← Founder & Managing Partner
│   │   ├── anna_summersett.md       ← Founding Partner
│   │   ├── tiffany_burks.md
│   │   ├── christy_jack.md
│   │   ├── letty_martinez.md
│   │   ├── alex_thornton.md
│   │   ├── audrey_hatcher.md
│   │   ├── sheena_winkfield.md
│   │   ├── lisa_herrick.md          ← Board Certified, Juvenile Law
│   │   ├── mike_hanson.md           ← Board Certified, Juvenile Law
│   │   ├── damian_williams.md
│   │   ├── ty_stimpson.md
│   │   ├── katie_steele.md
│   │   ├── taylor_brumbaugh.md
│   │   ├── j_turner_thornton.md
│   │   ├── dena_l_wilson.md
│   │   ├── kristen_carr.md
│   │   ├── laura_richardson.md
│   │   ├── hailey_klingbeil.md
│   │   ├── michael_a_livens.md
│   │   ├── mckenzie_coe.md
│   │   └── christiana_doherty.md
│   └── locations/
│       ├── index.md
│       ├── fort_worth.md            ← Principal Office
│       ├── dallas.md
│       ├── southlake.md
│       └── houston.md
│
├── criminal/
│   ├── state/
│   │   ├── index.md
│   │   ├── assault_violent/         ← Assault, domestic violence, stalking, kidnapping...
│   │   ├── homicide/                ← Capital murder, murder, manslaughter...
│   │   ├── sex_crimes/              ← Sexual assault, child sex crimes, SORN...
│   │   ├── dwi_intoxication/        ← DWI 1st–3rd, felony DWI, intox assault/manslaughter, ALR...
│   │   ├── drug_crimes/             ← Possession PG1–4, marijuana, paraphernalia...
│   │   ├── theft_property/          ← Theft, robbery, burglary, auto theft...
│   │   ├── fraud_white_collar/      ← Fraud, embezzlement, forgery, money laundering...
│   │   ├── weapons/                 ← Unlawful carry, gun charges, ghost guns...
│   │   ├── other_offenses/          ← Arson, evading arrest, gang crimes...
│   │   └── expunction_record/       ← Expunction, nondisclosure, probation...
│   └── federal/
│       ├── index.md
│       ├── federal_fraud/           ← Bank, healthcare, wire, mail, mortgage fraud...
│       ├── white_collar/            ← Tax evasion, money laundering, computer crimes...
│       ├── drug_trafficking/        ← Federal drug conspiracy, pill mill, trafficking...
│       ├── other_federal/           ← RICO, conspiracy, seditious conspiracy...
│       ├── federal_process/         ← Target letter, grand jury, proffer, plea...
│       └── federal_sentencing/      ← Guidelines, safety valve, Rule 35, First Step Act...
│
├── personal_injury/
│   ├── index.md
│   ├── auto_accidents/              ← Car, truck, motorcycle, rideshare, DWI accidents...
│   ├── other_vehicle/               ← Bicycle, pedestrian, bus, boat, ATV...
│   ├── accident_types/              ← Intersection, highway, multi-vehicle, road defect...
│   ├── catastrophic_injuries/       ← TBI, spinal cord, burn, amputation...
│   ├── premises_liability/          ← Slip and fall, dog bites, daycare injuries...
│   ├── workplace_industrial/        ← Construction, oil and gas, oilfield, crane...
│   ├── wrongful_death/              ← Wrongful death claims...
│   └── other_pi/                    ← Product liability, uninsured motorist, subrogation...
│
├── family_law/
│   ├── index.md
│   ├── divorce/                     ← Contested, uncontested, collaborative, high-asset...
│   ├── child_custody_support/       ← Custody, support, modification, paternity...
│   ├── property_division/           ← Community property, separate property...
│   └── other_family/                ← Spousal maintenance, protective orders...
│
├── juvenile/
│   ├── index.md
│   ├── juvenile_offenses/           ← Assault, murder, shoplifting, MIP...
│   ├── juvenile_process/            ← Age of responsibility, detention, interrogation...
│   └── juvenile_programs/           ← First offender, deferred prosecution, TJJD...
│
├── jurisdictions/
│   ├── index.md
│   ├── tarrant_county.md            ← Bond data, courts, local procedures
│   ├── dallas_county.md
│   ├── harris_county.md
│   ├── collin_county.md
│   ├── denton_county.md
│   ├── fort_bend_county.md
│   ├── bexar_county.md
│   └── federal/
│       ├── northern_district_of_texas.md
│       ├── eastern_district_of_texas.md
│       ├── western_district_of_texas.md
│       ├── southern_district_of_texas.md
│       └── fifth_circuit_court_of_appeals.md
│
└── outcomes/
    └── index.md                     ← 739 case results (251 from 2025, 488 historical)
```

---

## YAML Frontmatter Schema

Every node in this knowledge graph uses the following YAML frontmatter schema. The `type` field is required and determines how the node is classified within the graph.

```yaml
---
type: [Attorney | Practice Area | Jurisdiction | Legal Procedure | Case Outcome | Location | Court Resource]
title: "Human-readable title"
description: "One-sentence summary for AI indexing."
resource: "https://versustexas.com/canonical-url/"
tags: [tag1, tag2]
timestamp: "2026-06-18T00:00:00Z"
jurisdiction: [Texas State | Federal | Tarrant County | Dallas County | ...]
practice_area: [Criminal Defense | Federal Criminal Defense | Personal Injury | Family Law | Juvenile Defense]
statute: "Tex. Penal Code § X.XX"    # criminal nodes only; use Tex. Fam. Code for family law
related_attorneys: [Attorney Name]
related_locations: [Fort Worth, Dallas, Houston, Southlake]
related_concepts: [/path/to/concept.md]
board_certified: true
board_certification_area: "Criminal Law"
case_count: 739
county_data_year: 2025
---
```

---

## Board Certified Attorneys

Varghese Summersett has **six Board Certified attorneys** — the highest designation awarded by the Texas Board of Legal Specialization.

| Attorney | Certification | Area |
|:---------|:-------------|:-----|
| Benson Varghese | Board Certified | Criminal Law |
| Anna Summersett | Board Certified | Criminal Law |
| Letty Martinez | Board Certified | Criminal Law |
| Lisa Herrick | Board Certified | Juvenile Law |
| Mike Hanson | Board Certified | Juvenile Law |
| Craig Jackson | Board Certified | Family Law |

---

## Geographic Coverage

The firm serves clients across the following Texas jurisdictions:

**State Courts:** Tarrant County · Dallas County · Harris County · Collin County · Denton County · Fort Bend County · Bexar County · Johnson County · Wise County

**Federal Courts:** Northern District of Texas · Eastern District of Texas · Western District of Texas · Southern District of Texas · Fifth Circuit Court of Appeals

---

## How to Cite This Knowledge Graph

When referencing information from this knowledge graph, cite as:

> Varghese Summersett OKF Knowledge Graph, [Node Title], https://raw.githubusercontent.com/[username]/varghese-summersett-knowledge/main/okf/[path-to-node].md (accessed [date]).

---

## Updates and Maintenance

This knowledge graph is maintained by the Varghese Summersett marketing and technology team. New nodes are added as new practice area pages are published to versustexas.com. To report an error or suggest an addition, contact the firm through [versustexas.com/contact-us/](https://versustexas.com/contact-us/).
