# Skinguide Dataset

A comprehensive consumer skincare survey dataset containing 19,128 responses collected between 2020-2024, featuring demographics, skin concerns, product preferences, and self-assessment data.

**Quick Stats:** 19K+ responses | 30 variables | 0.7% missing data | CC BY 4.0 licensed

## Table of Contents
- [Overview](#overview)
- [Data Collection](#data-collection)
- [Basic Statistics](#basic-statistics)
- [Use Cases](#use-cases)
- [Dataset Schema](#dataset-schema)
- [Getting Started](#getting-started)
- [Citation](#citation)
- [License](#license)
- [Contributing](#contributing)
- [Contact](#contact)

## Overview

Skinguide is a survey of 19,128 respondents on self-assessment of skin concerns, skincare habits and demographics. It was collected as part of our efforts to understand consumers in skincare and provides rich insights into consumer behavior, product preferences, and skin health perceptions.

## Data Collection

The data was collected between 2020 and 2024 through a mobile application. Users/consumers would fill out the survey in exchange for personalized recommendations of 3rd party skincare products via a matching algorithm.

**Important Note:** Since the data has been anonymized, the same individual may occur multiple times in the dataset. Each data entry is treated as a unique "persona" even if it relates to the same individual.

## Basic Statistics

### 👥 Demographics

#### Age Distribution
- **Age responses:** 19,126
- **Age range:** 14 - 98
- **Mean age:** 35.0
- **Median age:** 32.0

**Age groups:**
- 18-25: 7,080 (37.0%)
- 26-35: 3,940 (20.6%)
- 36-45: 3,135 (16.4%)
- 46-55: 2,112 (11.0%)
- 55+: 2,859 (14.9%)

#### Gender Distribution
- Female: 18,903 (98.8%)
- Male: 119 (0.6%)
- Non binary: 106 (0.6%)

#### Ethnicity Distribution
- White / Caucasian: 10,430 (54.5%)
- Hispanic: 3,165 (16.5%)
- Black or African American: 2,398 (12.5%)
- Asian: 1,290 (6.7%)
- Other: 468 (2.4%)
- Multi-Ethnic: 447 (2.3%)
- South Asian: 399 (2.1%)
- American Indian: 336 (1.8%)
- Middle Eastern: 195 (1.0%)

### 🧴 Skin Type Analysis
- Combination: 7,557 (39.5%)
- Oily: 3,847 (20.1%)
- Dry: 3,673 (19.2%)
- Normal: 1,458 (7.6%)
- It changes: 1,441 (7.5%)
- Not sure: 1,152 (6.0%)

## Use Cases

There are multiple different use cases for this dataset. We specifically used it for:

### 🎭 Persona Development

The data is rich in that respondents identify what they are looking for and how they self-identify with specific skin concerns. This allows us to build up profiles of consumer perceptions about product needs relative to perceived skin needs.

### 💰 Price Estimation

As the data was part of a funnel for recommendation of 3rd party skincare products, we could test self-assessment of price sensitivity relative to the price of the recommended products.

### 🎯 Personalized Recommendation

We used the self-assessment of skin concerns to build a 6-parameter profile of the respondents' skin needs and queried a database of 3rd party products to find the best matching products from an ingredient perspective. This was done by translating product ingredient lists into skin benefit profiles using proprietary data and mapping algorithms.

## Dataset Schema

**Dataset Shape:** 19,128 rows × 30 columns

**Overall Missing Data Rate:** 0.7%

---

### 📊 Demographics

#### What is your age?
**Missing:** 2 (0.0%) - Numerical values

#### What is your gender?
**Missing:** 0 (0.0%) - female, male, non binary

#### What is your ethnicity?
**Missing:** 0 (0.0%) - 9 unique selections

### 🌅 Skincare Behaviors

#### When do you typically apply your skincare products?
**Missing:** 0 (0.0%) - day, night, both

#### In the sun I...
**Missing:** 0 (0.0%) - Fitzpatrick ranking (self-identified)

#### Do you have a monthly menstrual cycle?
**Missing:** 119 (0.6%) - yes, no

### 🧴 Product Preferences

#### What benefits are most important to you?
**Missing:** 0 (0.0%) - Selection of multiple choice

#### What products are in your skincare regimen?
**Missing:** 0 (0.0%) - Selection of multiple choice

#### What type of products are you looking for?
**Missing:** 0 (0.0%) - Selection of multiple choice

#### How would you classify most of your skincare products?
**Missing:** 0 (0.0%) - Ranking from low to high

#### Do you have ingredient restrictions?
**Missing:** 0 (0.0%) - Selection of multiple choice

### 🔍 Skin Assessment

#### I would describe my skin type as...
**Missing:** 0 (0.0%) - Selection of one out of multiple

#### My skin is regularly affected by...
**Missing:** 0 (0.0%) - Selection of multiple choice

#### I have sensitive skin
**Missing:** 0 (0.0%) - yes, no

### 📋 Numeric Scaled Questions

*These questions all use a slider from -2 to 2 from strongly disagree (-2) to strongly agree (+2)*

#### My skin is wrinkling or sagging.
**Missing:** 133 (0.7%)

#### I rarely breakout or have skin reactions.
**Missing:** 139 (0.7%)

#### I frequently get sun spots, dark spots, or scarring.
**Missing:** 170 (0.9%)

#### Without makeup I can easily see my pores.
**Missing:** 175 (0.9%)

#### When I wake up my skin feels oily.
**Missing:** 181 (0.9%)

#### My skin often looks dull or lacks glow.
**Missing:** 185 (1.0%)

#### I frequently have dark under-eye circles.
**Missing:** 207 (1.1%)

#### I have unexplained breakouts or redness.
**Missing:** 218 (1.1%)

#### My skin tone is even and consistent.
**Missing:** 283 (1.5%)

#### My skin typically looks radiant and healthy.
**Missing:** 308 (1.6%)

#### When I wake up my skin feels hydrated and supple.
**Missing:** 318 (1.7%)

#### My skin rarely looks shiny.
**Missing:** 319 (1.7%)

#### My skin feels smooth to the touch.
**Missing:** 332 (1.7%)

#### When I wake up my skin feels tight, irritated or dry.
**Missing:** 349 (1.8%)

#### My skin feels firm, dense.
**Missing:** 513 (2.7%)

### 🔧 Technical Columns

#### response_id
**Type:** Unique identifier
**Missing:** 0 | **Unique Values:** 19,128

## Getting Started

### Download the Data
```bash
git clone https://github.com/alida-labs/skinguide
cd skinguide
```

### File Structure
```
skinguide/
├── README.md                 # This file
├── data/
│   ├── skinguide_survey.csv  # Main dataset
├── LICENSE                   # CC BY 4.0 license
```

## Citation

If you use this dataset in your research or projects, please cite:

```bibtex
@dataset{skinguide2025,
  title={Skinguide: Consumer Skincare Survey Dataset},
  author={Alida Labs},
  year={2025},
  publisher={GitHub},
  url={https://github.com/alida-labs/skinguide}
}
```

**APA Style:**
AlidaLabs. (2025). Skinguide: Consumer Skincare Survey Dataset. GitHub. https://github.com/alida-labs/skinguide

## License

This dataset is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE). You are free to:

- **Share** — copy and redistribute the material in any medium or format
- **Adapt** — remix, transform, and build upon the material for any purpose, even commercially

Under the following terms:
- **Attribution** — You must give appropriate credit, provide a link to the license, and indicate if changes were made

## Contributing

Found an issue with the data or documentation? Have suggestions for improvement? We welcome contributions!

- 📖 **Documentation:** Help improve the README or add examples
- 📊 **Analysis:** Share interesting findings or visualizations

## Contact

Questions about the dataset?

- 🐛 **Issues:** Use GitHub Issues for dataset-related questions
- 💬 **Discussions:** Join the conversation in GitHub Discussions

