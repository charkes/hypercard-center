---
title: annuity
card_id: 51607
---

# annuity

<code>annuity([ph:number1], [ph:number2])</code>

where <code>[ph:number1]</code> represents the  <b>interest rate</b> (expressed as a decimal)  and <code>[ph:number2]</code> represents the number of <b>periods</b> over which you receive annuity payments.

Value returned: the total cost of an annuity now that will pay you one unit per period over the specified number of periods, or a number equal to <code>(1 - (1 + rate) ^ -periods) / rate</code>


An interest rate involves a certain percentage (expressed as a decimal) per some unit of time—usually per year. You must use the same unit of time to measure the number of periods.

For example, if you have a yearly percentage rate but your annuity pays you monthly, use <code>rate / 12,</code> and be sure to express the number of periods as months (2 years = 24 months). 


## Examples

```
Use annuity to compute values as follows:

amountLoaned = onePayment * annuity(rate,periods) or
onePayment = amountLoaned / (annuity(rate,periods))

Example 1: You want to purchase an annuity that pays you $10,000 a year for 10 years. The interest rate on the annuity is 10%. How much will it cost you now?

amountLoaned = 10000 * annuity(.10,10) = 61445.67

Note that the annuity costs you $61,445.67, but over 10 years you actually receive $100,000. The difference, $38,554.33, is the interest you earned.

Example 2: You borrow $10,000 over 3 years at 10% interest with monthly payments. How much is each monthly payment?

onePayment = 10000 / (annuity(.10/12,3*12)) = 322.67 per month
```

## Related Topics

* [Arithmetic operators](/HyperTalkReference/operatorsandconstants/Arithmetic-operators)
* [compound](/HyperTalkReference/functions/compound)
* [numberFormat](/HyperTalkReference/properties/numberFormat)
