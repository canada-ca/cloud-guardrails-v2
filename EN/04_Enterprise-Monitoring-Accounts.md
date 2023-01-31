# Enterprise Monitoring Accounts

([Back](../README.md))

## Objective

Create role-based account to enable enterprise monitoring and visibility

## Applicable Service Models

- IaaS, PaaS, SaaS

## Mandatory Requirements

- Enable enterprise visibility by establishing monitoring roles for GC approved stakeholders with read-only access following the least privilege principle to support validation of:
  - billing information
  - security configuration as part of cloud guardrails monitoring
- Review access privileges periodically and remove access when it is no longer required.

## Validation

- Verify that roles required to enable GC visibility to have been provisioned/assigned.
- Confirm alert notification to the authorized personnel is implemented flagging misuse, suspicious sign-in attempts, or when changes are made to the privileged and non-privileged accounts.

## Additional Considerations

None

## References

1. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), subsection 6.2.3
2. CSE Top 10 #2

Related security controls: AC-3(7), AC-6(5), IA-2(1)
