# Requirements
You need to have a valid python virtual environment manager. We recommend poetry which you can install from [here](https://python-poetry.org/docs/)

## Install the candles UI interface
If you wish to visualize the candles at the end, in a our custom web interface, please do the following:

```bash
git clone https://github.com/Cultivating-Alpha/candles-ui.git
cd candles-ui
npm install
```

# Setup
##  Install the python dependencies using poetry
```bash
poetry install 
```

Alternatively, you can install the depencies using the supplied `requirements.txt` file.

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
