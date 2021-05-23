# StockData

StockData is an API containing historical data and descriptions on over 100 stock along with crypto and minerals
#### Features

 * Free & Blazing Fast response
 * No Rate limits
 * 100+ Stocks
#### Stocks

bellow is the list of available stocks

```bash
"KIRK","DAC","CTRN","CMBM","AMTX","NMM","BGFV","RICK","RFP","DDS","SID","FNKO","BXC","TGB","STKS","UAN","HOV","HOME","NOTV","SIG","NESRW","TMST","FCX","HYRE","LOVE","NTP","TWI","AA","SBOW","UROY","TGLS","ORGO","SPLP","HRI","SBLK","OLN","RRD","FLXS","PRTY","EGLE","REPX","BBW","LB","SCHN","RILY","ANF","CVGI","AVID","CAR","JYNT","EPIX","INTT","AHT-I","MOXC","LOB","VOLT","ESEA","FUTU","CLF","AR","SMTS","GDEN","TTI","SI","AHT-F","BWMX","XPEL","BNTX","PLBY","WLMS","FLL","CROX","SIC","RCON","EGLX","HIBB","AHT-H","CX","ARCB","VSTO","CELH","GTIM","CUBI","DEN","AEO","SGRY","VEDL","KTB","MT","LXU","MKTY","TROX","GTLS","CAL","GPS","SOLY","LIVE","CPRI","AAPL","SBUX","MSFT","CSCO","QCOM","FB","AMZN","TSLA","AMD","ZNGA","GOLD","BTC-USD","OIL","SILVER"
```
#### URL Structure:
 1. Get stocks list
    - API Endpoint 
    
    ```bash 
    https://cdn.jsdelivr.net/gh/kamesguen21/StockData@main/api/stocks.json
    ```
    - Response Example 
    ```json 
    [{"SYMBOL":"KIRK"},{"SYMBOL":"DAC"},{"SYMBOL":"CTRN"}]
    ```
 2. Get stock HistoricalData
     - API Endpoint 
     
     ```bash 
     https://cdn.jsdelivr.net/gh/kamesguen21/StockData@main/api/historical/{SYMBOL}.csv
     ```
     - Response Example 
     ```csv 
     Date,Open,High,Low,Close,Adj Close,Volume
     2016-05-18,22.083570,22.468050,21.506849,21.675060,21.527481,9671078
     2016-05-19,21.434759,21.939390,21.098339,21.915359,21.766146,10212484
     2016-05-20,22.179689,22.299841,21.675060,21.891331,21.742281,7857220
     2016-05-23,22.299841,22.492081,21.939390,22.299841,22.148008,8475406
     2016-05-24,22.540140,22.948650,22.251780,22.636259,22.482136,7693134
     2016-05-25,22.852530,23.261040,22.780439,23.068800,22.911734,5824511
     2016-05-26,23.477310,23.573429,22.684320,22.852530,22.696936,6500375
     2016-05-27,22.852530,22.948650,22.371929,22.468050,22.315073,10010362
     2016-05-31,22.516109,22.780439,22.203720,22.275810,22.124142,8778277
     2016-06-01,22.107599,22.347900,21.867300,22.347900,22.195742,7075323
     ```
 3. Get stocks Descriptions
    - API Endpoint 
    ```bash 
    https://cdn.jsdelivr.net/gh/kamesguen21/StockData@main/api/description/{SYMBOL}.json
    ```
    - Response Example 
    ```json 
    {
        "logo": "https://s3.polygon.io/logos/aa/logo.png",
        "listdate": "1990-01-02",
        "cik": "1675149",
        "bloomberg": "EQ0000000045469815",
        "figi": null,
        "lei": "ABPN11VOHLHX6QR7XQ48",
        "sic": 3356,
        "country": "usa",
        "industry": "Metals & Mining",
        "sector": "Basic Materials",
        "marketcap": 6702596121,
        "employees": 14600,
        "phone": "+1 412 315-2900",
        "ceo": "Roy Christopher Harvey",
        "url": "http://www.alcoa.com",
        "description": "Alcoa Corp is an integrated aluminum company. The company engages in aluminum production from bauxite mining to manufactures finished aluminum goods. It serves finished aluminum goods to a wide-variety of industrial end markets.",
        "exchange": "New York Stock Exchange",
        "name": "Alcoa Corporation",
        "symbol": "AA",
        "exchangeSymbol": "NYE",
        "hq_address": "201 Isabella Street Pittsburgh PA, 15212-5858",
        "hq_state": "PA",
        "hq_country": "USA",
        "type": "CS",
        "updated": "11/16/2018",
        "tags": [
            "Basic Materials",
            "Aluminum",
            "Metals & Mining"
        ],
        "similar": [
            "BBL",
            "CENX",
            "KALU",
            "BHP",
            "ACH"
        ],
        "active": true
    }
    ```
 
#### Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
#### INFO
i need to find a way to make daily updates on the data, right now its just updated to 2021-05-17. stock apis are not free and i needed this for a school project.
if you need up to date data this is a nice (paid) api https://polygon.io/ or https://finance.yahoo.com/

#### License
[MIT](https://github.com/kamesguen21/StockData/blob/main/LICENSE)
