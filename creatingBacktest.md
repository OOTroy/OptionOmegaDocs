# Getting Started

## Running your first backtest
To create a new backtest, hit the "New Backtest" button on your dashboard

![](images/newBacktestButton.png)

## Tickers
We offer backtesting in SPY, SPX, QQQ, and IWM

![](images/ticker.png)

## Dates
You can test as far back as 1/1/13 and as most recent as yesterday.

![](images/dates.png)

We have some nice little bubbles with popular timeframes that will autopopulate for you

![](images/dates1.png)

If you notice on the "End Date" field, we have a little arrow. That will populate the last available trading day

![](images/dates2.png)

## Common Strategies

Under the "Strategy" section, we have a list of common strategies that you can choose from. Below is information about each one.

*Please note, all examples are from The Options Playbook and Tastytrade.*.

- [Butterfly](https://www.optionsplaybook.com/option-strategies/long-call-butterfly-spread/)
- [Calendar](https://www.optionsplaybook.com/option-strategies/calendar-call-spread/)
- [Double Calendar](https://www.tastytrade.com/news-insights/double-calendar-spread-mechanics)
- [Iron Condor](https://www.optionsplaybook.com/option-strategies/iron-condor/)
- [Iron Fly](https://www.optionsplaybook.com/option-strategies/iron-butterfly/)
- [Jade Lizard](https://www.tastytrade.com/concepts-strategies/jade-lizard)
- [Long Call](https://www.optionsplaybook.com/option-strategies/long-call/)
- [Long Call Spread](https://www.optionsplaybook.com/option-strategies/long-call-spread/)
- [Long Put](https://www.optionsplaybook.com/option-strategies/long-put/)
- [Long Put Spread](https://www.optionsplaybook.com/option-strategies/long-put-spread/)
- [Ratio Spread](https://www.tastytrade.com/concepts-strategies/ratio-spread)
- [Short Call](https://www.optionsplaybook.com/option-strategies/short-call/)
- [Short Call Spread](https://www.optionsplaybook.com/option-strategies/short-call-spread/)
- [Short Put](https://www.optionsplaybook.com/option-strategies/short-put/)
- [Short Straddle](https://www.optionsplaybook.com/option-strategies/short-straddle/)
- [Short Strangle](https://www.optionsplaybook.com/option-strategies/short-strangle/)
## Strategy

### Strike Selection Type

*Please note, you can only choose one selection for all legs in the trade*.

![](images/whatKindOfLeg.png)

By default, the option legs will be based on delta
![](images/deltaLeg.png)
*Notice the delta symbol in the "type column" between the QTY and the DTE fields*.

You can also use Percentage OTM (Out of the Money)
![](images/otmLeg.png)
*Notice the percentage symbol in the "type column" between the QTY and the DTE fields*.

You can also use Percentage OTM (Out of the Money)
![](images/percentageLeg.png)
*Notice the dollar symbol in the "type column" between the QTY and the DTE fields*.

### Option Legs

What is an option leg? At the end of the day, a leg is made up of type (put or call), direction (buy or sell), and days to expiration (DTE)

type (put or call)

![](images/callLeg.png)
![](images/putLeg.png)

direction (buy or sell)

![](images/sellLeg.png)
![](images/buyLeg.png)

quantity (qty) of each leg

![](images/qtyLeg.png)

days to expiration (dte)

![](images/dteLeg.png)

### Linked Legs

There are some strategies that require different things. For instance, when you are selling a put spread that is 10-wide, 
you will need to know what the short leg's strike is before you can buy a leg 10 points away. Another example would be if you are buying a calendar.
You will need to know what the short strike is for the front month before you can purchase the long strike for the back month.
To solve this, Option Omega uses the concept of "Linked Legs".

In order to link a leg, we will use this magical button here:

![](images/linkButton.png)

When you click that button you will see that the button highlights and a new leg drops down underneath.

![](images/linkedLeg.png)

Notice on the bottom leg that the spot where your selection type goes looks different than the one above.

![](images/linkedLegOffset.png)

We default this to 0 for you. That means that as it currently stands, the bottom leg will be the same strike price as the top leg. 
This is useful for time spreads where you have different option legs with different days to expiration. For example, a common long calendar strategy:

![](images/calendarStrategy.png)


Let's say we wanted to sell a 25 delta put spread and we wanted the spread to be 10 points wide. How would we go about setting that up?

![](images/25DeltaPutSpread.png)

The top leg shows us selling a 25 delta put and the bottom leg has an offset of -10. It is important to remember that 
negative values in the offset mean down the option chain.

How about if we wanted to sell a 25 delta call spread and we wanted the spread to be 50 points wide. How would we go about setting that up?

![](images/50DeltaCallSpread.png)

The top leg shows us selling a 25 delta call and the bottom leg has an offset of +50. It is important to remember that
positive values in the offset mean up the option chain.




## Entry Conditions
> Entry Conditions

## Exit Conditions
> Stuff about strategies

## Misc
> Stuff about strategies