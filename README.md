# Installation
Run the installation script: `./install.sh`

The script does the following

1. Install the python dependencies using poetry
```bash
poetry install 
```

2. Install the candles UI interface
```bash
git clone git@github.com:Cultivating-Alpha/candles-ui.git
cd candles-ui
npm install
```


## Run the jupyter notebook
The notebook is located under `./src/main.ipynb`

It does the following:
1. Generate random data
2. Generate a moving average crossover
3. Backtest the strategy
4. Optimize the strategy to find winning parameters
5. Plot equity in matplotlib
6. Export the OHLC, indicators, and trades data to the candle-ui folder



## Run Candles UI 
Once the jupyter notebook runs, do the following:
```bash
cd candles-ui
npm run dev
```

Then navigate to `http://localhost:3000/` to see the UI`
