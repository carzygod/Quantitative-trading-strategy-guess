# Martingale-mesh base float margin control system

​	**Martingale-mesh (M&M) base float margin control system is a automatically risk control balancer system to avoid position liquidation cross multi-accounts , also incress the liquidity usage .**

## Abstruct

​	As we all know , M&M trading strategies are classical but powerful trading rules . Most of time , trader can make profite from this classical trading strategie by against the market risk .But M&M trading strategie still facing many issues , so it's a powerful key , but not an `any key` . 

##### The core issues of M&M are : 

- Hightly risk during facing the black swan events . Risk incress with `X^n`.
- Low liqudity usage during low market volatility.

​	To slove issues above , it require a automaticlly margin control system . The margin control system should be able to culcuate the **risk rate** of each positions & accounts , and make decision of **Hold or quit**  , which is not a part of tradition M&M rules but AI control seems like a future way .

##### M&M margin control logic :

- Single M&M mulity accounts risk control 
  - Staking all the balance into live farming . 
  - Mulity positions start up with a safe but small position margin .
  - Realtime position risk culcuate . 
  - Unstake part of balance into risk margin
  - Cut loss action (Option , AI powered)
- Mulity strategies M&M margin risk control
  - Split margin into different account with different strategies , and lable different risk rate :
    - Bigger|Smaller incress interval 
    - Bigger|Smaller incress leverage 
  - Balance the margin cross accounts to avoid liquidation 
  - Stop some of low risk account to avoid height risk account got liquidation

​	To build automatic logic program like this , require a `GOD server` to have access control to all accounts & sub-accounts , which heigly incress the risk of server contol (netwoke proxy may reduce the risk)

