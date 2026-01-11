# Bridge Hand Distribution Analysis

## Project Overview
This Python script analyzes suit distributions in bridge hands (13 cards from a 52-card deck). It calculates the probability of having various maximum and minimum numbers of cards in any single suit within a hand, providing valuable insights for bridge players and probability enthusiasts.

## Key Results

### Maximum Cards in a Single Suit
| Max Cards | Probability | Frequency | 1 in X Hands |
|-----------|-------------|-----------|--------------|
| 5 | 44.34% | 281,562,853,572 | 2.3 |
| 4 | 35.08% | 222,766,089,260 | 2.9 |
| 6 | 16.55% | 105,080,049,360 | 6.0 |
| 7 | 3.53% | 22,394,644,272 | 28.4 |
| 8 | 0.47% | 2,963,997,036 | 214.2 |
| 9 | 0.04% | 235,237,860 | 2,699.5 |
| 10 | 0.00% | 10,455,016 | 60,737.7 |
| 11 | 0.00% | 231,192 | 2,746,693.5 |
| 12 | 0.00% | 2,028 | 313,123,057.0 |
| 13 | 0.00% | 4 | 158,753,389,900.0 |

### Minimum Cards in a Single Suit
| Min Cards | Probability | Frequency | 1 in X Hands |
|-----------|-------------|-----------|--------------|
| 2 | 53.80% | 341,657,192,448 | 1.9 |
| 1 | 30.55% | 194,023,212,812 | 3.3 |
| 3 | 10.54% | 66,905,856,160 | 9.5 |
| 0 | 5.11% | 32,427,298,180 | 19.6 |

## Mathematical Foundation

### Total Possible Hands
The total number of possible bridge hands is given by the combination formula:

\[
\text{Total Hands} = \binom{52}{13} \approx 635,013,559,600
\]

### Distribution Calculation
For each possible suit distribution (spades, hearts, diamonds, clubs), the number of ways to achieve that distribution is:

\[
\text{Combinations} = \binom{13}{s} \times \binom{13}{h} \times \binom{13}{d} \times \binom{13}{c}
\]

where \( s + h + d + c = 13 \), and each suit count ranges from 0 to 13.

## Insights for Bridge Players

1. **Most Common Maximum**: A 5-card suit is the most common maximum (44.34% probability)
2. **Balanced Hands**: 4-card maximum occurs in 35.08% of hands
3. **Long Suits**: 7+ card suits are relatively rare (4.04% combined probability)
4. **Void Suits**: A void (0 cards in a suit) occurs in about 5.11% of hands
5. **Singletons**: A singleton (1 card in a suit) occurs in 30.55% of hands

## Code Features

- **Combinatorial Enumeration**: Examines all possible suit distributions
- **Probability Calculation**: Converts frequencies to percentages and "1 in X" format
- **Data Visualization**: Generates pie charts for top distributions
- **Formatted Output**: Clean, readable tables with proper number formatting

## Installation & Usage

bash
# Clone the repository
git clone https://github.com/yourusername/bridge-distribution-analysis.git

# Navigate to the directory
cd bridge-distribution-analysis

# Install dependencies
pip install matplotlib

# Run the analysis
python min_max_bridge_cards_in_hand.py


Requirements

    Python 3.6+

    matplotlib

    Standard math library

Applications

    Bridge strategy development

    Probability education

    Game theory analysis

    Statistical modeling of card games

File Structure
text

bridge-distribution-analysis/
│
├── min_max_bridge_cards_in_hand.py  # Main script
├── README.md                        # This file
├── requirements.txt                 # Dependencies
└── images/                          # Generated charts
    ├── max_distribution.png
    └── min_distribution.png

License

MIT License - Feel free to use and modify for educational purposes.
Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
Author

Dinko Trendafilov - https://github.com/DinkoTrendafilov

Note: This analysis provides bridge players with statistical insights into hand distributions, helping inform bidding strategies and play decisions based on mathematical probabilities rather than intuition alone.
