# Task 1: Reconnaissance and Information Gathering

## Objective

The goal of this task was to identify publicly available information about the OWASP Juice Shop application and enumerate its components using tools such as Nmap and browser-based analysis.

## Step 1: Nmap Host Discovery

Command used:
```
nmap -sn juice-shop.herokuapp.com
```

Result:
- The host was confirmed to be up and running.
- Primary IP address: 54.220.192.176
- Additional IPs (suggesting load balancing): 46.137.15.86, 54.73.53.134

## Step 2: Nmap Fast Port Scan

Command used:
```
nmap -F juice-shop.herokuapp.com
```

Result:
- Port 80/tcp was open, indicating the use of HTTP.
- Port 443/tcp was open, indicating the use of HTTPS.
- 98 other ports were filtered, which is typical for cloud-hosted applications with firewall restrictions.

## Summary

The OWASP Juice Shop application is actively hosted and accessible. Nmap scans confirmed that the application is running on standard web ports. The presence of multiple IP addresses suggests a cloud-based infrastructure with possible load balancing.

Screenshots taken during this task have been included separately in the GitHub repository under the `screenshots` folder.
