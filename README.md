<p align="center">
  <img src="https://datadrivenconstruction.io/wp-content/uploads/2023/07/DataDrivenConstruction-1-1.png" alt="DDC Logo" width="200"/>
</p>

# 🧰 CAD/BIM Community Converters

Offline `.exe` tools to convert Revit®, IFC, DWG and DGN files into structured data (Excel, PDF, DAE, etc).  
**No Autodesk® software, no cloud APIs, no plugins, no installation needed.**

---

## 🔧 What's Included

|     Converter     | Description | Supported Formats | Executable |
|-------------------|-------------|-------------------|------------|
| `RvtExporter.exe` | Converts `.rvt` Revit® models to Excel + optional PDF sheets, schedules, and geometry | Revit® 2017–2024 | ✅ |
| `IfcExporter.exe` | Converts `.ifc` (Industry Foundation Classes) models to Excel + DAE geometry | IFC2x3, IFC4 | ✅ |
| `DwgExporter.exe` | Converts `.dwg` CAD files (2D/3D) to Excel tables | DWG 2007–2024 | ✅ |
| `DgnExporter.exe` | Converts `.dgn` MicroStation® files to Excel tables (beta) | DGN V7, V8 | ✅ |

All converters are **portable**, **standalone** `.exe` files (Windows only).

---

## 📥 How to Use

1. 📁 Download the `.exe` file(s) from this repository.

### 2.1 🧠 Command Line Mode (CLI)

Use the `.exe` directly in your terminal or batch scripts:

```bash
RvtExporter.exe your_project.rvt standard sheets2pdf schedule bbox
```

> You can batch-process multiple files using `.bat` scripts or include the converter in other automated tools.
> 

### 2.2 🖱️ Simple UI (Executable File)

Each `.exe` also supports **click-based interaction**.  
Just double-click the converter to launch a basic user interface:

- 📂 Select your file
- ⚙️ Choose conversion mode (e.g. `basic`, `standard`, `complete`)
- ✅ Click to run — no command line required

> Works on Windows. No installation or Revit®/AutoCAD® needed.

---

### 2.3 🔄 Integration with n8n (Web UI + Automation)

Use a graphical web interface powered by [n8n.io](https://n8n.io) to:

- Upload files via browser
- Select export options from a form
- Automate folder creation, result reading, and validation
- Generate **AI-based Python code** for data analysis

📂 Ready-to-use workflow:  
➡️ [n8n BIM Conversion Pipeline](https://github.com/datadrivenconstruction/Revit-IFC-DWG-Converter-in-n8n)




---

## ✅ Output Files

Each converter produces:

- 🧾 `*.xlsx` — Full metadata export in matrix form  
  *(rows = elements, columns = all properties)*
- 🧱 `*.dae` — Polygonal geometry in open Collada format  
  *(Revit & IFC only)*
- 📄 `*.pdf` — Exported sheets *(Revit only, if enabled)*
- 📋 `*.xlsx` — Schedules *(Revit only, if selected)*

---

## 💬 Use Cases

- 📊 Offline CAD-BIM data analysis
- 🛠️ Custom automations (Python, n8n, Excel macros)
- 📦 Bulk conversion without Revit®, AutoCAD®, or BIM viewers
- 💼 Regulatory validation & reporting

---

## ⚖️ License

These converters are provided as **community tools** for offline data workflows.  
Commercial redistribution is **not** allowed without permission from [DataDrivenConstruction.io](https://datadrivenconstruction.io).

---

## 📫 Questions?

Contact 👉 [https://datadrivenconstruction.io](https://datadrivenconstruction.io)  
Or use them with the full pipeline:  
➡️ [n8n-bim-conversion-pipeline](https://github.com/datadrivenconstruction/CAD-BIM-to-Code-Automation-Pipeline-DDC-Workflow-with-LLM-ChatGPT)

<p align="center">
  <a href="https://datadrivenconstruction.io"> 
  <img src="https://datadrivenconstruction.io/wp-content/uploads/2023/07/DataDrivenConstruction-1-1.png" alt="DDC Logo" width="200"/>
  </a>
</p>
