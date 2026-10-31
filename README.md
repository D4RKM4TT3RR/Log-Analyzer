# Log-Analyzer
# SSH Log Analyzer

A simple Python tool that parses SSH authentication logs and flags
potential brute-force attacks based on failed login attempt thresholds.

## Usage
1. Export your SSH logs: `sudo journalctl -u ssh --since "1 day ago" > auth-review.log`
2. Run: `python3 log_analyzer.py`

Flags any user/IP combination with 5+ failed attempts as a possible
brute-force attempt.

## Built while studying for CompTIA Security+.
