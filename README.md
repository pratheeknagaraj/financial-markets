# Financial Markets

![GitHub package.json version](https://img.shields.io/github/package-json/v/pratheeknagaraj/financial-markets.svg)
![repo size](https://img.shields.io/github/repo-size/pratheeknagaraj/financial-markets)
[![GitHub license](https://img.shields.io/github/license/pratheeknagaraj/financial-markets.svg)](https://github.com/pratheeknagaraj/financial-markets/blob/master/LICENSE)
![commit activity](https://img.shields.io/github/commit-activity/m/pratheeknagaraj/financial-markets?color=yellow)
![last commit](https://img.shields.io/github/last-commit/pratheeknagaraj/financial-markets?color=purple)
![keywords](https://img.shields.io/github/package-json/keywords/pratheeknagaraj/financial-markets?color=ff69b4)

![financial markets](img/financial_markets.jpg?raw=true "Financial Markets")

**Financial Markets** is a repository that contains dynamically updating daily market data for top financial instruments across global markets.

## Description

The repository contains financial market data for financial instruments globally. It collects daily data regarding the open, high, low, close and volume data on financial instruments. It auto-updates the data on a daily basis for the latest available information.

The repository contains **50+** financial instruments. The repository contains data as early as **1927** for the earliest financial instrument, while many more are listed with data starting around **2000**.

## Purpose

Aggregating and collecting financial market data can be a tedious and difficult procedure. This repositories purpose is to simplify the access to publically available data and make it available in an easy to use and dynamic manner. The accuracy of the data is cross-referenced to provide a best effort sanity check on the reported data.

## Usage

This repository contains raw data in a flat format for easy research or integration.

This repository self-updates on a daily basis. One can re-`pull` or redownload data on a daily basis in order to have the most up to date information.

## Definitions

[**Financial Instrument**](https://en.wikipedia.org/wiki/Financial_instrument) - *"Financial instruments are monetary contracts between parties. They can be created, traded, modified and settled. They can be cash (currency), evidence of an ownership interest in an entity or a contractual right to receive or deliver in the form of currency; debt (bonds, loans); equity (shares); or derivatives (options, futures, forwards)."*

## Data Format

The data in the repository is in `.csv` format. The headers for each of the files are 

- **Date** - ISO 8601 formated date (i.e. 1970-01-01)
- **Open** - Open price for the financial instrument at the start of trading time
- **High** - Highest price for the financial instrument during trading time
- **Low** - Lowest price for the financial instrument during trading time
- **Close** - Close price for the financial instrument at the stop of trading time
- **Adj Close** - Adjusted Close price for the financial instrument incorporating corporate actions (splits, dividends, rights offerings, etc.). *Note: Adjusted Close price may be identical to close depending on the financial instrument*
- **Volume** - Number of contracts or total value of the financial instrument traded during trading time. Note: volume data is not available for all financial instruments*

## Repository Structure

The repository structure is as follows:

    data
        <region>
            <asset class>
                (<instrument group> if applicable)
                    <instrument name>
                        instrument_name.csv

For instance, the *S&P 500* US stock index would be in the following path: `data/us/stock/sandp/sandp.csv`

## Financial Instruments

Major global financial instruments are available in this repository.

 - **Regions** include: `americas, asia, euro, global, oceania,  us`
 - **Asset Classes** include: `stock, commodity (agriculture, eneergy, metals), currency, treasury`

Financial instruments update daily on the days that the trading activity is available. For instance, while some financial instruments will update 5 days a week (Monday-Friday) others are updated 7 days a week.

The availability of data depends on the financial instrument and accurate reporting numbers. While some financial instruments date back into 1900s others are only available from 2000 onward.

## Issues

If there are any issues or inconsistencies with the data, please submit an [issue](https://github.com/pratheeknagaraj/financial-markets/issues) or file a [pull request](https://github.com/pratheeknagaraj/financial-markets/pulls) so that the author may investigate and accept fixes.
## Disclaimer

No guarantees are provided as to the accuracy of the data. The author has worked to ensure that the data is in a *best effort* correct and consistent with primary sources.

## Citation

If you wish to use or reference **Financial Markets** please provide the recommended citation that includes:
- **Author**: *Pratheek Nagaraj*
- **Title**: *Financial Markets*
- **GitHub**: [github.com/pratheeknagaraj/financial-markets](https://github.com/pratheeknagaraj/financial-markets)

Below is an example TeX friendly citation:

```
@misc{pnagaraj_financial-markets_2021,
  author = {Pratheek Nagaraj},
  title = {Financial Markets},
  year = {2021},
  howpublished = {\url{https://github.com/pratheeknagaraj/financial-markets}}
}
```

## License

Copyright (c) 2021 Pratheek Nagaraj. Released under MIT License. See [LICENSE][license] for details.

[license]: LICENSE

