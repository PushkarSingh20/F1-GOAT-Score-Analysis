# F1 GOAT Score Analysis 🏎️🐐

---

## Overview

**F1 GOAT Score Analysis** is a data-driven project designed to answer the age-old question:  
**“Who is the greatest Formula 1 driver of all time?”**  

Instead of relying on fan opinions or total wins alone, this project calculates a **GOAT Score** for each driver based on:

- ⚙️ **Era-Adjusted Dominance** - How dominant a driver was in their own era.  
- 🤝 **Teammate Supremacy** - How often a driver outperformed their teammate in the same car.  
- 🚗 **Car-Adjusted Performance** - How much a driver outperformed their car’s expected potential.  
- 📈 **Consistency** - Race finishes and reliability across the career.

The metrics are normalized and combined to give a single **GOAT Score**, allowing fair comparisons across eras and machinery.

---

## Dataset

The project uses the **Formula 1 World Championship dataset (1950-2020)** from Kaggle:  
[Formula 1 World Championship (1950-2020)](https://www.kaggle.com/datasets/rohanrao/formula-1-world-championship-1950-2020/data)

Required files:

- `results.csv`
- `races.csv`
- `drivers.csv`
- `constructors.csv`
- `status.csv`

---

## Methodology

1. **Era-Adjusted Dominance** - Normalize points per season relative to the champion.  
2. **Teammate Supremacy** - Compare finishing positions against teammates for each race.  
3. **Car-Adjusted Performance** - Measure performance relative to the car’s expected rank.  
4. **Consistency** - Calculate finish rate using race status.  

All metrics are scaled to 0-100 and weighted to compute the **GOAT Score**:
GOAT Score = 0.4 * EraAdjustedDominance + 0.3 * TeammateSupremacy + 0.2 * CarAdjustedPerformance + 0.1 * Consistency


---

## Technical Stack

- **Language:** Python  
- **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn  

---

## Results

- Ranked list of top F1 drivers based on GOAT Score.  
- Visualizations comparing drivers’ strengths across the four metrics.  

Example:

| Rank | Driver              | GOAT Score |
|------|-------------------|------------|
| 1    | Juan Fangio        | 92.63      |
| 2    | Lewis Hamilton     | 83.40      |
| 3    | Max Verstappen     | 80.73      |
| 4    | Alain Prost        | 73.61      |
| 5    | Michael Schumacher | 73.54      |
| 6    | Jim Clark          | 72.94      |
| 7    | Fernando Alonso    | 70.77      |
| ...  | ...                | ...        |

---

## Kaggle Notebook

Check out the full notebook on Kaggle:  
📊 [F1 GOAT Score Analysis](https://www.kaggle.com/code/pushkarsingh20/f1-goat-score-analysis)

---

## License

This project is open-source. You are free to use, modify, and share it for educational purposes. 

---

## Author

**Pushkar Singh**

## How to Run Locally

1. Clone this repository:  
```bash
git clone <your-repo-url>


