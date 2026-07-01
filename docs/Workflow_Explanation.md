# Workflow Explanation

## Problem

E-commerce teams often waste time manually copying order details, generating invoices, updating records, and sending customer confirmations.

## Solution

This n8n workflow automates the entire order-to-invoice process.

## Business Impact

- Saves 12+ hours/week
- Reduces invoice errors
- Speeds up customer confirmation
- Creates a clean Airtable record system
- Makes operations scalable

## Nodes Used

- Webhook
- Code node for validation and invoice calculation
- HTTP Request node for PDF generation
- Airtable node for order storage
- HTTP Request node for Twilio WhatsApp
- Respond to Webhook node
