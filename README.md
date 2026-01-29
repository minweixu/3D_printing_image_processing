
# A Novel Quantitative Framework for Printability Evaluation in Extrusion-Based Food 3D Printing

## Overview
This repository contains the data analysis code supporting the manuscript:

**“A novel quantitative framework for printability evaluation in extrusion-based food 3D printing.”**

The code implements a quantitative evaluation framework that decouples *printability* into three physically interpretable indices:
- **Extrudability Index (EI)** – characterizing material flow behavior during extrusion  
- **Surface Index (SI)** – quantifying printing accuracy and post-print structural integrity  
- **Printability Index (PI)** – integrating EI and SI to evaluate overall printing performance  

The framework is demonstrated using soybean meal–based food inks but is designed to be extendable to other extrusion-based food 3D printing systems.

---

## Related Publication
Chen, Q., Liang, Z., Jin, Z., & Xu, M. (2026).  
*A novel quantitative framework for printability evaluation in extrusion-based food 3D printing.*  
(*Manuscript under review / in press*).

---

## Author Contributions
- **Qiong Chen** – Methodology, data analysis, original draft  
- **Zhikai Liang** – Software development, computer-vision algorithms  
- **Zhao Jin** – Resources, supervision  
- **Minwei Xu** – Conceptualization, review & editing, funding acquisition  

---

## Funding
This work was supported by the **Minnesota Soybean Research & Promotion Council (MSRPC)**  
Grant No. **FAR0038336**, and the **North Dakota Agricultural Experiment Station (Hatch Project ND 2248)**.

---

## Code Origin and Adaptation
Parts of the computer-vision workflow used in this repository are **adapted and extended from** the following open-source project:

> **Food3DPrinting**  
> https://github.com/zlianglab/Food3DPrinting

Significant modifications were made to:
- Develop new quantitative indices (EI, SI, PI)
- Improve robustness, normalization, and statistical validation
- Integrate surface analysis from 3D scanning data
- Support factorial-design-based printability evaluation

---

## Repository Structure
```text
├── Fluidity.ipynb
│   └── Extrudability analysis and EI calculation based on image processing
│
├── 3D_scanning_surface_index.ipynb
│   └── Surface Index (SI) calculation using 3D scanned mesh data
│
├── data/
│   └── (Not included) Raw images and 3D scan files
│
└── README.md
````

---

## Requirements

The code was developed and tested using Python.
Typical dependencies include:

* Python ≥ 3.9
* numpy
* pandas
* matplotlib
* opencv-python
* scikit-image
* trimesh (for 3D surface analysis)

> Exact package versions may be specified in a future `requirements.txt`.

---

## Usage

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   ```
2. Install required Python packages.
3. Run the notebooks in the following order:

   * `Fluidity.ipynb` → Extrudability Index (EI)
   * `3D_scanning_surface_index.ipynb` → Surface Index (SI)
4. Combine EI and SI to calculate the Printability Index (PI) as described in the manuscript.

---

## Notes

* Raw experimental data (images and 3D scans) are **not included** due to size and data-management constraints.
* The repository focuses on **analysis methods**, not printer control or hardware operation.
* The framework is intended for **research and educational use**.

---

## Citation

If you use this code or framework in academic work, please cite:

```text
Chen, Q., Liang, Z., Jin, Z., & Xu, M. (2026).
A novel quantitative framework for printability evaluation in extrusion-based food 3D printing.
GitHub repository.
```

---

## License

**For academic and research use only.**
Commercial use is not permitted without prior permission from the authors.

---

## Contact

For questions related to the methodology or code:

* **Qiong Chen**
* **Minwei Xu**, Ph.D. (Corresponding Author)
  Department of Plant Sciences, North Dakota State University

```

---


