---
title: compound
card_id: 54407
---

# compound

`compound([ph:number1], [ph:number2])`

where `[ph:number1]` represents the <b>interest rate</b> (expressed as a decimal) and `[ph:number2]` represents the number of <b>periods</b> over which the interest is compounded.

Value returned: value of one unit of principal invested at the interest rate and compounded over the specified number of periods, or a number equal to `(1 + rate) ^ periods`

An interest rate involves a certain percentage (expressed as a decimal) per some unit of time—usually per year. You must use the same unit of time to measure the number of periods.

For example, if you have a yearly interest rate that is compounded monthly, you must convert the  yearly rate to the interest per month (`rate / 12`) and be sure to express the number of periods as months (2 years = 24 months).

## Examples

```
Use compound to compute a future value as follows:

futureValue = principal * compound(rate,periods)

Example 1: $100 invested for 20 years at 10% interest compounded yearly.

futureValue = 100 * compound(.10,20) = 672.75

The net gain over the original investment is 672.75 - 100 = 572.75. Note that $100 invested for 20 years at 10% simple interest (which applies only to the principal) yields $300, for a net gain of only $200.

Example 2: $100 invested for 20 years at 10% interest compounded monthly.

futureValue = 100 * compound(.10/12,20*12) = 732.81
```

## Demo Script

<code><pre>
on compoundDemo
  set numberFormat to "0.00"
  answer "$100 invested for 5 years at 5.75% interest" &&¬
  "compounded quarterly yields $" & (100 * compound(.0575/4,5*4))
end compoundDemo
</pre></code>

## Related Topics

* [annuity](/HyperTalkReference/functions/annuity)
* [Arithmetic operators](/HyperTalkReference/operatorsandconstants/Arithmetic-operators)
* [numberFormat](/HyperTalkReference/properties/numberFormat)
