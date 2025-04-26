# AWS SSM Runbook to delete all RDS instances running for more than 8H

## Steps 
- input a list of OU
- input IAM cross account deployed
- describe RDS instances (same region)
- filter those running +8H
- terminate each that meet criteria (SkipFinalSnapshot=true)