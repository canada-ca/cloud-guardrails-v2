# Plan for Continuity

([Back](../README.md))

## Objective

Ensure that there is a plan for continuity of access and service that accommodates both expected and unexpected events.

## Applicable Service Models

- IaaS, PaaS, SaaS

## Mandatory Requirements

- Document, implement, and test a break glass emergency account management process.
- Obtain signature from Departmental Chief Information Officer (CIO) and Chief Security Officer (CSO) to confirm acknowledgement and approval of the break glass emergency account management procedures.

## Validation

- Verify that a break glass emergency account management procedure has been developed
- Verify that break glass accounts are not subject to MFA, ABAC or AACS policies
- Verify that alerting is in place to report any use of break glass accounts
- Verify that testing of break glass account took place, and that periodic testing is included in break glass emergency account management procedure.
- Confirm through attestation that the Departmental Chief Information Officer (CIO) and Chief Security Officer (CSO) have approved the break glass emergency account management procedure for the cloud service.

## Additional Considerations

- Develop a cloud backup strategy that takes into account where GC data is stored, replicated, or backed up by the cloud service, in consideration of the IT continuity plan for the service/application.
- Confirm through attestation that the cloud backup strategy procedure is developed and approved by the business owner.
- Verify if there are scripts that support the ability to restore from code (e.g., infrastructure as code).
- Ensure that cloud workloads are associated with the applicable Application ID in the TBS Application Portfolio Management (APM) tool, in support of the Standard on At-Risk Technology.
- Provide a list of all software, including versions, deployed on VMs associated with the application IDs from APM.
- Ensure departmental cyber security event management plans include cloud services, in alignment with the GC Cyber Security Event Management Plan.
- Provide a list of all software, including versions, deployed on VMs associated with the application IDs from APM

## References

1. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html)
2. Refer to the [template](https://gcconnex.gc.ca/file/view/55010566/break-glass-emergency-account-procedure-departments-can-use-to-develop-their-emergency-access-management-controls-for-cloud?language=en) for a break glass emergency account management procedure.
3. Refer to the [Department Cyber Security Event Management Plan (CSEMP) Template](https://www.gcpedia.gc.ca/gcwiki/images/6/66/Department_CSEMP_Template.docx).

Related security controls: AC-1, CP-1,CP-2,CP-9,CA-3
