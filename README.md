# PineScript-SMC-Strategy
 The strategy create based on SMC strategy

Pine Script SMC Strategy
This repository contains a Pine Script strategy based on the Smart Money Concept (SMC). The strategy identifies key areas in the market such as order blocks and liquidity sweeps, which are often used by institutional traders (smart money) to make high-probability trades.

Features
Order Blocks:
Identifies and plots bullish and bearish order blocks using rectangles.
These zones represent areas of high buying (demand) or selling (supply) pressure.
Liquidity Sweeps:
Identifies liquidity grabs by detecting liquidity floors (sweep below lows) and liquidity ceilings (sweep above highs).
Helps to highlight areas where the market may reverse after hunting liquidity.
Risk-Reward Management:
The script calculates take-profit (TP) and stop-loss (SL) levels dynamically based on recent highs and lows, with a customizable risk-reward ratio.
How It Works
This strategy uses the following components:

Market Structure Shifts (MSS): Identifies shifts in market structure when price breaks a previous high or low.
Order Blocks: Plots demand and supply zones (order blocks) as rectangles based on these shifts.
Liquidity Sweeps: Highlights liquidity sweeps when price wicks above recent highs or below recent lows, often followed by a reversal.
Trade Entries:
Long Trades: Triggered after a liquidity sweep below recent lows, followed by a bullish candle.
Short Trades: Triggered after a liquidity sweep above recent highs, followed by a bearish candle.
Stop-Loss and Take-Profit: Automatically calculated based on the risk-reward ratio (default 2:1).
Pine Script Code
The Pine Script code for this strategy can be found in the smc_strategy.pine file.

Parameters:
Risk-Reward Ratio: Customizable ratio to control risk management in your trades.
Order Block Colors: Colors used to highlight bullish and bearish order blocks.
Installation
Copy the smc_strategy.pine code.
Go to TradingView.
Open the Pine Script editor and paste the code.
Apply the script to your chart to visualize the order blocks, liquidity sweeps, and trade signals.
Usage
The script identifies high-probability zones for entering trades based on SMC principles.
Use the bullish and bearish order blocks as potential support and resistance zones.
Use liquidity sweeps to spot potential reversals after a liquidity grab.
Adjust the risk-reward ratio to suit your trading style.