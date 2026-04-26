# Expense Trends

Static, single-page web app for visualizing a personal expense log stored in JSONL format.

The page reads a local file you select (via the browser's file picker) and renders stats, charts, and a filterable transactions table — all in your browser. Nothing is uploaded; your data never leaves the device.

## Use

Open the deployed site, click **Load expenses.txt**, and pick your JSONL file.

Each line of the file is a JSON object with this shape:

```json
{"ts":"2026-04-26T10:30:00+05:30","amount":250,"currency":"INR","merchant":"Chai Shop","category":"Food & Beverage","payment_method":"upi","source":"manual","card_last4":"","raw_text":"chai 250","note":""}
```

## Stack

Plain HTML + Chart.js (via CDN). No build step.
