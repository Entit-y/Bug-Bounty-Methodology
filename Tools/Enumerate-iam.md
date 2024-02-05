[[Tags]] #CLI_Tool #Recon 

## Description:

Enumerate-iam tries to brute force all API calls allowed by the IAM policy.
The calls performed by this tool are all non-destructive (only get* and list* calls are performed)
AWS releases new services every quarter, to make sure that this tool is
finding all the existing permissions run:
```bash
cd enumerate_iam/
git clone https://github.com/aws/aws-sdk-js.git
python generate_bruteforce_tests.py
rm -rf aws-sdk-js
```

## Usage:
When you find an AWS *Access key* and *Secret key*, use enumerate-iam to validate them with:
```bash
enumerate-iam --access-key ACCESS_KEY --secret-key SECRET_KEY
```

