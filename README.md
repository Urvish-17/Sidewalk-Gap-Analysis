# Sidewalk-Gap-Analysis

# Sidewalk-Gap-Analysis

---

## 🛠 Tools & Technologies

- **QGIS** – GIS Software used for digitization and analysis  
- **Field Calculator** – To create logic for flagging missing segments  
- **Topology Checker** – QA/QC validation  
- **Spatial SQL** – For querying sidewalk conditions and joins  
- **CSV / GeoJSON** – Formats for input/output data  

---

## 📍 Step-by-Step Workflow

### 🔹 Step 1: Sidewalk Digitization
- Open Google Satellite in QGIS.
- Manually digitize sidewalk segments.
- Add an attribute column `SW` (`y` for sidewalk, `n` for missing).

### 🔹 Step 2: Attribute Cleanup
- Standardize attribute names and formats.
- Use the Field Calculator to ensure consistent values in the `SW` field.

### 🔹 Step 3: Topology QA/QC
- Enable Topology Checker in QGIS.
- Apply rules like "Must Not Overlap", "Must Not Have Gaps", etc.
- Fix errors flagged in the output.

### 🔹 Step 4: Sidewalk Gap Identification
- Use Spatial SQL or Field Calculator to filter segments with `SW = 'n'`.
- Flag these segments for planners to review.

### 🔹 Step 5: Visualization
- Create final map layouts:
  - Full sidewalk network
  - Highlighted missing segments
- Export maps as `.png` for reporting.

### 🔹 Step 6: Documentation
- Include project metadata, data sources, and QA notes.
- Write summary statistics (e.g., "450+ sidewalk gaps flagged").

---

## 📊 Results

- ✅ 100% of West Seneca and Orchard Park sidewalk segments digitized  
- 🧩 450+ sidewalk gaps identified and flagged  
- 📈 Ready-to-use maps exported for urban planning departments  
- 🛠 Spatial data validated through QA/QC topology rules  

---

## 🔐 Data Note

Some files are mock/demo versions due to data privacy agreements. The project structure and logic remain consistent with the original internship deliverables.

---

## 🧑‍💻 Author

**Urvish Raval**  
GIS Intern @ GoBike Buffalo  
[LinkedIn](https://www.linkedin.com/in/urvish-raval-7296101a0) • [Email](mail to:rawalurvish9876@gmail.com)

---

## 📄 License

This project is open-source for learning and portfolio purposes. Please attribute credit when using.


