# 🐯 SIM-PHS: Sistem Informasi Monitoring Perilaku Harimau Sumatera

> **Live App** → [https://nadiya-analytics.shinyapps.io/APP_BKSDA/](https://nadiya-analytics.shinyapps.io/APP_BKSDA/)

An interactive R Shiny application for visualizing behavioral monitoring data of Sumatran tigers (*Panthera tigris sumatrae*) — built to support veterinarians and wildlife officers in analyzing individual tiger behavior patterns as part of rehabilitation and release assessment programs.

> Developed during an internship at BKSDA (Balai Konservasi Sumber Daya Alam), in collaboration with AI tools (Claude by Anthropic).

---

## Background

Behavioral monitoring is a critical component in determining whether a Sumatran tiger in rehabilitation is ready for release into the wild. This application provides an accessible, visual interface for wildlife professionals — particularly veterinarians — to explore tracking data without requiring programming knowledge.

The Sumatran tiger is classified as **Critically Endangered** by the IUCN Red List, with fewer than 400 individuals estimated to remain in the wild.

---

## Features

- 📂 **CSV Upload** — load behavioral observation data directly from field records
- 📊 **Interactive Visualization** — time-series plot of behavioral frequency built with Plotly, fully zoomable and hoverable
- 🕐 **Time-of-Day Color Coding** — observations color-coded by session: Pagi (morning), Siang (afternoon), Sore (evening), Malam (night)
- 🔽 **Behavior Selector** — switch between different behavioral categories dynamically
- 📋 **Data Table** — full tabular view of uploaded data with pagination and horizontal scroll
- 💾 **Chart Export** — download generated plots as PNG reports

---

## Tech Stack

| Library | Role |
|---|---|
| `shiny` | Web application framework |
| `ggplot2` | Static plot generation |
| `plotly` | Interactive chart rendering |
| `DT` | Interactive data table |
| `bslib` | UI theming (Minty / Bootstrap 5) |
| `dplyr` | Data wrangling |
| `bsicons` | UI icons |

---

## How to Run Locally

```r
# Install dependencies
install.packages(c("shiny", "ggplot2", "DT", "bslib", "dplyr", "plotly", "bsicons"))

# Run the app
shiny::runApp("app.R")
```

---

## Context

This application was developed as part of an internship project at a government wildlife conservation agency and submitted as a working tool for field use. It reflects a collaboration between biology domain knowledge, field conservation context, and computational implementation.

**Domain**: Wildlife conservation · Sumatran tiger · IUCN Critically Endangered  
**Version**: 1.3 Stable  
**End users**: Veterinarians, wildlife conservation officers  
**Purpose**: Support data-driven behavioral analysis for tigers in rehabilitation programs

---

## Data Notice

Observational data used in this application is the property of the relevant government conservation agency (BKSDA) and is **not included** in this repository. The codebase is shared for educational and portfolio purposes.

---

## Author

**Nadiya Linie Juniva**  
Biology Student · Universitas Negeri Padang (UNP)  
Faculty of Mathematics and Natural Sciences (FMIPA)  
Internship · BKSDA Sumatera Barat

---

*Built with curiosity, domain knowledge, and a willingness to work across disciplines — one small step toward evidence-based wildlife conservation in Indonesia.*
