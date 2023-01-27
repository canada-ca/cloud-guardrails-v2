# Protection of Data-in-Transit

([Back](../README.md))

## Objective

Protect data transiting networks through the use of appropriate encryption and network safeguards

## Applicable Service Models

- IaaS, PaaS, SaaS

## Mandatory Requirements

- Encrypt data in transit by default (e.g., TLS v1.2, etc.) to protect the confidentiality and integrity of data, including for all publicly accessible sites and external communications as per the GC Website and Services Configuration Requirements, and wherever possible for internal zone communication.
- Use CSE-approved cryptographic algorithms and protocols, in accordance with ITSP.40.111 and ITSP.40.062.
- Leverage non-person entity certificates from certificate authorities that align with the Recommendations for TLS Server Certificates.

## Validation

- Confirm that TLS v1.2 or above encryption is implemented for all cloud services (via HTTPS, TLS or other mechanism).
  (Note: While this is often the default, cloud platforms and cloud services often have configuration options to select the permitted TLS version.)
- Cryptographic algorithms and protocols configurable by the consumer are leveraged in accordance with ITSP 40.111 and 40.062.
- Confirm that NPE certificates are issued from certificate authorities that align with GC recommendations for TLS server certificates.

## Additional Considerations

None

## References

1. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), subsection 6.2.4
2. [ITPIN 2018-01](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/policy-implementation-notices/implementing-https-secure-web-connections-itpin.html)
3. Refer to the cryptography guidance in [ITSP.40.111](https://cyber.gc.ca/en/guidance/cryptographic-algorithms-unclassified-protected-and-protected-b-information-itsp40111) and [ITSP.40.062](https://www.cse-cst.gc.ca/en/system/files/pdf_documents/itsp.40.062-eng.pdf).
4. Refer to the network security zoning guidance in [ITSG-22](https://cyber.gc.ca/en/guidance/baseline-security-requirements-network-security-zones-government-canada-itsg-22) and [ITSG-38](https://cyber.gc.ca/en/guidance/network-security-zoning-design-considerations-placement-services-within-zones-itsg-38).
5. Refer to the guidance in [Considerations for Cryptography in Commercial Cloud Services](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/cloud-services/government-canada-consideration-use-cryptography-in-cloud.html).
6. [Government of Canada Recommendations for TLS Server Certificates for GC Public Facing Web Services](https://wiki.gccollab.ca/images/9/92/Recommendations_for_TLS_Server_Certificates_-_14_May_2021.pdf)

Related security controls: IA-7,SC12, SC13, SC28, SC28(1)
