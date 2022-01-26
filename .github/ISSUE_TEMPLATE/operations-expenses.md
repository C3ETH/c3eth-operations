---
name: Team Expenses
about: Monthly expense payments
title: 'Operations [Expenses]: Pay team expenses for MONTH.'
labels: 'Documentation:Process, Operations:Administration, Treasury:Payments, Treasury:Reporting'
assignees: 'wolstaeb, cardanoz'
---

As per our consensus and #102, pay @C3ETH/c3eth-team remuneration for [MONTH] 2022. Perform the payment in one transaction for transparency and accountability purposes.

- [ ] See #102 more for details, and any meeting notes to confirm expenses. 
- [ ] Check expenses have been recorded in the [Accounting Sheet](https://bit.ly/3fV4buo).
- [ ] Get the 7-Day Average USD/ADA price from [coinmarketcap.com](https://bit.ly/3fVrYKT). See details below.
- [ ] [Update compensation spreadsheet](https://bit.ly/3H1G8G7) with exchange rate, and
- [ ] Work out Ada/Lovelace amounts
- [ ] Double Check amounts and put them into payment script
- [ ] [Transfer total amount needed]() to the local payment address.
- [ ] Update script with input transaction details
- [ ] [Perform the renumeration payment]()
- [ ] [Notify the @C3ETH/c3eth-team of the transaction]().
- [ ] Backup payment script details.
- [ ] Document transaction details

---
## Transaction Details

Links above document the expenses and the two associated transactions.

### Coin marketcap 7-Day rate

For Payment we use a simple seven day average to devise the payment conversion rates at the approximate time (within 30mins of) the payments being made. The USD/ADA rate is calculated using the following data points from Coinmarket Cap 7D prices. The intention is to smooth out fluations in the USD/ADA exchange rates.

```
ADA-7DA = (7DOPEN + 7DCLOSE + HIGH + LOW) / 4
```

Where: 7DOPEN, 7DCLOSE, HIGH, LOW are USD/ADA prices. HIGH and LOW are the Coinmarket Cap 7d Low/High, and the 7DSTART and 7DCLOSE are taken from the seven day window of the chart below.
