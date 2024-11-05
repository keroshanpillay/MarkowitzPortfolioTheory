# Mean-Variance Optimization in Python

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Python](https://img.shields.io/badge/python-3.7%2B-blue.svg)

This repository provides a comprehensive Jupyter notebook that serves as a practical tool to understand and implement **Mean-Variance Optimization** using Python. The notebook walks through the process of constructing an optimal investment portfolio based on the Modern Portfolio Theory (MPT) introduced by Harry Markowitz.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Data Preparation](#data-preparation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

---

## Introduction

Mean-Variance Optimization is a quantitative tool that allows investors to make informed decisions by considering the trade-off between expected return and risk (volatility). This repository aims to:

- Provide a step-by-step guide to implementing mean-variance optimization.
- Offer practical examples using real-world financial data.
- Visualize the efficient frontier and optimal portfolios.
- Simulate portfolio performance over time with rolling optimization.

---

## Features

- **Data Loading and Preprocessing**: Load and preprocess financial time series data.
- **Expected Returns and Covariance Matrix Calculation**: Compute mean returns and the covariance matrix from historical data.
- **Utility Functions**: Define and use different utility functions (Quadratic, Logarithmic, Exponential, Power) for optimization.
- **Portfolio Optimization**: Find the optimal asset weights that maximize the utility function.
- **Efficient Frontier Visualization**: Plot the efficient frontier and random portfolios for comparison.
- **Rolling Optimization Simulation**: Simulate portfolio performance over time with periodic rebalancing.
- **Detailed Explanations**: Each step is accompanied by explanations to enhance understanding.

---

## Getting Started

### Prerequisites

- Python 3.7 or higher
- Jupyter Notebook or JupyterLab
- Required Python libraries:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `scipy`
  - `IPython`

### Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/keroshanpillay/MarkowitzPortfolioTheory.git
   cd mean-variance-optimization
   ```

2. **Create a Virtual Environment**

  ```python
  python -m venv venv
  source venv/bin/activate  # On Windows use `venv\Scripts\activate`
  ```

3. **Install the libraries**

  ```python
  pip install numpy pandas matplotlib scipy ipython
  ```

### Data Preparation

*We have included the 8 Asset test data for you in `test-data/` of this repo.*

The notebook expects a CSV file containing daily price data for multiple assets. The data should be organized with timestamps as the index and asset symbols as columns.

1. **Data Format**
```python
timestamp,Asset1,Asset2,Asset3,...,AssetN
2024-03-01,PriceA1,PriceA2,PriceA3,...,PriceAN
2024-03-02,PriceA1,PriceA2,PriceA3,...,PriceAN
...
```

2. **Place your data file**
Place your data file (e.g., `data.csv`) in the `test-data/` directory or adjust the path in the notebook accordingly.

## Results
The notebook will produce:

- Optimized Portfolio Weights: The optimal allocation for each asset.
- Expected Portfolio Return and Volatility: Key metrics for the optimized portfolio.
- Efficient Frontier Plot: Visualization of the efficient frontier along with random portfolios and the optimized portfolio.
- Portfolio Performance Over Time: Simulation results showing how the portfolio value evolves.

  Example plot:
  ![frontier](https://ubgb8o3jr1fhytpd.public.blob.vercel-storage.com/standard-mixed-buvK1ruEV3dwHnIFrRv8fgenZGltEI.png)

## Contributing
Contributions are welcome! If you have suggestions for improvements or want to add new features:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/your-feature-name`.
3. Commit your changes: `git commit -am 'Add some feature`'.
4. Push to the branch: `git push origin feature/your-feature-name`.
5. Open a pull request.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Ackowledgements

- Harry Markowitz: 1952, 1959, 1961

  @article{markowitz1952portfolio,
  title={Portfolio selection},
  author={Markowitz, Harry M},
  journal={The Journal of Finance},
  volume={7},
  number={1},
  pages={77--91},
  year={1952},
  publisher={Wiley Online Library}
}

@article{markowitz1991nobel,
  title={Foundations of Portfolio Theory},
  author={Markowitz, Harry M},
  journal={The Journal of Finance},
  volume={46},
  number={2},
  pages={469-477},
  year={1991},
  publisher={Wiley Online Library}
}

@book{markowitz1959portfolio,
  title={Portfolio Selection: Efficient Diversification of Investments},
  author={Markowitz, Harry M},
  year={1959},
  publisher={John Wiley \& Sons},
  address={New York}
}


