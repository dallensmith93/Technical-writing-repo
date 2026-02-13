# Hazardous Waste Reporting API

## Overview

The Hazardous Waste Reporting API allows authorized systems to submit, retrieve, and manage hazardous waste disposal records for regulatory compliance tracking.

Base URL:
https://api.environmentalreporting.gov/v1

---

## Authentication

All endpoints require OAuth 2.0 Bearer Token authentication.

Include the token in the request header:

Authorization: Bearer {access_token}
Content-Type: application/json

---

## Submit Hazardous Waste Report

### Endpoint

POST /reports/hazardous-waste

### Description

Submits a new hazardous waste disposal record for compliance monitoring.

---

### Request Body

```json
{
  "facilityId": "FAC-10023",
  "wasteType": "Industrial Solvent",
  "quantity": 500,
  "unit": "gallons",
  "disposalMethod": "Incineration",
  "disposalDate": "2026-02-15",
  "reportedBy": {
    "name": "John Smith",
    "email": "john.smith@example.com"
  }
}

{
  "reportId": "REP-483920",
  "status": "Submitted",
  "timestamp": "2026-02-15T14:22:03Z"
}
