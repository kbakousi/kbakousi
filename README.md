### Aikaterini (Katerina) Bakousi

Agrifood and sustainability analyst working with soil carbon, Earth observation and agricultural data. <!-- EDIT: one line in your own words, e.g. current role / location in the Netherlands -->

My repositories are organised by **theme**. Each one is a tested, documented Python package, and each method is implemented from the publications cited in its documentation.

---

#### 🌾 Agriculture & Soil

| Repository | What it does |
|---|---|
| [**parcel-crop-monitor**](https://github.com/kbakousi/parcel-crop-monitor) | Parcel-level crop and land-use checks with Sentinel-2 time series. It derives rule-based land-use states and harvest/mowing events, checks each parcel's declared crop with a Random Forest that never trained on that parcel (spatial-block cross-validation), and gives a green/amber/red verdict per parcel. The demo uses Dutch BRP parcels. *Apache-2.0* |
| [**soilcarbon-toolkit**](https://github.com/kbakousi/soilcarbon-toolkit) | Soil organic carbon workflow: stratified field-sampling design, IDW and ordinary kriging, RothC / FAO GSOCseq scenario analysis (additional sequestration vs business as usual, area-weighted), and model–measurement agreement. *Apache-2.0* |
| [**leaf-spectra-disease**](https://github.com/kbakousi/leaf-spectra-disease) | Leaf-level hyperspectral analysis for plant disease detection (worked example: grapevine leaves with esca- and powdery-mildew-like symptoms). It reads Specim IQ / ENVI data, preprocesses spectra, and screens leaves with classifiers and a one-class model trained on healthy leaves. Validation holds out whole leaves and dates, and the package measures how much pixel-level splits and date confounding overstate accuracy. *Apache-2.0* |

#### 🌍 Climate & Earth observation

| Repository | What it does |
|---|---|
| [**eo-landscape-indicators**](https://github.com/kbakousi/eo-landscape-indicators) | Indicators from open satellite and climate data: spectral indices with cloud masking (Sentinel-2, Landsat, MODIS), seasonal climate anomalies (SPEI, ERA5-Land, GRACE), per-pixel trend tests (Theil–Sen, Mann–Kendall, FDR), burned-area frequency (MODIS MCD64A1), and land-cover diversity and fragmentation. *Apache-2.0* |

#### 🧭 In progress

- **Carbon-farming economics:** carbon credits, deductions, NPV and break-even prices on top of `soilcarbon-toolkit` (private, in development).
- **Atmosphere:** air quality from open sensor and reanalysis data.
- **Urban environment:** urban heat island analysis.
- **Rural environment:** survey analysis for agricultural and rural stakeholders.

---

#### How these repositories are built

- installable packages (`pyproject.toml`, `src/` layout) with tests that run offline on synthetic data;
- continuous integration on Linux and Windows for Python 3.10–3.12;
- `CITATION.cff`, a changelog, semantic versioning, and the method references in every module;
- explicit parameters instead of hidden thresholds, and no restricted data in any repository.

#### Contact

📫 [kbakousi3@gmail.com](mailto:kbakousi3@gmail.com)

<!-- EDIT: add LinkedIn / ORCID links you are happy to make public -->
