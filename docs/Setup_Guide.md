# Setup Guide

## 1. Import workflow

Import this file in n8n:

```text
n8n_workflows/Client_Order_to_Invoice_Automation.json
```

## 2. Airtable setup

Create a base:

```text
Order Automation CRM
```

Tables:

### Orders

- Order ID
- Invoice No
- Customer Name
- Customer Phone
- Grand Total
- Status
- Payment Method
- Order Date

### Order Items

- Order ID
- Invoice No
- SKU
- Product Name
- Quantity
- Unit Price
- Line Total

### Inventory

- SKU
- Product Name
- Stock Quantity
- Reorder Level
- Status

## 3. Twilio setup

Use Twilio WhatsApp Sandbox for testing.

Default sandbox sender:

```text
whatsapp:+14155238886
```

In Twilio HTTP node:

```text
Username: Twilio Account SID
Password: Twilio Auth Token
```

## 4. PDF generation setup

Use any PDF API:

- PDFShift
- PDF.co
- APITemplate
- DocRaptor

Replace credentials in `Generate PDF Invoice` node.

## 5. Test with Postman

Method:

```text
POST
```

URL:

```text
YOUR_N8N_WEBHOOK_TEST_URL
```

Header:

```text
Content-Type: application/json
```

Body:

```text
sample_payloads/sample_order_payload.json
```
