# NTSB Aviation Data Analysis

## Overview
This project analyzes National Transportation Safety Board (NTSB) aviation accident data to identify patterns and trends in aviation safety across different operational categories (General Aviation, Commercial Airlines, and Air Taxi operations).

## Key Findings
- Overall accident rates have shown a steady decline since data collection began
- Part 91 (General Aviation) operations show significantly higher accident rates compared to Part 121 (Airlines) and Part 135 (Commercial) operations
- Approximately 9.4% of accidents involve fuel-related issues
- Critical flight phases (takeoff and landing) show higher accident concentrations, particularly in General Aviation
- Weather conditions impact different operational categories differently:
  - Part 91: ~5% accidents in IMC
  - Part 135: ~15% accidents in IMC
  - Part 121: ~18% accidents in IMC

## Data Sources
- Primary dataset: NTSB Aviation Data (AviationData.csv)
- Supporting dataset: US State Codes (USState_Codes.csv)

## Project Structure
```text
.
├── data/
│   ├── AviationData.csv
│   └── USState_Codes.csv
└── analysis/
    └── NTSB_Analysis.ipynb
```

## Analysis Methodology
1. Data Cleaning and Preprocessing
   - Standardization of FAR descriptions
   - Creation of year column from event dates
   - Validation of state codes
   - Cleaning of weather condition data

2. Analysis Categories
   - Overall accident trends
   - Phase of flight analysis
   - Weather condition impact
   - Geographic distribution
   - Operational category comparison (Part 91 vs 121 vs 135)

## Requirements
- Python 3.x
- Required libraries:
  - numpy
  - pandas
  - matplotlib
  - seaborn

## Visualizations
The analysis includes a few visualizations:
- Accident trends over time
- Flight phase distribution
- Weather condition distribution
- Geographic distribution of accidents
- Comparative analysis across FAR parts

## Safety Implications
Key takeaways for aviation safety:
1. Fuel management remains a critical safety factor
2. Extra vigilance required during critical flight phases
3. Weather conditions play a significant role in accident rates
4. Commercial operations show better safety records, suggesting effective safety protocols

## Future Work
Potential areas for further analysis:
- Deeper investigation of fuel-related incidents
- Temporal analysis of weather-related accidents
- Aircraft type-specific analysis
- Regional safety trend analysis
