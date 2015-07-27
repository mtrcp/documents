#Microsoft Trusted Root Certificate Program Audit Requirements

This page sets out the requirements for Certification Authorities (CAs) who participate in the Microsoft Trusted Root Certificate Program ("Program") along with the requirements to use each of the EKUs that Microsoft currently supports as part of the Microsoft Trusted Root Certificate Program. Below you will find the requirements for both Commercial CAs and Government CAs along with information about what constitutes a Government CA. (See "Definitions", below). Additionally, you will find information about how the requirements are changing for Government CAs. 
________________________________________
##1 General Requirements

Microsoft requires that every CA submit evidence of a Qualifying Audit on an annual basis for the CA and any non-limited root within its PKI chain. A Qualifying Audit must meet the following four main requirements: (A) the auditor must be qualified, (B) the audit must be performed using the proper scope, (C) the audit must be performed using the proper standard, and (D) the audit must be performed and the attestation letter must be issued within the proper time period. It is the responsibility of the CA to provide Microsoft with a letter attesting to the results of the audit as well as conformance to the Audit Requirements in a timely manner.

###A. The Auditor's Qualifications
Microsoft considers an auditor to be a Qualified Auditor if s/he is an independent individual or company that is certified to perform certification authority audits by one of these three authorities: (1) WebTrust, (2) an ETSI Equivalent National Authority (published at http://aka.ms/ena) or, (3) in the case of a Government CA, the government itself. (For more information on Government CAs, see " Government CA Requirements" below.) 

If a CA chooses to obtain a WebTrust audit, Microsoft requires the CA to retain a WebTrust licensed auditor to perform the audit. The full list of WebTrust-licensed auditors is available at http://aka.ms/webtrustauditors. If a CA chooses to obtain an ETSI-based audit, Microsoft requires the CA to retain an authorized entity by an Equivalent National Authority (or "ENAs"). A catalogue of acceptable ENAs is based on the list at http://aka.ms/ena. If a CA is operated in a country that does not have an ETSI Equivalent National Authority, Microsoft will accept an audit performed by an auditor that is qualified under an Equivalent National Authority in the auditor's home country.

###B. The Scope of the Audit
The scope of the audit must include all roots, non-limited sub-roots, and cross-signed non-enrolled roots, under the root, except for sub-roots that are limited to a verified domain. The audit must also document the full PKI hierarchy. The final audit statements must be in a publicly-accessible location and must contain the start and end dates of the audit period. In the case of a WebTrust audit, WebTrust seal(s) must also be in a publicly-accessible location.

###C. Point-in-Time Readiness Assessments
Microsoft requires an audit prior to commencing commercial operations. For commercial CAs that have not been operational as an issuer of certificates for 90 days or more, Microsoft will accept a point-in-time readiness audit conducted by a Qualified Auditor. If the CA uses a point-in-time readiness audit, Microsoft requires a follow-up audit within 90 days after the CA issues its first certificate.

###D. The Time Period between the Assessment and the Auditor's Attestation
Microsoft requires that the CA obtain a conforming audit annually. To ensure that Microsoft has information that accurately reflects the current business practices of the CA, the attestation letter arising from the audit must be dated and received by Microsoft not more than 3 months from the ending date specified in the attestation letter.
________________________________________
##2. Conventional CA Audit Standards
The Program accepts two types of audit standards: WebTrust and ETSI. For each of the EKUs on the left, Microsoft requires an audit that conforms to the standard marked.

###A. WebTrust Audits

<table class="telerik-reTable-2" border="0" cellspacing="3" cellpadding="0" style="width:99%;">
<tbody>
<tr class="telerik-reTableHeaderRow-2">
<td class="telerik-reTableHeaderFirstCol-2">
<p>&nbsp;</p>
</td>
<td class="telerik-reTableHeaderOddCol-2">
<p>WebTrust Principles and Criteria for Certification Authorities - WebTrust for CAs 2.0
</p>
</td>
<td class="telerik-reTableHeaderEvenCol-2">
<p>WebTrust Principles and Criteria for Certification Authorities - SSL Baseline with Network Security - Version 2
</p>
</td>
<td class="telerik-reTableHeaderOddCol-2">
<p>WebTrust Principles and Criteria for Certification Authorities - Extended Validation SSL - Version 1.4.5
</p>
</td>
<td class="telerik-reTableHeaderLastCol-2">
<p>WebTrust Principles and Criteria for Certification Authorities - Extended Validation Code Signing
</p>
</td>
</tr>
<tr class="telerik-reTableOddRow-2">
<td class="telerik-reTableFirstCol-2">
<p>Server Authentication (non-EV)</p>
</td>
<td class="telerik-reTableOddCol-2">
<p>X</p>
</td>
<td class="telerik-reTableEvenCol-2">
<p>X</p>
</td>
<td class="telerik-reTableOddCol-2"></td>
<td class="telerik-reTableLastCol-2"></td>
</tr>
<tr class="telerik-reTableEvenRow-2">
<td class="telerik-reTableFirstCol-2">
<p>Server Authentication (non-EV) and Client Authentication only</p>
</td>
<td class="telerik-reTableOddCol-2">
<p>X</p>
</td>
<td class="telerik-reTableEvenCol-2">
<p>X</p>
</td>
<td class="telerik-reTableOddCol-2"></td>
<td class="telerik-reTableLastCol-2"></td>
</tr>
<tr class="telerik-reTableOddRow-2">
<td class="telerik-reTableFirstCol-2">
<p>Server Authentication (EV)</p>
</td>
<td class="telerik-reTableOddCol-2">
<p>X</p>
</td>
<td class="telerik-reTableEvenCol-2">
<p>X</p>
</td>
<td class="telerik-reTableOddCol-2">
<p>X</p>
</td>
<td class="telerik-reTableLastCol-2"></td>
</tr>
<tr class="telerik-reTableEvenRow-2">
<td class="telerik-reTableFirstCol-2">
<p>Server Authentication (EV) and Client Authentication only</p>
</td>
<td class="telerik-reTableOddCol-2">
<p>X</p>
</td>
<td class="telerik-reTableEvenCol-2">
<p>X</p>
</td>
<td class="telerik-reTableOddCol-2">
<p>X</p>
</td>
<td class="telerik-reTableLastCol-2"></td>
</tr>
<tr class="telerik-reTableOddRow-2">
<td class="telerik-reTableFirstCol-2">
<p>EV Code Signing</p>
</td>
<td class="telerik-reTableOddCol-2">
<p>X</p>
</td>
<td class="telerik-reTableEvenCol-2"></td>
<td class="telerik-reTableOddCol-2"></td>
<td class="telerik-reTableLastCol-2">
<p>X</p>
</td>
</tr>
<tr class="telerik-reTableEvenRow-2">
<td class="telerik-reTableFirstCol-2">
<p>Non-EV Code Signing and Time stamping</p>
</td>
<td class="telerik-reTableOddCol-2">
<p>X</p>
</td>
<td class="telerik-reTableEvenCol-2"></td>
<td class="telerik-reTableOddCol-2"></td>
<td class="telerik-reTableLastCol-2"></td>
</tr>
<tr class="telerik-reTableOddRow-2">
<td class="telerik-reTableFirstCol-2">
<p>Secured Email (S/MIME)</p>
</td>
<td class="telerik-reTableOddCol-2">
<p>X</p>
</td>
<td class="telerik-reTableEvenCol-2"></td>
<td class="telerik-reTableOddCol-2"></td>
<td class="telerik-reTableLastCol-2"></td>
</tr>
<tr class="telerik-reTableEvenRow-2">
<td class="telerik-reTableFirstCol-2">
<p>Client Authentication (without Server Authentication)</p>
</td>
<td class="telerik-reTableOddCol-2">
<p>X</p>
</td>
<td class="telerik-reTableEvenCol-2"></td>
<td class="telerik-reTableOddCol-2"></td>
<td class="telerik-reTableLastCol-2"></td>
</tr>
<tr class="telerik-reTableOddRow-2">
<td class="telerik-reTableFirstCol-2">
<p>Document Signing</p>
</td>
<td class="telerik-reTableOddCol-2">
<p>X</p>
</td>
<td class="telerik-reTableEvenCol-2"></td>
<td class="telerik-reTableOddCol-2"></td>
<td class="telerik-reTableLastCol-2"></td>
</tr>
</tbody>
</table>

###B. ETSI-Based Audits

<table class="telerik-reTable-2" border="0" cellspacing="3" cellpadding="0" style="width:99%;">
<tbody>
<tr class="telerik-reTableHeaderRow-2">
<td class="telerik-reTableHeaderFirstCol-2">
<p>&nbsp;</p>
</td>
<td class="telerik-reTableHeaderOddCol-2">
<p>ETSI TS 102 042 V2.4.1 or later (DVCP, OVCP or PTC-BR policies) - Electronic Signatures and Infrastructures (ESI); Policy requirements for certification authorities issuing public key certificates
</p>
</td>
<td class="telerik-reTableHeaderEvenCol-2">
<p>ETSI TS 102 042 V2.4.1 or later (EVCP or EVCP&#43; policies) - Electronic Signatures and Infrastructures (ESI); Policy requirements for certification authorities issuing public key certificates
</p>
</td>
<td class="telerik-reTableHeaderOddCol-2">
<p>ETSI TS 102 042 V2.4.1 or later (EVCG policy) - Electronic Signatures and Infrastructures (ESI); Policy requirements for certification authorities issuing public key certificates
</p>
</td>
<td class="telerik-reTableHeaderEvenCol-2">
<p>ETSI TS 102 042 V2.4.1 or later (LCP, NCP, NCP&#43; policies) - Electronic Signatures and Infrastructures (ESI); Policy requirements for certification authorities issuing public key certificates
</p>
</td>
<td class="telerik-reTableHeaderLastCol-2">
<p>ETSI TS 101 456 V1.4.3 or later - Electronic Signatures and Infrastructure (ESI); Policy requirements for certification authorities issuing qualified certificates
</p>
</td>
</tr>
<tr class="telerik-reTableOddRow-2">
<td class="telerik-reTableFirstCol-2">
<p>Server Authentication (non-EV)</p>
</td>
<td class="telerik-reTableOddCol-2">
<p>X</p>
</td>
<td class="telerik-reTableEvenCol-2"></td>
<td class="telerik-reTableOddCol-2"></td>
<td class="telerik-reTableEvenCol-2"></td>
<td class="telerik-reTableLastCol-2"></td>
</tr>
<tr class="telerik-reTableEvenRow-2">
<td class="telerik-reTableFirstCol-2">
<p>Server Authentication (non-EV) and Client Authentication only</p>
</td>
<td class="telerik-reTableOddCol-2">
<p>X</p>
</td>
<td class="telerik-reTableEvenCol-2"></td>
<td class="telerik-reTableOddCol-2"></td>
<td class="telerik-reTableEvenCol-2"></td>
<td class="telerik-reTableLastCol-2"></td>
</tr>
<tr class="telerik-reTableOddRow-2">
<td class="telerik-reTableFirstCol-2">
<p>Server Authentication (EV)</p>
</td>
<td class="telerik-reTableOddCol-2"></td>
<td class="telerik-reTableEvenCol-2">
<p>X</p>
</td>
<td class="telerik-reTableOddCol-2"></td>
<td class="telerik-reTableEvenCol-2"></td>
<td class="telerik-reTableLastCol-2"></td>
</tr>
<tr class="telerik-reTableEvenRow-2">
<td class="telerik-reTableFirstCol-2">
<p>Server Authentication (EV) and Client Authentication only</p>
</td>
<td class="telerik-reTableOddCol-2"></td>
<td class="telerik-reTableEvenCol-2">
<p>X</p>
</td>
<td class="telerik-reTableOddCol-2"></td>
<td class="telerik-reTableEvenCol-2"></td>
<td class="telerik-reTableLastCol-2"></td>
</tr>
<tr class="telerik-reTableOddRow-2">
<td class="telerik-reTableFirstCol-2">
<p>EV Code Signing</p>
</td>
<td class="telerik-reTableOddCol-2"></td>
<td class="telerik-reTableEvenCol-2"></td>
<td class="telerik-reTableOddCol-2">
<p>X</p>
</td>
<td class="telerik-reTableEvenCol-2"></td>
<td class="telerik-reTableLastCol-2"></td>
</tr>
<tr class="telerik-reTableEvenRow-2">
<td class="telerik-reTableFirstCol-2">
<p>Non-EV Code Signing and Time stamping</p>
</td>
<td class="telerik-reTableOddCol-2">
<p>X</p>
</td>
<td class="telerik-reTableEvenCol-2"></td>
<td class="telerik-reTableOddCol-2"></td>
<td class="telerik-reTableEvenCol-2">
<p>X</p>
</td>
<td class="telerik-reTableLastCol-2">
<p>X</p>
</td>
</tr>
<tr class="telerik-reTableOddRow-2">
<td class="telerik-reTableFirstCol-2">
<p>Secured Email (S/MIME)</p>
</td>
<td class="telerik-reTableOddCol-2">
<p>X</p>
</td>
<td class="telerik-reTableEvenCol-2"></td>
<td class="telerik-reTableOddCol-2"></td>
<td class="telerik-reTableEvenCol-2">
<p>X</p>
</td>
<td class="telerik-reTableLastCol-2">
<p>X</p>
</td>
</tr>
<tr class="telerik-reTableEvenRow-2">
<td class="telerik-reTableFirstCol-2">
<p>Client Authentication (without Server Authentication)</p>
</td>
<td class="telerik-reTableOddCol-2">
<p>X</p>
</td>
<td class="telerik-reTableEvenCol-2"></td>
<td class="telerik-reTableOddCol-2"></td>
<td class="telerik-reTableEvenCol-2">
<p>X</p>
</td>
<td class="telerik-reTableLastCol-2">
<p>X</p>
</td>
</tr>
<tr class="telerik-reTableOddRow-2">
<td class="telerik-reTableFirstCol-2">
<p>Document Signing</p>
</td>
<td class="telerik-reTableOddCol-2">
<p>X</p>
</td>
<td class="telerik-reTableEvenCol-2"></td>
<td class="telerik-reTableOddCol-2"></td>
<td class="telerik-reTableEvenCol-2">
<p>X</p>
</td>
<td class="telerik-reTableLastCol-2">
<p>X</p>
</td>
</tr>
</tbody>
</table>
________________________________________
##3. Government CA Requirements
Effective July 1, 2015, Government CAs may choose to either obtain the above WebTrust or ETSI-based audit(s) required of Commercial CAs, or to use an Equivalent Audit. If a Government CA chooses to obtain a WebTrust or ETSI-based audit, Microsoft will treat the Government CA as a Commercial CA. The Government CA can then operate without limiting the certificates it issues, provided it issues commercial (including non-profit) certificates from a different root than its government certificates and it signs a commercial CA contract with Microsoft.
###A. Equivalent Audit Restrictions
If the Government CA chooses not to use a WebTrust or ETSI audit, it may obtain an Equivalent Audit. In an Equivalent Audit ("EA"), the Government CA selects a third party to perform an audit. The audit has two purposes: (1) to demonstrate that the Government CA complies with local laws and regulations related to certificate authority operation, and (2) to demonstrate that the audit substantially complies with the relevant WebTrust or ETSI standard.

If a Government CA chooses to obtain an EA, Microsoft will limit the scope of certificates that the Government CA may issue. Government CAs that issue server authentication certificates must limit the root to government-controlled domains. Governments must limit the issuance of any other certificates to ISO3166 country codes that the country has sovereign control over.

Government CAs must also accept and adopt the appropriate, CAB forum baseline requirements for CAs based on the type of certificates the root issues. However, the Program Requirements and Audit Requirements supersede those requirements in any aspect in which they are in conflict.

Effective June 1, 2015, all Government CAs entering the Program will be subject to the above EA requirements. All Government CAs that are part of the Program prior to June 1, 2015 will be subject to the above EA requirements immediately upon expiration of their then-current audit.

###B. Content of the Equivalent Audit Report
Microsoft requires all Government CAs that submit an EA to provide an attestation letter from the auditor that:

1.	Attests that the audit is issued by an independent agency which is authorized by the Government CA's government to conduct the audit; 

1. 	Lists the Government CA's government's criteria for auditor qualification, and certifies that the auditor meets this criteria; 

1. 	Lists the particular statutes, rules, and/or regulations that the auditor assessed the Government CA's operations against; 

1. 	Certifies the Government CA's compliance with the requirements outlined in the named governing statutes, rules, and/or regulations; 

1. 	Provides information that describes how the statute's requirements are equivalent to the appropriate WebTrust or ETSI audit(s) ; 

1. 	Lists Certificate Authorities and third parties authorized by the Government CA to issue certificates on the Government CA's behalf within a certificate chain; 

  1. 	Documents the full PKI hierarchy; and 
  1.	Provides the start and end date of the audit period. 
 
________________________________________
###5. Definitions

A "Government CA" is either (1) an entity that is established by the sovereign government of the jurisdiction in which the entity operates, and whose existence and operations are directly or indirectly subject to the control of the sovereign government anywhere in the PKI chain, or (2) signs the Government Program Agreement.

A "Commercial CA" is an entity that is legally recognized in the jurisdiction(s) in which the entity operates (e.g., corporation or other legal person), that operates on a for-profit basis, and that issues digital certificates to other CAs or to the general public and that signs the Commercial Program Agreement. 

"Certification Authority" or "CA" means an entity that issues digital certificates in accordance with Local Laws and Regulations. 

"Local Laws and Regulations" means the laws and regulations applicable to a CA under which the CA is authorized to issue digital certificates, which set forth the applicable policies, rules, and standards for issuing, maintaining, or revoking certificates, including audit frequency and procedure. 
      
________________________________________
<h3><a name="Related"></a>6. Related</h3>
<p><a title="Go to the Microsoft Trusted Root Certificate Main Page" href="http://aka.ms/rootcert">Microsoft Trusted Root Program Requirements main page</a></p>
<p><br />



