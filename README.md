# 📈 USD/IDR Exchange Rate Forecasting Using FBProphet
### 🥇 Gold Medal — World Youth Invention and Innovation Award (WYIIA 2023)
**Mathematics Category | Yogyakarta, Indonesia | October 2023**

---

## Overview
This research forecasts the **Indonesian Rupiah (IDR) exchange rate
against the US Dollar (USD)** for the next **76 days**
(September 15 – December 29, 2023) using the **FBProphet**
time-series forecasting algorithm developed by Meta.

| Metric | Result |
|--------|--------|
| Training data | 166 business days (Jan 2 – Sep 14, 2023) |
| Forecast period | 76 days (Sep 15 – Dec 29, 2023) |
| **MAPE** | **0.006506206%** |
| **Accuracy** | **99.993%** |
| MAPE category | Very Accurate (< 10%) |
| Trend direction | ↑ Upward (IDR weakening against USD) |

---

## 🥇 Award
This project was awarded the **Gold Medal** at the
**World Youth Invention and Innovation Award (WYIIA) 2023**,
organized by the Indonesian Young Scientist Association (IYSA)
in collaboration with Universitas Sarjanawiyata Tamansiswa (UST)
and Institut Pertanian Bogor (IPB).

📄 Full extended abstract: Available upon request

---

## Research Team
| Name | Institution |
|------|-------------|
| **Arditya Sulistya Ningsih Apusing** (Lead) | Tadulako University |
| Rifdah Apriliani | Tadulako University |
| Zhafirah Tri Nursagita | Tadulako University |
| Uswatun Hasanah | Tadulako University |
| Muhamad Aidil | Tadulako University |

---

## FBProphet Model
FBProphet uses an **additive decomposition model**:

```
y(t) = g(t) + s(t) + h(t) + ε(t)
```

| Component | Description |
|-----------|-------------|
| `g(t)` | Trend — non-periodic changes over time |
| `s(t)` | Seasonality — weekly/annual periodic patterns |
| `h(t)` | Holiday effects — irregular schedule events |
| `ε(t)` | Error term — unusual changes not captured by model |

---

## Key Findings
- IDR/USD shows a **downward trend** Jan–Sep 2023 (rupiah strengthening),
  then **reverses upward** in the 76-day forecast period
- **Wednesday** consistently shows the highest IDR weakening (weekly component)
- Forecast predicts continued **IDR weakening** through December 2023
- Model achieves **99.993% accuracy** — MAPE categorized as "Very Accurate" (< 10%)

---

## Repository Structure
```
usd-idr-forecasting-fbprophet/
├── WYIIA_USD_IDR_Forecasting_FBProphet.ipynb   ← main analysis notebook
├── data/
│   └── Data_Kami_WYIIA.xlsx                    ← USD/IDR dataset (Bank Indonesia)
├── paper/
│   └── WYIIA2023_Extended_Abstract.pdf         ← published extended abstract
└── README.md
```

---

## How to Run

```bash
# 1. Install dependencies
pip install prophet pandas matplotlib openpyxl jupyter

# 2. Clone repository
git clone https://github.com/ardityaapusing/usd-idr-forecasting-fbprophet.git
cd usd-idr-forecasting-fbprophet

# 3. Open notebook
jupyter notebook WYIIA_USD_IDR_Forecasting_FBProphet.ipynb
```

---

## Data Source
**Bank Indonesia Official Website — bi.go.id**
- Variable: Daily USD/IDR middle exchange rate (Kurs Tengah Bank Indonesia)
- Period: January 2, 2023 – September 14, 2023
- Total: 166 business days
- Data is publicly available at: https://www.bi.go.id/id/statistik/informasi-kurs/transaksi-bi/default.aspx

---

## Descriptive Statistics (Training Data)

| Statistic | Value |
|-----------|-------|
| Mean | 15,102.6205 IDR/USD |
| Variance | 49,378.8 |
| Maximum | 15,635 IDR/USD (Jan 6, 2023) |
| Minimum | 14,632 IDR/USD (May 4, 2023) |
| Standard Deviation | 222.213344 |

---

## Tools & Stack
`Python 3.11` · `Prophet (FBProphet)` · `Pandas` · `Matplotlib` · `Jupyter Notebook` · `openpyxl`

---

## Acknowledgments
- **Indonesian Young Scientist Association (IYSA)** — competition organizer
- **Bank Indonesia** — data source
- **Prof. Junaidi, M.Si., Ph.D.** — research supervisor
- **Ade Hendrawan Krisdianto, S.Stat.** — methodology guidance

---

## Citation
```
Apusing, A.S.N., Apriliani, R., Nursagita, Z.T., Hasanah, U., & Aidil, M. (2023).
Forecasting The Dynamics Of The Indonesian Rupiah (IDR) Exchange Rate Against
The Dollar (USD) Using FBProphet Algorithm Analysis.
Extended Abstract, World Youth Invention and Innovation Award (WYIIA) 2023.
Gold Medal, Mathematics Category. Yogyakarta, Indonesia.
```

---

*Faculty of Natural Science and Mathematics, Tadulako University, Palu, Indonesia*
*Contact: ardityasulistya6@gmail.com | linkedin.com/in/ardityaapusing*
