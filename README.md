# Financial Planner Using API's and stochastic pricing models

This project creates two financial analysis tools by using a single Jupyter notebook:

Part 1: A financial planner for emergencies. People will be able to use this tool to visualize their current savings, they can then determine if they have enough reserves for an emergency fund.

Part 2: A financial planner for retirement. This tool will forecast the performance of their retirement portfolio in 30 years. To do this, the tool will make an Alpaca API call via the Alpaca SDK to get historical price data for use in Monte Carlo simulations.

## Requirements

To use the Financial Planner, you will need to have the following dependencies installed:

- python 
- pandas
- matplotlib
- numpy
- requests
- json
- dotenv
- alpaca_trade_api


## Usage

To use the Financial Planner, open the `financial_planner.ipynb` file using Jupyter Notebook. The notebook contains instructions on how to use the Financial Planner and perform Monte Carlo simulations.

## How it Works

The Financial Planner works by using Monte Carlo simulations to predict the possible outcomes of a portfolio. The program utilizes the following user information:

- The initial portfolio value
- The allocation of the portfolio between bonds and stocks
- The length of the investment horizon (in years)

Based on this information, the program generates 500 different portfolios using Monte Carlo simulations. Each portfolio is generated by randomly sampling returns from historical data on bonds and stocks. The program then calculates the portfolio value for each year in the investment horizon for each of the 500 portfolios.

The program generates a chart that illustrates the possible outcomes of the portfolio based on the Monte Carlo simulations. The chart shows the range of possible portfolio values for each year in the investment horizon, as well as the expected portfolio value.

## License

The Financial Planner is released under the [MIT License](LICENSE).
