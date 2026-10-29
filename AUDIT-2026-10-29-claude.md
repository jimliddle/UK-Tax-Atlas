# UK Tax Atlas: follow-up review, 29 October 2026

**Reviewed by Claude (Anthropic), 29 October 2026.** Baseline: commit `493877d`, 257 records, carrying the ChatGPT-6 reconciliation in [AUDIT-2026-10-29.md](AUDIT-2026-10-29.md). After this review: 262 records, of which 253 are distinct mechanisms once cross-references are excluded.

## Summary

Every Budget 2026 entry I could match against HM Treasury's overview of tax legislation and rates was correct, and the headline corrections in the earlier audit hold up. The problems were elsewhere. One live VAT relief had the wrong geography. Several core entries had never been updated for Budget 2025 measures that took effect in April 2026, even though the README claimed reconciliation against that Budget. Five statutory citations pointed at the wrong Act, Part or section. Five household-relevant charges were missing entirely, and 54 of the Budget 2026 records carried placeholder text where the atlas's distinctive payer and bearer analysis should be.

All of the changes below have been made in `index.html`. Record numbers are the `#item-ID` anchors on the site.

## Factual corrections

| # | Entry | Was | Now |
|---|---|---|---|
| 213 | Domestic electricity VAT 0% | UK-wide; "Announced — to 30 June 2027" | Great Britain only (Northern Ireland stays at 5%). In force since 1 October 2026; Budget 2026 extended the end date from 31 March to 30 June 2027. |
| 75 | Value Added Tax | Gave domestic electricity as a reduced-rate example | Notes the GB zero rate and the NI reduced rate. |
| 178 | Diverted Profits Tax | Current | Replaced for accounting periods beginning on or after 1 January 2026 by the Unassessed Transfer Pricing Profits charge within corporation tax (main rate plus 6 points, TIOPA 2010 Part 4A). |
| 181 | Economic Crime Levy | Finance Act 2022, Part 3 | Economic Crime (Transparency and Enforcement) Act 2022, Part 3, with corrected link. |
| 139 | Bank Levy | Finance Act 2011 s.17 | Finance Act 2011 s.73 and Sch 19. |
| 88 | Lottery Duty | Finance Act 1993 s.21 | Finance Act 1993 Part I Chapter II, charge at s.24. |
| 92 | Machine Games Duty | Finance Act 2012 Part 5 | Finance Act 2012 Part 6 (s.191 and Sch 24). |
| 180 | Domestic Top-up Tax | Finance (No. 2) Act 2023 Part 3 | Part 4. Part 3 is the multinational top-up tax. |
| 101 | London Congestion Charge | Transport Act 2000 Sch 23 | Greater London Authority Act 1999 s.295 and Sch 23. |
| 54 | Visitor levy | "Implementation underway", no link | Current in Edinburgh (5% since 24 July 2026); linked to the Visitor Levy (Scotland) Act 2024. |
| 177, 204 | Property income tax | Only Scotland could set its own property rates | Scotland and Wales can both do so under existing income tax powers; 24/44/49 is the default for England, Wales and NI. |
| 68 | Mansion tax proposals | "Not enacted", with no link to the surcharge | Cross-referenced to the High Value Council Tax Surcharge (#67) and narrowed to wider proposals. |
| Header | Intro text | "Last updated on the 15th June 2026" | Last updated 29 October 2026. |
| Wealth tab | HVCTS row | "Centrally administered … not a local council-tax band" | A nationally set surcharge billed by councils alongside Council Tax. |

## Entries brought up to date

- **#24 Dividend Tax:** the ordinary and upper rates rose to 10.75% and 35.75% from 6 April 2026 (Finance Act 2026 s.4). The additional rate stays at 39.35%.
- **#91 Remote Gaming Duty:** up from 21% to 40% from 1 April 2026 (Finance Act 2026 s.86).
- **#89 General Betting Duty:** a new 25% remote betting rate applies from 1 April 2027.
- **#121 Renewables Obligation:** 75% of its costs have been paid from general taxation since April 2026.
- **#125 Energy Company Obligation:** funding ended on 31 March 2026, so the record is now historical. I have not changed #127, the Great British Insulation Scheme. It probably ended at the same time, but I could not confirm that.
- **#82 Soft Drinks Industry Levy:** added the 2026/27 rates of £2.08 and £2.78 per 10 litres.
- **#15, #17, #30, #31 frozen thresholds:** added the end dates. Income tax and NIC thresholds are frozen to April 2031. The IHT nil-rate band and residence nil-rate band are frozen to 5 April 2031.
- **#67 and #200 High Value Council Tax Surcharge:** added the bands (£2,500 to £7,500 a year), owner liability, CPI uprating from 2029/30 and the deferral option. #200 is now scoped to England.
- **#114 Air Passenger Duty:** noted that APD stops applying in Scotland from 1 April 2027.
- **#12 Student loans:** the Plan 2 threshold stays frozen at £29,385.
- **#16 High Income Child Benefit Charge:** Child Benefit overpayments can now be set against the charge.
- **#29 Inheritance Tax:** IHT now turns on residence rather than domicile since April 2025.

## Records added

- **#257 VAT on private school fees:** 20% since 1 January 2025. Private schools in England also lost charitable business rates relief from April 2025.
- **#258 Winter Fuel Payment charge:** a charge equal to the payment, applied to pensioners with total income over £35,000 from winter 2025. It applies UK-wide, including Scotland's Pension Age Winter Heating Payment.
- **#259 Scottish Air Departure Tax:** replaces APD in Scotland from 1 April 2027.
- **#260 Low-value imports customs duty relief removal:** relief on consignments of £135 or less ends in October 2028, brought forward by Budget 2026.
- **#261 Motability scheme VAT and IPT:** applies to new leases from 1 July 2026.

## Data quality

- **Payer, bearer and scope:** the 54 Budget 2026 records that said "Varies by measure", "Statutory taxpayer/operator as specified" or "Households may bear direct or indirect effects" now name the legal payer and the likely bearer. The placeholder scope "UK-wide unless specified" was replaced throughout, with correct nation scope where the measure is devolved or territorial. This covers business rates, the council tax surcharge, SDLT, Landfill Tax, Carbon Price Support, the gas standing charges and APD after April 2027.
- **Cross-references:** seven Budget 2026 records that restate an existing entry are now flagged `crossref`, as #59 and #176 already were. They still appear in the catalogue with a cross-ref badge, but the dashboard no longer counts them as separate mechanisms. The records are #187, #198, #200, #204, #205, #222 and #224.
- **Typos:** fixed in the introduction, the AI note and the disclaimer.

## Not verified, and suggestions

I could not confirm two Budget 2026 entries from the published Budget text:

- the detail of #197, the removal of business rates relief for vape shops and adult gaming centres;
- the wording of #242, the cost control framework.

I also could not confirm the title of the SAF mandate order cited in #116.

The planned levy on aviation fuel suppliers to fund the SAF revenue certainty mechanism is a candidate for a future record once its start date is confirmed.

65 records link to the top of the Budget 2026 overview rather than the relevant paragraph. Adding paragraph references would make each claim checkable in one click.

Local fees, per-authority tariffs and historic legislation links not mentioned above were outside the scope of this review.

## Sources

- [HM Treasury, Budget 2026: overview of tax legislation and rates](https://www.gov.uk/government/publications/budget-2026-overview-of-tax-legislation-and-rates-ootlar/budget-2026-overview-of-tax-legislation-and-rates-ootlar)
- [HM Treasury, Budget 2026](https://www.gov.uk/government/publications/budget-2026-document/budget-2026-html)
- [HM Treasury, Budget 2025: overview of tax legislation and rates](https://www.gov.uk/government/publications/budget-2025-overview-of-tax-legislation-and-rates-ootlar/budget-2025-overview-of-tax-legislation-and-rates-ootlar)
- [HMRC, temporary zero rate of VAT for domestic electricity in Great Britain](https://www.gov.uk/government/publications/temporary-zero-rate-of-vat-for-domestic-electricity-in-great-britain/temporary-zero-rate-of-vat-in-great-britain-for-domestic-electricity)
- [HMRC, Unassessed Transfer Pricing Profits (INTM489105)](https://www.gov.uk/hmrc-internal-manuals/international-manual/intm489105)
- [Finance Act 2026](https://www.legislation.gov.uk/ukpga/2026/11/contents)
- [Economic Crime (Transparency and Enforcement) Act 2022, Part 3](https://www.legislation.gov.uk/ukpga/2022/10/part/3)
- [Visitor Levy (Scotland) Act 2024](https://www.legislation.gov.uk/asp/2024/8/contents)
- [High Value Council Tax Surcharge](https://www.gov.uk/government/publications/high-value-council-tax-surcharge/high-value-council-tax-surcharge)
- [What the Autumn Budget means for your energy bills](https://www.gov.uk/government/news/what-does-the-autumn-budget-mean-for-your-energy-bills)
- [Revenue Scotland, Air Departure Tax](https://www.revenue.scot/air-departure-tax)
- [HMRC, Winter Fuel Payments charge](https://www.gov.uk/government/publications/income-tax-charge-on-winter-fuel-payments/winter-fuel-payments-charge)
- [HMRC, VAT on private school fees](https://www.gov.uk/government/publications/vat-on-private-school-fees)
- [Building Safety Levy (England) Regulations 2025](https://lawplayer.com/uk/act/uksi-2025-1236)

This review is not a certification that every entry is correct. Check any specific liability with HMRC, the devolved revenue authorities or a qualified adviser.
