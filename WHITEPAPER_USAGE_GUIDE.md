# MIZ OKI 3.0™ Whitepaper Generator - Usage Guide

## Quick Start

1. **Install dependencies:**
   ```bash
   pip install python-docx
   ```

2. **Run the generator:**
   ```python
   python complete_whitepaper_generator.py
   ```

## Simple Usage Examples

### Generate Business Whitepaper (Word format)
```python
from complete_whitepaper_generator import create_whitepaper

# Generate healthcare whitepaper
files = create_whitepaper("healthcare", "word")
print(f"Generated: {files}")

# Generate media buying whitepaper
files = create_whitepaper("media_buying", "word")
print(f"Generated: {files}")

# Generate general business whitepaper
files = create_whitepaper("general_business", "word")
print(f"Generated: {files}")
```

### Generate Premium Whitepaper
```python
from complete_whitepaper_generator import create_premium_whitepaper

files = create_premium_whitepaper()
print(f"Generated premium whitepaper: {files}")
```

### Generate Technical Whitepaper
```python
from complete_whitepaper_generator import create_tech_whitepaper

files = create_tech_whitepaper()
print(f"Generated technical whitepaper: {files}")
```

## Command Line Usage

### Basic Commands
```bash
# Generate healthcare whitepaper in Word format
python complete_whitepaper_generator.py --industry healthcare --format word

# Generate media buying whitepaper in both formats
python complete_whitepaper_generator.py --industry media_buying --format both

# Generate premium whitepaper
python complete_whitepaper_generator.py --type premium

# Generate technical whitepaper
python complete_whitepaper_generator.py --type technical
```

### All Options
```bash
python complete_whitepaper_generator.py \
  --industry healthcare \
  --format word \
  --type business \
  --workspace /path/to/workspace
```

## Parameters

### Industries
- `healthcare` - Healthcare-focused whitepaper
- `media_buying` - Media buying and advertising
- `general_business` - General business applications

### Formats
- `markdown` - Markdown format (.md)
- `word` - Microsoft Word format (.docx)
- `both` - Generate both formats

### Types
- `business` - Business-focused whitepaper
- `technical` - Technical architecture whitepaper
- `premium` - Premium executive whitepaper

## Output

All generated files are saved to the `generated_whitepapers/` directory with timestamps.

Example output files:
- `MIZ_OKI_3.0_Whitepaper_healthcare_20250712_143022.docx`
- `MIZ_OKI_3.0_Premium_Whitepaper_20250712_143045.docx`
- `MIZ_OKI_3.0_Technical_Whitepaper_20250712_143102.docx`

## Features

✅ Professional Word document formatting  
✅ Industry-specific content templates  
✅ Patent information included  
✅ ROI calculations and metrics  
✅ Comparison tables  
✅ Implementation timelines  
✅ Contact information  
✅ Visual placeholders for diagrams  

## Requirements

- Python 3.7+
- python-docx library for Word document generation

## Troubleshooting

If you get import errors:
```bash
pip install python-docx
```

If Word generation fails, the script will fall back to markdown only.
