# API Versioning Policy

---

## Overview

This document defines the versioning standards for the Environmental Reporting API to ensure backward compatibility, predictable upgrades, and clear deprecation timelines.

---

## Versioning Strategy

The API follows Semantic Versioning:

MAJOR.MINOR.PATCH

- MAJOR: Breaking changes
- MINOR: Backward-compatible feature additions
- PATCH: Bug fixes and non-breaking improvements

Example:
v1.2.0

---

## Backward Compatibility

Minor and patch releases must maintain backward compatibility.

Breaking changes require:
- Incrementing the major version number
- Clear migration documentation
- Minimum 90-day deprecation notice

---

## Deprecation Policy

When an endpoint is deprecated:

1. Deprecation notice is published in release notes.
2. Documentation is updated with a "Deprecated" label.
3. Sunset timeline is provided.
4. Replacement endpoint (if applicable) is documented.

---

## Version Identification

API versions are specified in the URL path:

/v1/reports/hazardous-waste

Future versions will follow:

/v2/...

---

## Documentation Alignment

All documentation updates must be version-specific.

Archived documentation will remain accessible for deprecated versions until official sunset.
