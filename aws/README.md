
# AWS Brute Force Protection Scripts

#### Authors: @jfersec  
#### License: MIT  

## Overview

This folder contains scripts to block IPs on AWS using WAFv2. These scripts are designed to work with AWS Web ACLs to prevent brute-force and malicious attacks.

### Scripts

- **`block-ip-aws.sh`**: Blocks IPv4 addresses.
- **`block-ip-v6-aws.sh`**: Blocks IPv6 addresses.
- **`deploy-aws-web-acl.sh`**: Deploys a Web ACL.

### Setup

1. Configure `config.sh` with:
   - `WEB_ACL_NAME`
   - `IP_SET_ID`
   - `WEB_ACL_REGION`

2. Install AWS CLI and configure credentials:
   ```bash
   aws configure
   ```

### Usage

Run a script, for example:
```bash
./block-ip-aws.sh 192.168.1.1
```

### Notes

- Ensure AWS credentials are correctly set.
- Test configurations before deployment.
