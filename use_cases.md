# Splunk Use Cases

## 1. Failed Linux Logins
SPL:
```
index=* sourcetype=linux_secure "Failed password"
| stats count by host, user
```

## 2. Windows Login Failures (Event ID 4625)
```
index=* EventCode=4625
| stats count by Account_Name, host
```

## 3. Web Server Error Responses
```
index=* sourcetype=access_combined status>=400
| stats count by status, uri_path
```
