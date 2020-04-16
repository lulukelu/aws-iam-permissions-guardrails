---
layout: default
---



## AWS Billing

| Identifier    | Guardrail                                                                                                   | Rationale                                                                                                                                                                                                                                                     | Remediation                                                           | References                                                                                                                                             | IAM Actions                                                                                             |
|:--------------|:------------------------------------------------------------------------------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------|:--------------------------------------------------------------------------------------------------------|
| IAM-BILLING-1 | Check that the ability to modify or update AWS Billing options are only assumable to authorized principals. | In all AWS environments, ensure that only billing administrators and authorized principals should be able to update or modify AWS Billing options. Unauthorized modifications could affect your billing payments or account information such as email address | For unauthorized principals, either remove the associated IAM Actions | [https://docs.aws.amazon.com/IAM/latest/UserGuide/list_awsbilling.html](https://docs.aws.amazon.com/IAM/latest/UserGuide/list_awsbilling.html)<br><br> | aws-portal:ModifyBilling<br><br>aws-portal:ModifyAccount<br><br>aws-portal:ModifyPaymentMethods<br><br> |