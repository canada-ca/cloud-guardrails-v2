# Protect user accounts and identities

([Back](../README.md))

## Objective

Protect User Accounts and Identities.

## Applicable Service Models

- IaaS, PaaS, SaaS

## Mandatory Requirements

- Implement phishing-resistant multi-factor authentication (MFA) for all user accounts.

  (Note: User accounts and identities include:

  1. Root/Global administrator (as it is one that that has enhanced/highest level of privileges over the control plane and addresses all aspects of access control).
  2. Other Administrative user accounts. Refer to Section 4 of the “[Directive on Service and Digital- Canada.ca](https://www.tbs-sct.canada.ca/pol/doc-eng.aspx?id=32601), [Appendix G: Standard on Enterprise Information Technology Service Common Configurations- Canada.ca](https://www.tbs-sct.canada.ca/pol/doc-eng.aspx?id=32713) - [Account Management Configuration Requirements - Canada.ca](https://www.canada.ca/en/government/system/digital-government/policies-standards/enterprise-it-service-common-configurations/account.html)” for the definition of privileged accounts.
  3. Regular user accounts)

- Configure alerting to ensure the prompt detection of a potential compromise, in accordance with the GC Event Logging Guidance.
- Use separate dedicated accounts to administer cloud services to minimize the blast radius.

## Validation

- Confirm that MFA is enabled and enforced as per GC guidance through screenshots, compliance reports, or compliance check enabled through a reporting tool for all user accounts.

  (Note: The admin needs to be prompted for MFA every login. Break glass accounts are exempted from MFA)

- Confirm and report the count of Root/Global administrator registered (should have at least two and no more than 5).
- Confirm if monitoring and auditing is implemented for all user accounts.
- Confirm alert notification to the authorized personnel is implemented for flagging misuse, suspicious sign-in attempts, or when changes are made to all user accounts.
- Provide evidence that dedicated user accounts are used for administration (e.g., privileged access).

## Additional Considerations

None.

## References

1. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), subsection 6.2.3
2. CSE Top 10 #3
3. Refer to the [Recommendations for Two-Factor User Authentication Within the Government of Canada Enterprise Domain](https://intranet.canada.ca/wg-tg/rtua-rafu-eng.asp)
4. [Refer to the GC Multi-Factor Authentication (MFA) Strategy Paper](https://www.gcpedia.gc.ca/gcwiki/images/9/9e/GC_MFA_Strategy.pdf)
5. Refer to the [Directive on Service and Digital- Canada.ca](https://www.tbs-sct.canada.ca/pol/doc-eng.aspx?id=32601), [Appendix G: Standard on Enterprise Information Technology Service Common Configurations- Canada.ca](https://www.tbs-sct.canada.ca/pol/doc-eng.aspx?id=32713) - [Account Management Configuration Requirements - Canada.ca](https://www.canada.ca/en/government/system/digital-government/policies-standards/enterprise-it-service-common-configurations/account.html)
6. Refer to the [template](https://gcconnex.gc.ca/file/view/55010566/break-glass-emergency-account-procedure-departments-can-use-to-develop-their-emergency-access-management-controls-for-cloud?language=en) for a break glass emergency account management procedure.
7. Refer to the [GC Event Logging Guidance](https://www.gcpedia.gc.ca/gcwiki/images/e/e3/GC_Event_Logging_Strategy.pdf).

Related security controls: AC-2, AC-2(11), AC-3, AC-5, AC-6, AC- 6(5), AC- 6(10), AC-19, AC – 20 (3), IA-2, IA-2(1)
IA - 2(2), IA-2(3), IA – 2(11), IA-5(8), SI-4, SI-4(5), SA-4(12), CM-5.
