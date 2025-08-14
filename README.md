# OCR transformer model

Textline recognition model, implemented using PyTorch, specialised for the recognition of multi-script and multi-language lines containing Polytonic Greek and other scripts/languages.

This custom model was trained with ~6.2M of articially generated lines, as well as 350k real-world lines. It reaches a character-level accuracy of 98.2% on lines containing mixed Latin and Greek alphabets (+8% improvement with respect to our [Tesseract baseline](https://github.com/tesseract-ocr/tessdata_contrib/tree/main/grc_hist)). 

This model is only the core of a broader wrapper which allows it to ingest lines of any length. The modules are described [`ajmc_pipeline/ocr/pytorch`](https://github.com/AjaxMultiCommentary/ajmc-pipeline/tree/main/ajmc/ocr/pytorch) and a few example usages can be found in [`ajmc_pipeline/ocr/_scripts`](https://github.com/AjaxMultiCommentary/ajmc-pipeline/tree/main/ajmc/ocr/_scripts). A more user-friendly API will be released as soon as possible.  

## Acknowledgements

Code & data in this repository were produced in the context of the Ajax Multi-Commentary project, funded by the Swiss National Science Foundation under an Ambizione grant [PZ00P1\_186033](http://p3.snf.ch/project-186033).


## Citation

This work was released as part of [this PhD thesis](https://infoscience.epfl.ch/entities/publication/0ef2d7a8-8b8c-45c1-a6c1-a1cb47295164) (See Chapter 3). To cite this work, please use: 

```
@phdthesis{item_0ef2d7a88b8c45c1a6c1a1cb47295164, 
address={Lausanne}, 
title={Document processing in data-scarce, domain-specific environments: The case of multilingual classical commentaries},
url={https://infoscience.epfl.ch/handle/20.500.14299/243183},
DOI={10.5075/epfl-thesis-11208}, 
school={EPFL}, 
author={Najem-Meyer, Sven}, year={2025}, 
keywords={Document Processing | Machine Learning | Data-scarcity | Classical Scholarship | Low-Resource Artificial Intelligence},
language={en} }
```
