# Aviation Safety Analysis

This project analyzes aviation accident data from 1983–2023 to identify aircraft makes and models associated with lower rates of total destruction and serious or fatal injuries during accidents. The analysis focuses on professional aircraft still likely to be in operation and uses a minimum sample size to ensure statistical validity.

## Key Findings

- **Airbus, Embraer, and Douglas** models show the lowest serious/fatal injury rates among large aircraft types.
- Among small aircraft, **Maule, Helio, and Grumman-Schweizer** types demonstrate consistent survivability and low destruction rates.
- Accidents occurring under **Instrument Meteorological Conditions (IMC)** show significantly higher injury and destruction rates compared to Visual Meteorological Conditions (VMC).
- The **cruise and maneuvering phases** of flight are associated with the most severe accidents, while **taxiing and standing** phases have the least.
- Elevated risk was observed during **go-around and approach** scenarios, potentially due to cognitive commitment to landing ("get-there-itis").

## Dataset

Cleaned dataset saved as:  
`cleaned_aviation_data.csv`

Analysis performed in two notebooks:  
- `Aviation_Accidents_Cleaning.ipynb`  
- `Aviation_Accidents_Data_Analysis.ipynb` 
## Final Dataset Summary

- **Total rows**: 72,465  
- **Total columns**: 28  
- **Target variables**: `destroyed`, `serious_or_fatal_injury_rate`  
- **Identifier used for aircraft type**: `make_model`  
- **Dropped columns**: `airportcode`, `airportname` (due to excessive missing data)

### Columns with Missing Values:
The following columns still contain missing values but were retained for their analytical value:

- `location`: 38 missing
- `country`: 195 missing
- `injuryseverity`: 485 missing
- `registrationnumber`: 822 missing
- `make`: 11 missing
- `amateurbuilt`: 35 missing
- `numberofengines`: 4,363 missing
- `enginetype`: 5,284 missing
- `purposeofflight`: 3,667 missing
- `weathercondition`: 3,119 missing
- `broadphaseofflight`: 24,839 missing
- `reportstatus`: 5,300 missing
- `publicationdate`: 13,043 missing
- `serious_or_fatal_injury_rate`: 541 missing

These NaNs are acceptable based on context and the nature of real-world aviation reporting.



