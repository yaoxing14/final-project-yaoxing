# Data Documentation

## Dataset Dimensions
- Rows:5000
- Columns: 10


## Codebook
- `animal_type`: pet type (Cat or Dog)  
- `breed`: the pet’s breed  
- `sex_upon_intake`: sex & neuter status at intake  
- `sex_upon_outcome`: sex & neuter status at outcome  
- `age_upon_intake`: age when it entered the shelter  
- `age_upon_outcome`: age when it left the shelter  
- `intake_type`: how it entered (Stray, Owner Surrender, etc.)  
- `intake_condition`: condition at intake (Normal, Injured, etc.)  
- `outcome_type`: final outcome (Adopted, Transferred, etc.)  
- `time_in_shelter_days`: days spent in shelter

## Data Structure Preview

```r
library(tidyverse)
aac_small <- read_csv("data/aac_small.csv")
glimpse(aac_small)
```

```
Rows: 5,000

Columns: 10

$ animal_type          <chr> "Dog", "Cat", "Dog", "Dog", "Dog", "Dog", "Cat", "Dog", "Cat", "Dog"…
$ breed                <chr> "Pit Bull Mix", "Domestic Medium Hair Mix", "Great Pyrenees Mix", "B…
$ sex_upon_intake      <chr> "Intact Male", "Unknown", "Neutered Male", "Spayed Female", "Intact …
$ sex_upon_outcome     <chr> "Intact Male", "Unknown", "Neutered Male", "Spayed Female", "Spayed …
$ age_upon_intake      <chr> "2 years", "1 week", "1 year", "4 years", "1 month", "1 week", "3 mo…
$ age_upon_outcome     <chr> "2 years", "1 week", "1 year", "4 years", "1 month", "1 month", "4 m…
$ intake_type          <chr> "Owner Surrender", "Stray", "Stray", "Public Assist", "Stray", "Stra…
$ intake_condition     <chr> "Normal", "Nursing", "Normal", "Normal", "Normal", "Normal", "Normal…
$ outcome_type         <chr> "Euthanasia", "Transfer", "Return to Owner", "Return to Owner", "Ado…
$ time_in_shelter_days <dbl> 1.76111111, 0.02986111, 0.27708333, 2.21875000, 5.17708333, 48.07083…
```

