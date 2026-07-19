# Potera CMF

[中文](README.zh-CN.md)

Potera CMF is designed for modern display devices and real-world tasks. It includes 10° LMS cone fundamentals and 10° cone-fundamental-based XYZ functions. We used standard CIE methods to derive and publish the supporting data needed for straightforward integration into spectral colour-science projects.

Across mixed-use evaluations on multiple datasets, Potera CMF achieves state-of-the-art results under a range of metrics. It is particularly effective at covering the largest number of individual observers with minimal colour difference, and offers further advantages over traditional CMFs in display-matching tasks.

The Benchmark presents a new method proposed by Dynamico for comparing CMF performance. Instead of directly comparing OM- or OV-based values, it analyses the monotonic relationship between dE and individual-observer coverage, focuses on mid-range coverage, and appropriately de-emphasises the sub-JND region and the heavily compressed extreme tail.

Beyond the performance results, the detailed construction process and methods will be released with a forthcoming public technical report.

## Contents

- [`Potera_CMF/`](Potera_CMF/): final CMF tables and figures.
- [`Potera_Benchmarks/`](Potera_Benchmarks/): benchmark data and figures.

## Representative Benchmark Figures

### D65 Target: Coverage Trend Across All Display Devices

![D65 target: coverage trend across all display devices](Potera_Benchmarks/direct/d65/all_devices_auc.svg)

### D65 Target: Modern Smartphone OLED White Point

![D65 target: modern smartphone OLED white point](Potera_Benchmarks/direct/d65/smartphone_oled_ab.svg)

### KSF LCD → WOLED Colour Matching: Coverage Trends Across Illuminants

![KSF LCD to WOLED colour matching: coverage trends across illuminants](Potera_Benchmarks/pair/ksf_lcd_to_woled/all_illuminants_auc.svg)

## Data Sources and References

The following official datasets are published by the International Commission on Illumination (CIE) under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/):

- [CIE 1931 2° CMF](https://doi.org/10.25039/CIE.DS.xvudnb9b)
- [CIE 1964 10° CMF](https://doi.org/10.25039/CIE.DS.sqksu2n5)
- [CIE 2015 2° cone-fundamental-based XYZ](https://doi.org/10.25039/CIE.DS.548rw69q)
- [CIE 2015 10° cone-fundamental-based XYZ](https://doi.org/10.25039/CIE.DS.dm6qiig7)

Individual-observer data and model references:

- [Asano, Fairchild, and Blondé (2016), *Individual Colorimetric Observer Model*](https://doi.org/10.1371/journal.pone.0145671)
- [Stiles and Burch (1955)](https://doi.org/10.1080/713821039)
- [Stiles and Burch (1959)](https://doi.org/10.1080/713826267)
- The Judd–Vos 1978 CMF data were obtained from the [Colour & Vision Research Laboratory (CVRL)](http://cvrl.ioo.ucl.ac.uk/cmfs.htm).

## Software

Data processing and figure generation used [NumPy](https://numpy.org/), [SciPy](https://scipy.org/), [pandas](https://pandas.pydata.org/), [Matplotlib](https://matplotlib.org/), and [colour-science](https://www.colour-science.org/).

## Citation

Academic publications that use Potera CMF, derive numerical results from it, or compare against it as a benchmark should cite the archived dataset release recorded in [`CITATION.cff`](CITATION.cff). Please cite the specific version used in the experiment whenever possible. GitHub's “Cite this repository” function provides APA and BibTeX entries.

This citation request is an academic attribution request. It is separate from, and does not modify, the permissions and conditions of the Apache License 2.0.
