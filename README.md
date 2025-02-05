# Making Sense of Aviation Safety Data

As I pilot myself, I'm very interested in aviation safety trends. I took a look into NTSB's public accident database to understand what causes accidents and how we can prevent them. This project started as a personal exploration but grew into something I think other aviation enthusiasts and safety professionals might find useful.

## What I Found

Looking at nearly 8 decades of NTSB data revealed some interesting patterns. While commercial airlines have an impressive safety record, general aviation faces some persistent challenges. For instance, I was surprised to find that nearly 1 in 10 accidents involved fuel-related issues - something that's largely preventable.

The data shows a consistent improvement in safety across the board, but the gap between commercial and general aviation remains significant. What really caught my attention was how weather impacts different types of operations - general aviation pilots tend to avoid bad weather (only 5% of accidents in IMC), while commercial operations deal with it more frequently (15-18% of accidents in IMC).

## Datasets
I worked with two main datasets:
- The NTSB's aviation accident database
- A supplementary US state codes reference file

Here's how everything is organized:

```text
.
├── data/
│   ├── AviationData.csv
│   └── USState_Codes.csv
└── analysis/
    └── NTSB_Analysis.ipynb
```

## My Approach

I spent considerable time cleaning up inconsistencies in how flights were recorded and standardizing location data. The analysis focuses on aspects I found most crucial for understanding accident patterns:

- Long-term safety trends
- Critical phases of flight
- Weather's role in accidents
- Geographic patterns
- Differences between commercial, private, and charter operations

## Running This Yourself

If you want to explore the data, you'll need Python 3.x and some data science libraries (numpy, pandas, matplotlib, seaborn). The Jupyter notebook contains detailed comments explaining my reasoning at each step.

## Findings

After spending time with this data, a few things became clear:

Simple fuel management issues still cause too many accidents
Takeoffs and landings remain the riskiest parts of any flight
Weather decision-making is a key differentiator between commercial and private operations
