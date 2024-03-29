# PyCBCount
PyCBCount is a Python package designed to calculate various metrics from Complete Blood Count (CBC) tests. This package provides functionalities to compute key hematological parameters such as Mean Corpuscular Volume (MCV), Mean Corpuscular Hemoglobin (MCH), and Neutrophil to Lymphocyte Ratio (NLR), among others. It also includes reference ranges for a comprehensive list of CBC metrics across different age groups.

## Installation
To install pycbcount, run the following command:

```bash
pip install pycbcount
```

## Usage
Here is how you can use the pycbcount package:

```python
import pycbcount as cbc
from pycbcount import reference_range

# Calculate MCV
mcv_value = cbc.mcv(hct=0.45, rbc=5.2e6)

# Calculate MCH
mch_value = cbc.mch(hb=14, rbc=5.2e6)

# Adult reference range for MCV and MCH
reference_range["Adult"]["MCV"]
reference_range["Adult"]["MCH"]

# Adult age reference range for MCH and MCH
reference_range[18]["MCV"]
reference_range[18]["MCH"]
```

## Features
- Calculation of MCV, MCH, MCHC, NLR, ANC, and ALC.
- Reference ranges for WBC, RBC, HGB, HCT, MCV, MCH, MCHC, RDW, PLT, Neutrophils, Lymphocytes, Monocytes, Eosinophils, and Basophils.

## Formulas and References
- **MCV Formula:** [Mean Corpuscular Volume (Wikipedia)](https://en.wikipedia.org/wiki/Mean_corpuscular_volume)
- **MCH Formula:** [Mean Corpuscular Hemoglobin (Wikipedia)](https://en.wikipedia.org/wiki/Mean_corpuscular_hemoglobin)
- **MCHC Formula:** [Mean Corpuscular Hemoglobin Concentration (Wikipedia)](https://en.wikipedia.org/wiki/Mean_corpuscular_hemoglobin_concentration)
- **NLR Formula:** [Neutrophil to Lymphocyte Ration (Wikipedia)](https://en.wikipedia.org/wiki/Neutrophil_to_lymphocyte_ratio)
- **ANC Formula:** [Absolute Neutrophil Count (Wikipedia)](https://en.wikipedia.org/wiki/Absolute_neutrophil_count)
- **ALC Formula:** [Complete Blood Count (Wikipedia)](https://en.wikipedia.org/wiki/Complete_blood_count)
- **Reference Ranges:** [Complete Blood Count (Wikipedia)](https://en.wikipedia.org/wiki/Complete_blood_count)

## Contributing
Contributions to pycbcount are highly appreciated, whether they come in the form of code improvements, bug reports, or documentation updates. This project, particularly, welcomes assistance from medical professionals or hematologists for verifying the medical accuracy of the calculations and reference data.

If you're a medical expert and notice any discrepancies or potential improvements in the medical content of this package, please feel free to correct them or suggest changes. This kind of contribution is invaluable to ensure that pycbcount provides reliable and accurate information.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
