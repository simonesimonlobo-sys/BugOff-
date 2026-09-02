Team BugOff — Clinkt Investigation

What we found and what we recommend:
Clinkt's August 2026 data shows a real, severe cart-abandonment problem — 70.5% of cart-adds (666 of 945) never converted to an order — but it is not catalogue-wide: four of 36 products account for 33.3% of the ₹84,857 in abandoned value, and all four show the same signature of rising browsing interest paired with collapsing conversion, ruling out falling demand as the cause. Cross-checking each flagged product against the daily inventory ledger shows this is mostly *not* a stock problem: only Bath Soap 4-Pack genuinely ran out of stock, while Orange Juice and Laundry Detergent never fell below "Low Stock" all month, meaning their conversion collapse has to originate somewhere in the cart-to-checkout path rather than the warehouse; Instant Noodles sits in between, Critical-stocked for the second half of the month without ever hitting zero. We recommend treating these as two distinct problems requiring two distinct owners — a tightened replenishment trigger for Bath Soap (it went from Low Stock to Out of Stock in five days), and a direct checkout-path audit (pricing display, delivery-slot availability, payment step) for Orange Juice and Laundry Detergent, where availability was never the constraint — plus, separately, a process fix: our own interactive dashboard prototype computed every aggregate figure exactly right but fabricated the specific product names, category labels, and customer-segment counts layered on top of those numbers, so any AI-assisted analytics output from this event should have its named entities spot-checked against the source CSVs before being trusted, not just its totals.

Report: BugOff/Clinkt_Cart_Abandonment_Research_Paper .pdf
Code / Link to website : https://clinkt-insight-report.lovable.app/
Team: 
Simone Lobo
Tanvi Shedekar
Ruchita Teli
Anushka Joshi
