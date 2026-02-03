# BLUCK: A Benchmark Dataset for Bengali Linguistic Understanding and Cultural Knowledge
## Overview

BLUCK is a comprehensive multiple-choice question (MCQ) dataset designed to evaluate Bengali language understanding and cultural knowledge. The dataset contains questions across four major categories: Culture, History, Phonetics, and Semantics, covering various aspects of Bengali language, literature, and the cultural heritage of Bengal.

## Dataset Structure

The dataset is organized into CSV files within the `bn_dataset` directory, structured as follows:

```
bn_dataset/
├── Culture/
│   ├── Art, Heritage, & Media.csv
│   ├── Constitution.csv
│   ├── Geography.csv
│   ├── Indigenous People.csv
│   ├── Law.csv
│   ├── National Issues.csv
│   └── Resources.csv
├── History/
│   ├── Ancient Bengal.csv
│   ├── British Bengal.csv
│   └── Pakistan Era.csv
├── Phonetics/
│   ├── Alphabet.csv
│   ├── Conjunct Letters.csv
│   ├── Miscellaneous Phonetics.csv
│   ├── Phonetic Combining Rules.csv
│   ├── Pronunciation.csv
│   ├── Sound & Letters.csv
│   └── Sound Changes.csv
└── Semantics/
    ├── Antonyms.csv
    ├── Idioms.csv
    ├── Miscellaneous.csv
    ├── One Word Expressions.csv
    ├── Proverbs.csv
    ├── Synonyms.csv
```

## Data Format

Each CSV file contains multiple-choice questions with the following columns:

- `question`: The question text in Bengali
- `a`: Option A
- `b`: Option B
- `c`: Option C
- `d`: Option D
- `answer`: The correct answer (a, b, c, or d)

### Example

```csv
question,a,b,c,d,answer
আয়তনে বাংলাদেশের সবচেয়ে বড় জেলা কোনটি?,রাঙ্গামাটি,বরিশাল,চট্টগ্রাম,ময়মনসিংহ,a
```

## Usage

### Loading the Dataset

```python
import pandas as pd

# Load a specific category
df = pd.read_csv('bn_dataset/Culture/Geography.csv')

# Display the data
print(df.head())
```

## Statistics

The dataset contains questions across:
- **7** Culture subcategories
- **3** History subcategories
- **7** Phonetics subcategories
- **6** Semantics subcategories

**Total: 23 different topic areas**

## Language

All questions and answers are in **Bengali (বাংলা)** script.

## Citation

If you use this dataset in your research, please cite:

```bibtex
@dataset{bluck2024,
  title={BLUCK: A Benchmark Dataset for Bengali Linguistic Understanding and Cultural Knowledge},
  author={Your Name},
  year={2024}
}
```

## Acknowledgments

This dataset aims to promote Bengali language research and preserve cultural knowledge for future generations.
