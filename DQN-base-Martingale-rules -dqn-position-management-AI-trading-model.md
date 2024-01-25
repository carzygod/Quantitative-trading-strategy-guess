# DQN-base-Martingale-rules -dqn-position-management-AI-trading-model

**This draft is to build a DQN trading model with martingale trading rules , Base trading system are designed by humen using martingale & mesh , DQN model doing position control . **

## Training method :

- Open
- Close
- Height
- Low
- LongSize
- LongUnfinishedProfite
- ShortSize
- ShortUnfinishedProfite

## Output actions

- 0 //Do nothing and continue
- 1 //Close long position
- 2 //Close short position
- 3 //Close all position

## Expect result :

- Model trading with martingale trading rules . 
- Cut the risk before martingale unhandled . // Position risk control
- Cut the porfite-max for position 
  - Define max porfite rate 
  - Model define self porfite
- Close positions when meeting risk market environment 

## Coding

- Martingale position mock data system
  - Make martingale listen .
  - Make train data feed .
- Normalized system
  - Normalized the raw data.
- Training system
  - Mock train as virtual environment .