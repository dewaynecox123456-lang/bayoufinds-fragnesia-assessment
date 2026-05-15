# BayouFinds Fragnesia Exposure Assessment
![Hero](./screenshots/hero.png)
A lightweight Linux operational exposure assessment toolkit for reviewing observable XFRM/IPsec-related runtime indicators.

## What It Does

- Runs read-only local checks
- Reviews runtime XFRM/IPsec indicators
- Checks common related modules
- Generates a professional TXT report
- Optionally exports JSON
- Provides PASS/WARN style terminal output
- Uses an operator acknowledgment prompt before execution

## What It Does Not Do

This tool does **not**:
- guarantee vulnerability status
- exploit anything
- make system changes
- replace vendor advisories
- provide legal, compliance, or incident-response certification

## Supported Platforms

Recommended:
- Fedora Linux 42+
- Fedora Silverblue / Atomic variants

Other Linux systems may run with reduced accuracy.

## Quick Run

```bash
chmod +x fragnesia-assessment.sh
./fragnesia-assessment.sh --quick
```

## JSON Export

```bash
./fragnesia-assessment.sh --quick --json
```

## Automation

```bash
./fragnesia-assessment.sh --quick --json --accept-disclaimer
```

## Exit Codes

| Code | Meaning |
|---|---|
| 0 | Low exposure |
| 1 | Warning/moderate indicators |
| 2 | High-risk indicators |
| 3 | Cancelled or missing required acknowledgment |
## Optional Download Package

A packaged release version including documentation,
example reports, release artifacts, and commercial support files
is available here:

https://bayoufinds.com/b/GBL26

© 2026 BayouFinds.com


## Permission Notes

Some ZIP extraction methods may not preserve executable
permissions on Linux shell scripts.

If needed:

```bash
chmod +x fragnesia-assessment.sh
```

Alternative execution:

```bash
bash fragnesia-assessment.sh --quick
```
