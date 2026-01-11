Bridge Hand Distribution Analysis
Project Overview

This Python script analyzes suit distributions in bridge hands (13 cards from a 52-card deck). It calculates the probability of having various maximum and minimum numbers of cards in any single suit within a hand, providing valuable insights for bridge players and probability enthusiasts.
Key Results
Maximum Cards in a Single Suit

The table shows the probability of having a certain maximum number of cards in any one suit:
Max Cards	Probability	Frequency	1 in X Hands
5	44.34%	281,562,853,572	2.3
4	35.08%	222,766,089,260	2.9
6	16.55%	105,080,049,360	6.0
7	3.53%	22,394,644,272	28.4
8	0.47%	2,963,997,036	214.2
9	0.04%	235,237,860	2,699.5
10	0.00%	10,455,016	60,737.7
11	0.00%	231,192	2,746,693.5
12	0.00%	2,028	313,123,057.0
13	0.00%	4	158,753,389,900.0
Minimum Cards in a Single Suit

The table shows the probability of having a certain minimum number of cards in any one suit:
Min Cards	Probability	Frequency	1 in X Hands
2	53.80%	341,657,192,448	1.9
1	30.55%	194,023,212,812	3.3
3	10.54%	66,905,856,160	9.5
0	5.11%	32,427,298,180	19.6
Mathematical Foundation
Total Possible Hands

The total number of possible bridge hands is given by the combination formula:
Total Hands=(5213)≈635,013,559,600
Total Hands=(1352​)≈635,013,559,600
Distribution Calculation

For each possible suit distribution (spades, hearts, diamonds, clubs), the number of ways to achieve that distribution is:
Combinations=(13s)×(13h)×(13d)×(13c)
Combinations=(s13​)×(h13​)×(d13​)×(c13​)

where s+h+d+c=13s+h+d+c=13, and each suit count ranges from 0 to 13.
Insights for Bridge Players

    Most Common Maximum: A 5-card suit is the most common maximum (44.34% probability)

    Balanced Hands: 4-card maximum occurs in 35.08% of hands

    Long Suits: 7+ card suits are relatively rare (4.04% combined probability)

    Void Suits: A void (0 cards in a suit) occurs in about 5.11% of hands

    Singletons: A singleton (1 card in a suit) occurs in 30.55% of hands

Code Features

    Combinatorial Enumeration: Examines all possible suit distributions

    Probability Calculation: Converts frequencies to percentages and "1 in X" format

    Data Visualization: Generates pie charts for top distributions

    Formatted Output: Clean, readable tables with proper number formatting

Usage
bash

python min_max_bridge_cards_in_hand.py

The script outputs:

    Probability tables for maximum and minimum suit lengths

    Pie charts visualizing the most common distributions

Applications

    Bridge strategy development

    Probability education

    Game theory analysis

    Statistical modeling of card games

Requirements

    Python 3.6+

    matplotlib

    Standard math library

This analysis provides bridge players with statistical insights into hand distributions, helping inform bidding strategies and play decisions based on mathematical probabilities rather than intuition alone.

