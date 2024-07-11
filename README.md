# Vietnamese Non-Standard Words Dictionary

This repository contains a JSON file for a dictionary of non-standard words and their normalized forms. This dictionary is designed to assist in the normalization of vocabulary for various Natural Language Processing (NLP) tasks. The dictionary includes mappings from non-standard or colloquial expressions to their standard equivalents.

## Dictionary Source

The dictionary is extracted from the ViLexNorm dataset. You can find more details about the dataset [here](https://github.com/ngxtnhi/ViLexNorm.git).

## Dictionary Format

The dictionary is provided in a JSON file with the following structure:

```json
{
    "non-standard word 1": ["normalized form 1"],
    "non-standard word 2": ["normalized form 2"],
    ...
}
```

Each key in the JSON object is a non-standard word or phrase, and the corresponding value is a list of one or more normalized forms. Here is a sample of the dictionary:

```json
{
    "thuong tat": ["thương tật"],
    "thực hịn": ["thực hiện"],
    "#": ["khác"],
    "+": ["cộng"],
    "bang": ["băng", "bằng"],
    "bao ? ke": ["bảo kê"],
    "15p": ["15 phút"],
    ...
}
```
## Dictionary Statistics

- **Total number of NSWs**: 3506
- **NSWs with 1 normalized term (1-1 mapping)**: 3320
- **NSWs with 2 normalized terms (1-2 mapping)**: 150
- **NSWs with 3 normalized terms (1-3 mapping)**: 23
- **NSWs with more than 3 normalized terms**: 13

## Dictionary Extraction Process

The dictionary was extracted using the following process:
1. **Data Collection**: Gathered non-standard and colloquial expressions from the ViLexNorm dataset.
2. **Normalization**: Identified the standard equivalents for each non-standard expression.
3. **Mapping**: Created mappings from each non-standard word or phrase to its normalized form(s).
4. **Validation**: Ensured the accuracy and completeness of the mappings through manual review and validation.

## Usage

This dictionary can be used in various NLP tasks, such as:

1. **Text Normalization**: Standardizing text input to improve the performance of downstream NLP models.
2. **Preprocessing**: Cleaning and preprocessing text data to ensure consistency and accuracy in text analysis.
3. **Language Modeling**: Enhancing the quality of language models by providing normalized inputs.

## Installation

To use this dictionary in your project, simply download the `vi-nsw-dict.json` file and load it using your preferred JSON parser. For example, in Python, you can use the `json` module:

```python
import json

with open('vi-nsw-dict.json', 'r', encoding='utf-8') as f:
    dictionary = json.load(f)

print(dictionary)
```

## Contribution

Contributions to this dictionary are welcome. If you have suggestions for additional non-standard words or corrections to existing entries, please submit a pull request or open an issue.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Contact

For any questions or suggestions, please contact 20520134@gm.uit.edu.vn or 20520165@gm.uit.edu.vn.
