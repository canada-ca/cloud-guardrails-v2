# Manage Access

([Back](../README.md))

## Objective

Establish access control policies and procedures for management of all accounts.

## Applicable Service Models

- IaaS, PaaS, SaaS

## Mandatory Requirements

- Implement a mechanism for enforcing access authorizations for all user accounts, based on criteria listed in Directive on Service and Digital Appendix G – Account Management Configuration Requirements – Section 3.
- Leverage role-based access that are configured with least privileges. Use built-in roles where possible and document any custom roles created.
- Change default passwords in accordance with the GC password guidance.
- Configure the default password policy in accordance with GC Password Guidance.
- Implement password protection mechanisms to protect against password brute force attacks.
- Establish a guest user access policy and procedures that minimizes the number of guest users and manages their lifecycle where accounts are deprovisioned when access is no longer needed.

## Validation

- Demonstrate access configurations and policies are implemented for different classes of users (non-privileged, and privileged users).
- Confirm that the access authorization mechanisms have been implemented for the following:
  1. To uniquely identify and authenticate users to the cloud service;
  2. Validating that the least privilege role is assigned;
  3. Validating that Role Based Access is implemented;
  4. Terminating of role assignment upon job change or termination;
  5. Performing periodic reviews of role assignment (minimum yearly);
  6. Disabling default and dormant accounts;
  7. Avoiding use of user generic accounts.
- Verify that a review of Root/Global administrator accounts role assignment is performed at a minimum every 12 months.
- Demonstrate that cloud platform built-in roles are used with least privileges. Custom roles can be used but rationale should be documented and approved.
- Confirm that the default passwords have been changed for all the built-in accounts for the cloud-service.
- Demonstrate that password policy for the cloud platform has been configured as per the GC Password Guidance:
  1. Require longer passwords – At least 12 characters in length without a maximum length limit;
  2. Deny-list or ban common passwords and combinations, such as “Password1!”;
  3. Counter online guessing or brute forcing of passwords using throttling, account lockout policies, monitoring, and multi-factor authentication;
  4. Protect against offline attacks using effecting hashing, salting, and keyed hashing.
- Confirm that account lock out policies are enabled for all users.
- Confirm only the required guest user accounts are enabled (The required guest user accounts are as per the business requirements of the service)
- Provide list of non-organizational users with elevated privileges.

## Additional Considerations

- Document a process for managing accounts, access privileges, and access credentials for organizational users, non-organizational users (if required), based on criteria listed in Directive on Service and Digital Appendix G – Account Management Configuration Requirements – Section 3. This process should be approved by Chief Security Officer (CSO) (or delegate) and designated official for cyber security.
- Confirm that the Access Control procedure for management of administrative accounts have been documented for the cloud service. The procedure should include provision for any guest accounts, custom accounts, and must reference to the Emergency Break Glass procedure.
- Enforce just-in-time access for privileged user accounts to provide time-based and approval-based role activation to mitigate the risks of excessive, unnecessary, or misused access permissions.
- Confirm that just-in-time access for all privileged user accounts to provide time-based and approval-based role activation.
- Enforce attribute-based access control (ABAC) to restrict access based on combination of authentication factors (MFA), managed devices, device compliance, sign-in and user risks, and location.
- Provide evidence that attribute-based access control (ABAC) mechanisms are in place to restrict access based on attributes/signals such as authentication factors (MFA), managed devices, device compliance, sign-in and user risks, and location.
- Leverage tools such as privilege access management systems to enforce access control to privilege functions by configuring roles that requires approval for activation and choose one or multiple users or groups as delegated approvers
- Provide evidence that all privileged user accounts role activation requires approval, and that privilege elevation is time-bound (temporary activation).

## References

1. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), subsection 6.2.3
2. CSE Top 10 #3
3. Refer to [CCCS ITSP.30.031 V2 User Authentication Guidance for Information Technology Systems](https://cyber.gc.ca/en/guidance/user-authentication-guidance-information-technology-systems-itsp30031-v3)
4. Refer to the [Guidance on Cloud Authentication for the Government of Canada](https://intranet.canada.ca/wg-tg/cagc-angc-eng.asp)
5. Refer to the [Recommendations for Two-Factor User Authentication Within the Government of Canada Enterprise Domain](https://intranet.canada.ca/wg-tg/rtua-rafu-eng.asp)
6. Refer to the [Directive on Service and Digital](https://www.tbs-sct.canada.ca/pol/doc-eng.aspx?id=32601), [Appendix G: Standard on Enterprise Information Technology Service Common Configurations](https://www.tbs-sct.canada.ca/pol/doc-eng.aspx?id=32713) - [Account Management Configuration Requirements](https://www.canada.ca/en/government/system/digital-government/policies-standards/enterprise-it-service-common-configurations/account.html)
7. Refer to ITSP.50.104 Guidance on defence in depth for cloud-based services, subsection 4.6
8. [GC Password Guidance](https://www.canada.ca/en/government/system/digital-government/online-security-privacy/password-guidance.html)

Related security controls: AC‑2, AC‑2(1), AC‑2(7) AC‑3, AC‑3(7), AC‑3, AC‑4 AC‑5, AC‑6, AC‑6(5), IA‑2, IA‑2(1), IA‑2(8), IA‑2(11), IA‑4, IA‑5, IA‑5(1), IA‑5(6)
