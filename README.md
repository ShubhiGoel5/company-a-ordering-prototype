# Direct ordering prototype

A clickable prototype of a restaurant chain's own ordering platform, built as a design and behaviour exercise.

It is a single static file, `index.html`, with no build step and no dependencies.

## Three screens (switch with the "Demo controls" button, bottom left)

| Screen | Route | What it shows |
|---|---|---|
| Customer website | `#home` | Menu, cart, checkout, order tracking, party orders, rewards |
| Kitchen display | `#kitchen` | Live orders, timers, late colouring, busy mode, out of stock |
| Admin console | `#admin` | Dashboard, menu and prices, outlets, party requests, loyalty rules |

## Try this

1. Add the Chicken dum biryani (Family pack), go to checkout, apply `DIRECT10`, use points, pay (test).
2. Demo controls > Kitchen display. The order is in NEW. Tap Accept.
3. Demo controls > "Jump to 21:20", then pick Kukatpally: order #146 shows red, "LATE +4 MIN".
4. To watch the kitchen update live while ordering, open the page in a second tab.

## What is real and what is not

Real behaviour: outlet by area, delivery or pickup, portions and add-ons, coupons, loyalty points, 5% GST shown as included, a promise time (higher of the prep estimate and the outlet minimum, plus delivery, rounded to 5 minutes), late alerts at +10 minutes, auto-cancel when nobody accepts, out-of-stock pausing, busy mode, offline tablet handling.

Not real: the database, payment gateway, SMS and WhatsApp (all simulated), food photos (SVG illustrations), and the brand name, which is a placeholder. All data is synthetic.
