# Client Order-to-Invoice Automation (n8n)

A portfolio-ready workflow automation project for an e-commerce client.

## Project Description

**Client Order-to-Invoice Automation | n8n, Airtable, Twilio WhatsApp, Webhooks**

- Designed automated workflow for e-commerce client replacing 12+ hours/week of manual operations.
- New orders automatically trigger PDF invoice generation, Airtable order logging, inventory-ready item tracking, and WhatsApp confirmation.
- Built a zero-manual-touch pipeline from order receipt to customer confirmation.

## What is included

```text
n8n_workflows/Client_Order_to_Invoice_Automation.json
sample_payloads/sample_order_payload.json
airtable/airtable_schema.csv
templates/invoice_template.html
templates/whatsapp_message.txt
docs/Setup_Guide.md
docs/Workflow_Explanation.md
docs/Portfolio_Case_Study.md
screenshots_guide/Screenshot_Capture_Checklist.md
```

## Workflow Steps

1. Webhook receives new order.
2. Order payload is validated.
3. Invoice totals are calculated.
4. Invoice HTML is generated.
5. PDF generation API node is triggered.
6. Airtable order record is created.
7. WhatsApp confirmation is sent through Twilio.
8. Success response is returned to the client system.

## Import in n8n

Open n8n → Workflows → Import from File → select:

```text
n8n_workflows/Client_Order_to_Invoice_Automation.json
```

Replace placeholders:

```text
YOUR_AIRTABLE_BASE_ID
YOUR_TWILIO_ACCOUNT_SID
PDF API credentials
Airtable credentials
Twilio credentials
```
