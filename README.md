# Shopou Advisor

A shopping assistant for ChatGPT that plans a **purchase**, not a search. You say
what you are setting up, what you already own and what you can spend; it reads
live Digikala listings and answers with a complete set, an itemized total, and
the fits it could not verify.

It is read-only. There is no cart, no checkout, no payment and no order — every
purchase still happens on the retailer's own site, under the retailer's terms.

This repository is the public place to ask questions and report problems. The
server code is private; nothing here runs the connector.

## Using it

1. In ChatGPT, open **Settings → Apps & Connectors**.
2. Choose **Create**, give it a name, and paste the connector address:
   `https://advisor.shopou.ir/mcp`.
3. Ask in your own words — a goal, a budget and what you already own:

   > A pour-over coffee setup for one or two cups, up to 6.5 million toman. I
   > already have a gooseneck kettle.

The connector's address, the three illustrated steps and the support page are on
the site: [advisor.shopou.ir](https://advisor.shopou.ir) ·
[فارسی](https://advisor.shopou.ir/fa).

## Before you open an issue

- **Prices move, and every answer says when it was read.** A price from a few
  hours ago may already be wrong; ask the assistant again first.
- **"Prices unavailable" is not "nothing in your budget."** It means the retailer
  could not be read. Try again in a few minutes.
- **"Unverified" compatibility means exactly that.** The listing did not state
  the fact needed to check the fit. The answer says which fact is missing and
  where to find it.
- **Orders, payments, delivery, returns, warranty and Digikala account problems**
  belong to Digikala support, not this service. It never places an order.

## Reporting a problem

Use the issue templates:

- **Connector problem** — it would not connect, sign-in failed, a tool returned
  an error, or an answer was clearly wrong.
- **Price or listing is wrong** — a price, stock state, seller or product detail
  does not match the listing.
- **Question or suggestion** — anything else.

Please include:

- the local date and time, with the timezone;
- what you asked, in the words you used;
- which answer or tool was involved;
- the exact error text, if there was one;
- the language of the page or conversation (English or Persian).

If you call the service directly with `curl` or your own client, every response
carries an `x-correlation-id` header. Include that value — it is how the request
is found in the server log.

**Never paste access tokens, refresh tokens, passwords, API keys or personal
information into an issue.** Nothing in a report needs them. A chat client does
not show response headers, so inside ChatGPT the time of the message is the best
identifier.

## Privacy

No account to create, no cookies, no analytics. The service keeps its cache and
counters in memory only, and writes nothing to a database or to disk. What is
processed, what reaches Digikala and what is kept is written out at
[advisor.shopou.ir/privacy](https://advisor.shopou.ir/privacy)
([فارسی](https://advisor.shopou.ir/fa/privacy)).

## Security

Please do not report a vulnerability in a public issue. Use the contact address
on the [support page](https://advisor.shopou.ir/support) instead.

## License

This repository contains no source code. The service is operated privately; no
license is granted for the connector or its output.
