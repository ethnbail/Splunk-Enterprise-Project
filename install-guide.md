# Splunk Enterprise Install Guide on Kali Linux

##  Step 1: Download the .tgz Package
Go to the Splunk website:
https://www.splunk.com/en_us/download/splunk-enterprise.html

Select:
- Platform: Linux
- Architecture: 64-bit
- Package Type: `.tgz`

##  Step 2: Extract and Move to /opt
```bash
cd ~/Downloads
tar -xvzf splunk-9.4.2-*.tgz
sudo mv splunk /opt/
```
##  Step 3: Start Splunk and Accept License
```
sudo /opt/splunk/bin/splunk start --accept-license
```
## Step 4: Access the Web Interface
http://localhost:8000

## Step 5: Run Your First Searches

Example: index=_internal
Example: sourcetype=splunkd_ui_access
