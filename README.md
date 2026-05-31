MEV (Maximul Extractable Value)
The extra profit that blockchain block producers (validators in PoS or miners in PoW) can earn by reordering, including, or excluding transactions 
in a block beyond the standard block rewards and gas fees. 

**Problem**
In DeFi, bots front-run trades (MEV), Users lose money silently. 
**Solution**
Encrypted transaction execution
-Trade details hidden until execution
-No front-running possible

MEVSHIELD is a prototype for full private DeFi trading.

MEV protection layer
-The shield toggle shows the real price difference between protected (~0.05% fee) vs unprotected (~2.6% loss to MEV)
-Live bot-attempt feed in the sidebar ,new front-run and sandwich attack attempts appear every ~4 seconds, all marked "Blocked"
-Block counter increments in real time to simulate chain activity

Core trading flow
-Token swap UI with live quote calculation across ETH, USDC, WBTC, and DAI pairs
-Adjustable slippage with commit-window blocks that scale accordingly
-4-step encryption pipeline that actually runs when you hit "Execute" watch it walk through hash → commit → reveal → settle

