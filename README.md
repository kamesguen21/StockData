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
     https://cdn.jsdelivr.net/gh/kamesguen21/StockData@main/api/historical/{SYMBOL}.json
     ```
     - Response Example 
     ```json 
     [
       {
         "date": "2016-05-18",
         "open": 689.56,
         "high": 702.54,
         "Close": 688.76,
         "Low": 697.45,
         "AdjClose": 697.45,
         "volume": 4283200
       },
       {
         "date": "2016-05-19",
         "open": 691.88,
         "high": 699.4,
         "Close": 689.56,
         "Low": 698.52,
         "AdjClose": 698.52,
         "volume": 3025600
       }
    ]
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
