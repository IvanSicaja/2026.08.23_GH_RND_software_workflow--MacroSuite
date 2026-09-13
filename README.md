📌 **Project Title:** **MacroSuite — Nutrition Planning Software**  
📅 **Project Timeline:** **August 2026 – Ongoing**  
🎥 YouTube Demo: **TBD**  
📦 GitHub Source Code: <https://github.com/IvanSicaja/2026.08.23_GH_RND_software_workflow--MacroSuite>  

---

📍 My Personal Profiles ⬇︎  
🎥 Video Portfolio: To be added  
📦 GitHub Profile: <https://github.com/IvanSicaja>  
👔 LinkedIn: <https://www.linkedin.com/in/ivan-si%C4%8Daja-832682222>  
🎥 YouTube: <https://www.youtube.com/@ivan_sicaja>  

---

### 💡 Core Challenge This Project Resolves:

Designing and engineering an integrated desktop nutrition-planning system that synchronizes structured Excel data, user-managed ingredients, meals, menus, nutrition calculations, persistent configuration, image data, and automatic save/backup mechanisms while preserving database structure and data consistency.

---

### 🔧 Core Skills Tree Used To Build The Project - Skills and Tech Stack:
*(Project-Specific Structured Overview)*
```text
│
├── Software Engineering
│ ├── Software / Frameworks / Libraries
│ │ ├── Python
│ │ ├── PySide6 / Qt
│ │ ├── openpyxl
│ │ ├── Python Dataclasses
│ │ ├── pathlib
│ │ ├── QSettings
│ │ └── Git / GitHub
│ │
│ └── Skills
│   ├── Desktop GUI application development
│   ├── Event-driven application architecture
│   ├── Object-oriented data modeling
│   ├── Dynamic table & form generation
│   ├── Search, filtering & sortable data presentation
│   ├── Persistent application configuration
│   ├── Keyboard-driven workflow optimization
│   └── Exception handling & user-facing diagnostics
│
├── System Integration Engineering
│ ├── Software / Frameworks / Libraries
│ │ ├── Python
│ │ ├── openpyxl
│ │ ├── Microsoft Excel (.xlsx)
│ │ └── PySide6 / Qt
│ │
│ └── Skills
│   ├── GUI-to-Excel data integration
│   ├── Multi-sheet data synchronization
│   ├── Dynamic database schema detection
│   ├── Header-driven column mapping
│   ├── Ingredient-meal-menu data dependency integration
│   ├── Persistent filesystem configuration
│   ├── Automatic database backup handling
│   ├── Temporary-file-based safe save workflow
│   └── End-to-end data flow integration
│
├── Validation & Data Integrity
│ ├── Software / Frameworks / Libraries
│ │ ├── openpyxl
│ │ └── PySide6
│ │
│ └── Skills
│   ├── Input range validation
│   ├── Database header & column detection
│   ├── Type-safe numeric conversion
│   ├── Missing-value handling
│   ├── Data relationship validation
│   ├── Controlled Excel value updates
│   ├── Preservation of existing spreadsheet formatting
│   ├── Save-error handling & backup protection
│   └── Nutrition target deviation analysis
│
├── Data Processing & Calculation
│ ├── Software / Frameworks / Libraries
│ │ ├── Python
│ │ └── openpyxl
│ │
│ └── Skills
│   ├── Structured nutrition data processing
│   ├── Per-100-gram normalization
│   ├── Ingredient quantity scaling
│   ├── Meal nutrition aggregation
│   ├── Menu nutrition aggregation
│   ├── Dynamic nutrition-column ordering
│   ├── Daily nutrition target calculation
│   └── Target-versus-actual deviation evaluation
│
└── Research & Development Engineering
  ├── Software / Frameworks / Libraries
  │ └── Integrated within sections above
  │
  └── Skills
    ├── Application workflow architecture
    ├── Iterative GUI & data-model development
    ├── Data-interface integration
    ├── Reliability-oriented file handling
    ├── User workflow optimization
    ├── Technical debugging & diagnostics
    └── End-to-end desktop system development
```


---

### 📋 Core System Capabilities - List Only:

- **Ingredient database management**
- **Meal creation from reusable ingredients**
- **Menu creation from ingredients and complete meals**
- **Automatic nutrition scaling by ingredient weight**
- **Automatic meal & menu nutrition aggregation**
- **Nutrition values per 100 g**
- **Personalized daily nutrition target calculation**
- **Target-versus-consumption deviation analysis**
- **Dynamic Excel nutrition-column detection**
- **Excel database read/write synchronization**
- **Preservation of existing spreadsheet headers & formatting**
- **Automatic database backup creation**
- **Delayed automatic saving after data changes**
- **Persistent database path & user-profile settings**
- **Ingredient, meal & menu image management**
- **Search, filtering, sorting & keyboard-assisted data entry**



---

### 🧠️ How It Works - Core System Capabilities Workflow:

The application is built as a **Python desktop system using PySide6 / Qt** with an **Excel workbook as its structured data backend**. The application connects the user interface, nutrition calculation logic, persistent settings, images, and Excel data into a single workflow.

**Database integration:**  
The user selects an **`.xlsx` nutrition database**, which is opened through `openpyxl`. MacroSuite detects nutrition columns from the workbook headers rather than relying exclusively on fixed positions. This enables the application to map fields such as **energy, fat, saturated fat, carbohydrates, sugars, fibre, protein, and salt** to the corresponding internal data model.

**Ingredient management:**  
Ingredients are represented using structured Python dataclasses containing identification data, brand and product information, package size, nutrition values, and optional image data. Nutrition values can be automatically scaled according to the selected amount in grams.

**Meal composition:**  
Meals are assembled from existing ingredients. Each ingredient retains its specified weight, while MacroSuite calculates the corresponding nutrition contribution and aggregates all values into complete meal totals.

**Menu composition:**  
Menus can combine both individual ingredients and previously defined meals. The software automatically identifies the selected item type, scales its nutritional contribution according to weight, and calculates the total nutrition profile of the complete menu.

**Daily nutrition targets:**  
A persistent personal profile stores parameters such as **gender, age, weight, height, and training status**. MacroSuite calculates estimated daily energy and macronutrient targets and compares menu or meal totals against those targets. Deviations are evaluated as percentages and visually classified to support rapid validation of the resulting nutrition plan.

**Image data integration:**  
Ingredients can contain multiple images, while meals and menus can contain thumbnail images. Images can be loaded, displayed, rotated, removed, and stored as encoded data through the application workflow.

**Persistence & reliability:**  
The selected database path and personal settings are persisted through **QSettings**. Data modifications trigger a delayed automatic-save mechanism, while manual saving is also available. A database backup is created before modification, and save operations use a temporary workbook file before replacing the active database. Save failures are surfaced through application diagnostics while the backup remains available.

---

### ⚠️ Note:

MacroSuite currently implements extensive runtime input validation, data-consistency handling, exception handling, backup protection, and save-failure diagnostics. A dedicated automated unit/integration test suite is not currently part of the published project repository, so formal test automation remains a future extension.

---

### 📸 Project Snapshots:

<p align="center">
  <strong>TBD</strong>
</p>

<p align="center">
  <strong>TBD</strong>
</p>

<p align="center">
  <strong>TBD</strong>
</p>

---

### 🎥 Video Demonstration:

<p align="center">
  <strong>TBD</strong>
</p>

---

### 📣 Hashtags Section:

**#MacroSuite #Python #PySide6 #Qt #OpenPyXL #ExcelAutomation #SystemIntegration #SoftwareEngineering #DesktopApplication #DataProcessing #DataValidation #ConfigurationManagement #BackupRecovery #DataIntegrity #GUI #NutritionPlanning #NutritionSoftware #Automation #ResearchAndDevelopment**