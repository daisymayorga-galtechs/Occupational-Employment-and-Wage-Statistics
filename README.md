# Modesto MSA Tech & Industrial Workforce Analysis (2009–2026)
### Uncovering In-House Tech, Industrial Automation, and Career Pathways in Stanislaus County

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![Data Source](https://img.shields.io/badge/Data%20Source-California%20EDD%20%7C%20OEWS-brightgreen.svg)](https://data.ca.gov/)
[![Taxonomy](https://img.shields.io/badge/Taxonomy-Standard%20Occupational%20Classification%20(SOC)-purple.svg)](https://www.bls.gov/soc/)

---

## Overview

When looking at industry classifications (NAICS) in Stanislaus County, dedicated software and tech service companies appear to account for only **238 external vendor jobs** across 66 establishments. This creates a false impression that technology opportunities do not exist in the region.

This project shifts the analytical paradigm from **industry classification (NAICS)** to **occupational classification (SOC)** using the California Employment Development Department's **Occupational Employment and Wage Statistics (OEWS)** dataset (2009–2026). 

By tracking individual occupations across the **Modesto Metropolitan Statistical Area (Stanislaus County)**, this study reveals an embedded ecosystem of **1,800 to 2,000+ technical, software, and industrial computing professionals** working directly in-house across agriculture, food processing, logistics, healthcare, public education, and municipal utilities.

---

## Research Questions & Investigative Perspectives

This exploratory analysis examines the Central Valley labor market through three connected lenses:

1. **For Computer Science Majors & Workforce Entrants:**  
   Where do computer science graduates actually land locally? Beyond traditional remote work or out-of-region tech hubs, what in-house technical positions (data science, software engineering, systems design) drive the regional economy?
2. **For Industrial Tech & Advanced Manufacturing:**  
   How do programming and hardware merge in the Central Valley? Why do non-traditional technical roles like **CNC programmers, CNC tool operators, and SCADA/PLC automation specialists** represent such a critical slice of local technical employment?
3. **For Mid-Career Job Seekers & SMB Technology Enablement:**  
   What skills, software proficiencies, and industry-recognized certifications bridge traditional workers into stable, high-wage operational and infrastructure technology positions?

---

## Key Findings

### 1. The In-House Reality
Over **85% of tech workers in Stanislaus County are employed in-house** at non-tech organizations (such as E. & J. Gallo Winery, Foster Farms, Memorial Medical Center, Modesto City Schools, and Modesto Irrigation District) rather than external tech agencies.

### 2. Composition of the Regional Tech Workforce
* **Operations & User Support Lead Volume:** **Computer User Support Specialists (~360+ jobs)** represent the single largest tech occupation in the county, maintaining mission-critical uptime across healthcare clinics, packing sheds, and public schools.
* **Architecture Over Legacy Maintenance:** **Software Developers (~300 jobs)** outnumber traditional **Computer Programmers (~50 jobs)** by a 6:1 ratio, reflecting demand for modern cloud integration, ERP customization, and full-stack software development.
* **Management-Heavy Structure:** **Computer and Information Systems Managers (~230 jobs)** outnumber systems analysts and network administrators, as local enterprises hire in-house directors to guide strategy while outsourcing modular support.
* **Industrial Tech is Front and Center:** **CNC Tool Operators (~140 jobs)** and **CNC Tool Programmers (~20 jobs)** write G-code, configure CAD/CAM paths, and run precision fabrication for agricultural machinery (e.g., Flory Industries) and sanitary food-processing equipment.
* **Emerging Data & Security Needs:** An established baseline of **Data Scientists (~80 jobs)** supports yield forecasting, supply chain logistics, and predictive maintenance.

```text
Stanislaus County Tech Footprint:
├── External Tech Vendor Firms (NAICS 5415/5132):     ~238 jobs
└── In-House Technical Occupations (SOC 15-xxxx / 11-3021): ~1,900+ jobs
```

---

## Dataset & Classification Framework

### NAICS vs. SOC: Why the Switch Was Necessary
* **NAICS (North American Industry Classification System):** Measures the *economic activity of the employer* (e.g., Beverage Manufacturing, General Warehousing, Hospitals). It hides technical roles embedded inside traditional operations.
* **SOC (Standard Occupational Classification):** Measures the *specific job tasks of the worker*, regardless of which employer writes the paycheck.

### Data Source
* **Dataset:** California Occupational Employment and Wage Statistics (OEWS), 2009–2026
* **Published By:** California Employment Development Department (EDD) / U.S. Bureau of Labor Statistics (BLS)
* **Coverage Area:** Modesto MSA (FIPS 33700 / Stanislaus County)
* **File Format:** Multi-year time-series CSV (`OEWS 2009-2026.csv`)

---

## Target Occupations Tracked

| SOC Code | Occupational Title | Primary Local Industry Setting |
| :--- | :--- | :--- |
| **`15-1232`** | Computer User Support Specialists | Education, Healthcare, Municipal Gov, Distribution Hubs |
| **`15-1252`** | Software Developers | AgTech, Food Processing HQs, Healthcare Systems |
| **`11-3021`** | Computer and Information Systems Managers | Corporate HQ, Public Utilities (MID/TID), Education |
| **`15-1244`** | Network and Computer Systems Administrators | School Districts, County Administration, Hospitals |
| **`15-1211`** | Computer Systems Analysts | Supply Chain, Cold Storage, Packaging Logistics |
| **`51-4011`** | CNC Tool Operators | Machine Shops, Ag Equipment (Flory), Metal Fabrication |
| **`15-2051`** | Data Scientists | Agribusiness, Route Optimization, Retail Analytics |
| **`15-1241`** | Computer Network Architects | Enterprise Infrastructure, Regional MSPs (Datapath) |
| **`51-9162`** | CNC Tool Programmers | Precision Manufacturing, Sanitary Food Machinery |
| **`15-1212`** | Information Security Analysts | Health Systems, Financial Institutions, Municipal Defense |

---

## Career & Certification Pathways for the Central Valley

To transition computer science students, career switchers, and workforce programs from exploratory insight into employment, this analysis identifies three credential tracks aligned with regional demand:

### 1. Industrial Tech & Precision Tooling (CNC & CAM)
* **Core Tools:** Mastercam, SolidWorks, Autodesk Fusion 360, G-code / M-code
* **Target Certifications:**
  * National Institute for Metalworking Skills (NIMS) CNC Operator / Mill Programming
  * Mastercam Associate / Professional Certification
  * Certified SOLIDWORKS Associate (CSWA / CSWP)

### 2. Industrial Automation & SCADA Engineering
* **Core Tools:** Inductive Automation (Ignition), Rockwell Studio 5000, Python, SQL, MQTT, OPC-UA
* **Target Certifications:**
  * Inductive Automation Ignition Core & Gold Certification
  * Rockwell Automation Logix5000 Certificate
  * ISA Certified Automation Professional (CAP)

### 3. Enterprise Infrastructure, Cloud & Cybersecurity
* **Core Tools:** Cisco IOS, Microsoft Entra ID / Active Directory, Azure, Linux, VMware
* **Target Certifications:**
  * CompTIA A+ / Network+ / Security+
  * Cisco Certified Network Associate (CCNA)
  * Microsoft Certified: Azure Administrator Associate (AZ-104)

---

## Repository Structure

```text
├── modesto_msa_2009_2026.ipynb    # Primary Jupyter notebook containing data pipeline and charts
├── data/
│   └── OEWS 2009-2026.csv         # California EDD raw multi-year dataset (or download instructions)
├── assets/
│   └── tech_jobs_volume_2026.png  # Exported charts and visual distributions
└── README.md                      # Project documentation and workforce insights
```

---

## Getting Started

### Prerequisites
* Python 3.10+
* Jupyter Notebook or Google Colab
* Required libraries: `pandas`, `matplotlib`, `seaborn`

### Quickstart

1. **Clone the repository:**
   ```bash
   git clone https://github.com/daisymayorga-galtechs/Occupational-Employment-and-Wage-Statistics.git
   cd Occupational-Employment-and-Wage-Statistics
   ```

2. **Install dependencies:**
   ```bash
   pip install pandas matplotlib seaborn
   ```

3. **Run the Notebook:**
   ```bash
   jupyter notebook modesto_msa_2009_2026.ipynb
   ```

---

## References & Official Documentation

* [California Open Data Portal — OEWS Dataset (2009–2026)](https://data.ca.gov/@california-employment-development-department/oews)
* [California EDD Labor Market Information Division (LMID)](https://labormarketinfo.edd.ca.gov/)
* [U.S. Bureau of Labor Statistics — Standard Occupational Classification (SOC) System](https://www.bls.gov/soc/)
* [BLS Occupational Employment and Wage Statistics — Modesto, CA MSA](https://www.bls.gov/oes/current/oes_33700.htm)
