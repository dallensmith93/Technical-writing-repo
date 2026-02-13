
That alone demonstrates:

- REST structure
- JSON clarity
- Professional formatting
- Logical organization

---

# 🧾 Document 2: API Integration Guide (Salesforce)

This one directly matches the job description.

---

## salesforce-integration-guide.md

```markdown
# Salesforce Integration Guide
## Submitting Hazardous Waste Reports via REST API

---

## Overview

This guide explains how to integrate Salesforce with the Hazardous Waste Reporting API to automate regulatory submission workflows.

---

## Prerequisites

- Salesforce admin access
- API credentials (Client ID & Client Secret)
- OAuth 2.0 enabled for integration user
- Access to the Environmental Reporting API

---

## Step 1: Obtain Access Token

Send a POST request to the OAuth token endpoint:

POST /oauth/token

Required fields:
- client_id
- client_secret
- grant_type
- redirect_uri

Example response:

```json
{
  "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9",
  "expires_in": 3600,
  "token_type": "Bearer"
}
