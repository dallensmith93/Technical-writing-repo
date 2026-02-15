# Error Handling Standards

---

## Overview

Consistent error responses improve integration reliability and troubleshooting efficiency.

All API error responses must follow a standardized schema.

---

## Error Response Schema

```json
{
  "error": {
    "code": "INVALID_REQUEST",
    "message": "The 'facilityId' field is required.",
    "details": [
      {
        "field": "facilityId",
        "issue": "Missing required field"
      }
    ]
  }
}
