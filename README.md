# StripeCashOps

**Hackathon:** Stripe Hackathon  
**Builder:** Hossam Elshahaby  
**Date:** October 3, 2026  
**Track:** Track 2 - Accounting  
**Live demo:** https://stripecashops.lovable.app  
**Pitch video:** https://youtu.be/cLdgKzmBh-s

## Overview

StripeCashOps helps small businesses turn accounting documents into payment actions. The app reads invoices, receipts, and payment records, finds overdue or risky invoices, creates Stripe payment links, and prepares customer reminders.

The goal is simple: help business owners recover cash faster without spending hours checking documents manually.

## Problem

Small businesses often lose time and money because invoices, receipts, and payment records live in different places. Owners and service providers need to check old invoices, bank statements, and tickets by hand. As a result, unpaid invoices stay hidden for weeks, payment follow-up happens late, and cash flow becomes harder to manage.

## Solution

StripeCashOps acts as an invoice-to-cash assistant. It converts messy accounting inputs into a prioritized recovery workflow:

- extracts invoice and receipt data
- flags overdue, duplicate, partial, and risky payments
- ranks invoices by urgency and recoverable cash
- creates Stripe payment links
- drafts or sends payment reminder emails
- keeps a fallback copyable reminder draft when email sending is unavailable

## Key Features

- **Cash recovery dashboard:** shows overdue amount, recoverable cash, processed invoices, and reconciliation confidence.
- **Document inbox:** organizes invoices, receipts, restaurant tickets, and bank-statement records.
- **Risk detection:** highlights overdue invoices, duplicate invoice IDs, VAT mismatches, and partial payments.
- **Stripe payment action:** generates payment links for selected invoices.
- **Reminder workflow:** uses Brevo email with a verified sender for demo reminders, with copyable drafts as fallback.
- **Demo mode:** keeps the product usable even when a connector or live email service is unavailable.

## Stripe Integration

The prototype uses Stripe test-mode flows for payment recovery. The intended production workflow connects each overdue invoice to a Stripe payment link or checkout session, then tracks payment status through Stripe events.

## Demo Script

1. Open the live app: https://stripecashops.lovable.app
2. Review the dashboard to see recoverable cash.
3. Select an overdue invoice.
4. Generate or view the Stripe payment link.
5. Draft or send the reminder email.
6. Mark the invoice as ready to send or paid in the workflow.

## Impact

StripeCashOps helps small teams reduce manual accounting work, follow up faster, and recover cash that would otherwise sit unpaid. For accountants and business owners, the value is direct: fewer hours spent reconciling documents and a faster path from invoice discovery to payment.

## Production Roadmap

- connect a verified business email domain for stronger deliverability
- add stable Stripe webhooks for payment status updates
- integrate OCR for uploaded invoices and receipts
- add bank transaction import and matching
- build accountant review queues for low-confidence cases
- support multi-business workspaces

## Submission Details

**Project name:** StripeCashOps  
**Category:** Accounting automation  
**Website:** https://stripecashops.lovable.app  
**Pitch video:** https://youtu.be/cLdgKzmBh-s  
**Builder:** Hossam Elshahaby  
