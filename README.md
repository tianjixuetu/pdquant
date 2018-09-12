# pdquant
This module mainly use pandas to do backtest and live trading on python.

pandas's dataframe is very similar to MS EXCEL,what-you-see-is-what-you-get,

this property can make you test your startegy and do a live trading.

now,the first value is used to test currency,and trade in oanda.In the future,

this module may assit stock,future,fund,and so on.

# key concept

A strategy contains :

1.when to open a trade in  position size

2.when to close the trade that has opened before

3.whether to add or minus the position

4.whether to stop loss or take profit

position size contains:

1.the same position size  overrall the strategy

2.the position size is a same percentage of your value 

3.the position size change according some conditions

columns contains:

1.datas:open,high,low,close,volume,and so on.

2.signals:which decide buy\sell\close

3.position:which decide we buy or sell how much size

4.cash:how much cash in your account

5.cash_used:how much cash you have used to buy or sell

6.position_value:how much value about your positions.

7.value:how much about your account

8.return:how much log return you got from every period.

performance contains:

according to the daily return,this module will use pyfolio module

to calculate the performance.

# backtest

if you use the vector backtest:all you need do is to use the datas to generate the siganls if your position size

don't changes about some conditions,except your value.

if you use the for-loop backtest,you need generates the signals and position size.

# live trading

if you use a for-loop mode,you can use this mode to generate signals and position size,then,this module will 

creat order and trade in the oanda

# note

this is just the version0.1,so,there maybe somebugs,if you use this module backtest and trade,you should bear the consequences





