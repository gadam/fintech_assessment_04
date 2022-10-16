# Credit Union Personal and Retirement Financial Planning Tools
## Prototype
### Personal Finance
This tool is a personal finance planner that will allow users to visualize their savings composed by investments in shares and cryptocurrencies to assess if they have enough money as an emergency fund.
### Retirement Planning
Also included is a retirement planning tool that will fetch historical closing prices for a retirement portfolio composed of stocks and bonds, then run simulations to project the portfolio performance at 30 years. It will then calculate the expected portfolio returns given a specific initial investment amount.
## Approach
The brief for this prototype recommended the use of `Alpaca Markets`, a 
> technology company headquartered in the bay area California which enables developers to build investing apps, brokerage services, trading algorithms that can access the market through its API (chrunchbase, nd)

The course recommended the use of the `tradeapi.REST` API from the `alpaca-trade-api-python` SDK to obtain stock and bond closing prices, however the `alpaca-trade-api-python` SDK is now a legacy kit as outlined on alpaca's `README.md` page on `github` where it states that support will be ending at the end of this year (githib, nd).  I elected to follow the API publisher's recommendation and use the new `get_stock_bars` API from its new `aplaca-py` SDK.

Using the new API also meant that I could not retrieve up to date market information so I resorted to retrieving data as at close of business of a `Thursday` of the week prior to current.

## References
Curnchbase. (n.d.). Alpaca. Crunchbase. Retrieved October 16, 2022, from (https://www.crunchbase.com/organization/alpacadb)

github. (n.d.) alpaca-trade-api-python. Retrieved October 16, 2022, from (https://github.com/alpacahq/alpaca-trade-api-python/)
