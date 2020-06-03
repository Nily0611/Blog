#### Snapshot 403 error

Error codes
```
        "type": "a_w_s_security_token_service_exception",
        "reason": "User: arn:aws:sts::acountid:assumed-role/cp-sts-grant-role/swift-region-prod-365021432299 is not authorized to perform: sts:AssumeRole on resource: role-arn (Service: AWSSecurityTokenService; Status Code: 403; Error Code: AccessDenied; Request ID: some-id)"
```

Solution

Edit trust relationships, make sure, `es.amazonaws.com` is in your trust entity list.
