## Trading description

The trading is done in the Binance market platform, which of course, does not have markets for every altcoin pair. The default bridge currency is Tether (USDT), which is stable by design and compatible with nearly every coin on the platform.
- satdevelop.com

<p align="center">
  Coin A → USDT → Coin B
</p>

<div align="center">
  <p><b>Coin A</b> → USDT → Coin B</p>
  <p>Coin B → USDT → Coin C</p>
  <p>...</p>
  <p>Coin C → USDT → <b>Coin A</b></p>
</div>

The bot jumps between a configured set of coins on the condition that it does not return to a coin unless it is profitable in respect to the amount held last. The risk is that one of the coins may freefall relative to the others all of a sudden, attracting our reverse greedy algorithm.

## Binance Setup

- Create a [Binance account](https://www.binance.com/en/register?ref=13222128) (Referral: Doan Duc Tin).
- Enable Two-factor Authentication.
- Create a new API key.
- Get a cryptocurrency. If its symbol is not in the default list, add it.

## Tool Setup

- None

### Install Python dependencies

Run: `pip install -r requirements.txt`.

### Create user configuration

- Editting the configurations file to run
- This step fowards need my private instruction [Contact me](https://fb.com/satfomacej)

**The configuration file consists of the following fields:**

- **api_key** - Binance API key generated in the Binance account setup stage.
- **api_secret_key** - Binance secret key generated in the Binance account setup stage.
- **current_coin** - This is your starting coin of choice. This should be one of the coins from your supported coin list. If you want to start from your bridge

#### Environment Variables

All of the options provided in `user.cfg` can also be configured using environment variables.

```
CURRENT_COIN_SYMBOL:
SUPPORTED_COIN_LIST: "XLM TRX ICX EOS IOTA ONT QTUM ETC ADA XMR DASH NEO ATOM DOGE VET BAT OMG BTT"
BRIDGE_SYMBOL: USDT
API_KEY: vmPUZE6mv9SD5VNHk4HlWFsOr6aKE2zvsw0MuIgwCIPy6utIco14y7Ju91duEh8A
API_SECRET_KEY: NhqPtmdSJYdKjVHjA7PZj4Mge3R5YNiP1e3UZjInClVN65XAbvqqM6A7H5fATj0j
SCOUT_MULTIPLIER: 5
SCOUT_SLEEP_TIME: 1
TLD: com
STRATEGY: default
BUY_TIMEOUT: 0
SELL_TIMEOUT: 0
```

### Run

```
contact www.satdevelop.com
```

### Docker

```shell
docker-compose up
```

```shell
docker-compose up -d sqlitebrowser
```

## Testing

## Developing
