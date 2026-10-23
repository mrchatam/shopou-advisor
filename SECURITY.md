# Security policy

## Reporting a vulnerability

Do not open a public issue, discussion or pull request for a vulnerability.

Send it privately to the contact address on the
[support page](https://advisor.shopou.ir/support). Include:

- what the problem is and what an attacker could do with it;
- the smallest set of steps that reproduces it;
- the time you tested it, with the timezone;
- whether you want to be credited, and under what name.

Please do not include real access tokens, other people's data, or anything taken
from an account that is not yours.

## Scope

In scope:

- the connector endpoint at `https://advisor.shopou.ir/mcp`;
- the OAuth flow and token handling;
- the public pages and the favicon/font endpoints;
- the way the service talks to the retailer and to the exchange-rate source.

Out of scope:

- Digikala's own site, API or accounts;
- denial of service, load testing or automated scanning against the live service;
- missing security headers that have no demonstrated impact;
- reports produced only by a scanner, without a reproducible path.

## What to expect

This is a small, privately operated service, not a company with a security team.
Reports are acknowledged and investigated on a best-effort basis. There is no
bug bounty. Please give a reasonable amount of time to fix the issue before
disclosing it publicly.

---

## امنیت (فارسی)

آسیب‌پذیری را در ایشو یا گفت‌وگوی عمومی ننویسید. آن را خصوصی به نشانی تماسی که در
[صفحهٔ پشتیبانی](https://advisor.shopou.ir/fa/support) آمده بفرستید.

- مشکل چیست و مهاجم با آن چه کاری می‌تواند بکند؛
- کوتاه‌ترین راهی که مشکل را نشان می‌دهد؛
- زمان آزمایش، با منطقهٔ زمانی؛
- این‌که می‌خواهید نامتان ذکر شود یا نه.

توکن واقعی، دادهٔ دیگران یا چیزی از حسابی که مال شما نیست نفرستید.

سرویس کوچک و خصوصی است؛ گزارش‌ها در حد توان بررسی می‌شوند و جایزهٔ نقدی وجود ندارد.
