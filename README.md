# Pydantic Educational Project

A hands-on tutorial demonstrating Pydantic's data validation capabilities through a practical order processing system.

## What You'll Learn

- **Data Validation**: Automatic type checking and constraint validation
- **Field Validators**: Custom validation logic with `@field_validator`
- **Model Validators**: Cross-field validation with `@model_validator`
- **Computed Fields**: Dynamic properties with `@computed_field`
- **Serialization**: Converting models to/from JSON and dictionaries

## Project Overview

This notebook implements a simple order processing system with three models:
- **Item**: Product with validated price and quantity
- **Customer**: User with email validation
- **Order**: Complete transaction with automatic total verification

## Installation

```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
source venv/bin/activate  # macOS/Linux
# or
venv\Scripts\activate     # Windows

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook
```

## Usage

Open `main.ipynb` and run the cells sequentially to explore:
1. Basic validation with `Field` and `PositiveInt`
2. Email validation with `EmailStr`
3. Custom validators for price rounding
4. Cross-field validation for order totals
5. Model serialization and deserialization

## Requirements

- Python 3.11+
- Pydantic 2.0+
- Jupyter Notebook
