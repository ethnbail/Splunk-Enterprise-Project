
# Splunk Enterprise on Kali Linux

This project demonstrates how to set up and use Splunk Enterprise 9.4.2 on Kali Linux using the `.tgz` package. It walks through the full installation process, first-run setup, and sample SPL searches to analyze internal Splunk logs.

##  Features
- Manual Splunk Enterprise installation on Kali
- Access via web interface at `http://localhost:8000`
- First searches using Splunk's internal logs
- Redacted example logs and screenshots

##  Project Contents
- `install-guide.md`: Step-by-step setup instructions
- `logs/redacted_sample.log`: Sanitized log sample
- `configs/`: Optional sample configuration files
- `screenshots/`: Redacted UI captures

##  What You Learn
- How to manually install `.tgz` packages
- How to explore and search Splunk internal logs
- How to interpret Splunk metrics and UI access logs

## Example: Internal Sourcetype Activity Over Time

This chart shows how various Splunk sourcetypes (e.g., `splunkd`, `mongod`, `scheduler`) are producing internal log events over time.

Query used:
```spl
index=_internal | timechart count by sourcetype
