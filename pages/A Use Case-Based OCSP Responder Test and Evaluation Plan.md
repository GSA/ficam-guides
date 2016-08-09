---
layout: page
title: A Use Case-based OCSP Responder Test and Evaluation Plan
permalink: /A Use Case-based OCSP Responder Test and Evaluation Plan/
---
###A Use Case-based OCSP Responder Test and Evaluation Plan  
  
  
  
#####GSA FIPS 201 Evaluation Program  
#####August 2016  

---

####Introduction
This playbook describes use case scenarios for an OCSP responder product and provides a suite of
tests that determine whether the responder meets the requirements in those scenarios.

####Background
GSA's most current [OSCP Responder Approval Procedures] (https://www.idmanagement.gov/IDM/servlet/fileField?entityId=ka0t0000000TNVtAAO&field=File__Body__s) is no longer synchronized with 
the Validation System testing being performed by the GSA Evaluation Program.  Similarly, the 
DoD's Online Certificate Status Protocol Responder Interoperability Master Test Plan is out-of-date
with today's signing key sizes.  Neither test plan addresses many of the use cases that have
developed over the past decade.  The goal of this playbook is to enable the community to add use case
scenarios and to provide one or more test cases to determine that a give OSCP responder product
can be used with that use case.

Some use cases and test plans have been "borrowed" from both the JITC Master Test Plan as well as the GSA approval
procedures for the GSA OCSP Responder Approval Procedures.

####Standards
This playbook was initially written based on standards in effect at the time of writing.  As newer normative publications
are released by NIST, these references will need to be updated. We'll be using:
  * [FIPS 201-2 Personal Identity Verification \(PIV\) of Federal Employees and Contractors] (http://dx.doi.org/10.6028/NIST.FIPS.201-2)
  * [FIPS 180-4 Secure Hash Standard (SHS)] (dx.doi.org/10.6028/NIST.FIPS.180-4)
  * [NIST SP 800-78-4 Cryptographic Algorithms and Key Sizes for Personal Identity Verification] (http://dx.doi.org/10.6028/NIST.SP.800-78-4)
  * [RFC 6960 X.509 Internet Public Key Infrastructure Online Certificate Status Protocol - OCSP] (https://tools.ietf.org/html/rfc6960)
  * [RFC 6066 Transport Layer Security \(TLS\) Extensions: Extension Definitions] (https://tools.ietf.org/html/rfc6066)
  
####1. Mandatory Requirements
The requirements in this section are mandatory for all OCSP responder products.  It
assumes that the responder is connected to the Internet and can access all CRLs
and CA certificates necessary for verifying signed requests and initiating TLS
sessions (including OCSP stapling CA chains to TLS handshake responses).

#####1.1 Handle an Unsigned OCSP Request for a Single Certificate Using HTTP
######1.1.1 Good
TODO: Describe the use case for an unsigned OCSP request for a single good certificate and what the desired response should look like.  
TODO: Describe the test procedure needed to verify the response.   
######1.1.2 Revoked
TODO: Describe the use case for an unsigned OCSP request for a single revoked certificate and what the desired response should look like.  
TODO: Describe the test procedure needed to verify the response.  
######1.1.3 Unknown
TODO: Describe the use case for an unsigned OCSP request for a single unknown certificate and what the desired response should look like.  
TODO: Describe the test procedure needed to verify the response.

#####1.2 Handle a Signed OCSP Request for a Single Certificate Using HTTP
######1.2.1 Good
TODO: Describe the use case for a signed OCSP request for a single good certificate and what the desired response should look like.  
TODO: Describe the test procedure needed to verify the response.

######1.2.2 Revoked
TODO: Describe the use case for a signed OCSP request for a single revoked certificate and what the desired response should look like.  
TODO: Describe the test procedure needed to verify the response.

######1.2.3 Unknown
TODO: Describe the use case for a signed OCSP request for a single unknown certificate and what the desired response should look like.  
TODO: Describe the test procedure needed to verify the response.

#####1.3 Handle an Unsigned OCSP Request for Multiple Certificates Using HTTP
######1.3.1 Good
TODO: Describe the use case for an unsigned OCSP request for good multiple certificates and what the desired response should look like.  
TODO: Describe the test procedure needed to verify the response.

######1.3.2 Revoked
TODO: Describe the use case for an unsigned OCSP request for revoked multiple certificates and what the desired response should look like.
TODO: Describe the test procedure needed to verify the response.
  
######1.3.3 Unknown
TODO: Describe the use case for an unsigned OCSP request for revoked multiple certificates and what the desired response should look like.   
TODO: Describe the test procedure needed to verify the response.

#####1.4 Handle a Signed OCSP Request for Multiple Certificates Using HTTP
######1.4.1 Good
TODO: Describe the use case for a signed OCSP request for multiple good certificates and what the desired response should look like.  
TODO: Describe the test procedure needed to verify the response.
######1.4.2 Revoked
TODO: Describe the use case for a signed OCSP request for multiple revoked certificates and what the desired response should look like.  
TODO: Describe the test procedure needed to verify the response.
######1.4.3 Unknown
TODO: Describe the use case for a signed OCSP request for multiple unknown certificates and what the desired response should look like.  
TODO: Describe the test procedure needed to verify the response.

#####1.5 Handle an Unsigned OCSP Request for a Single Certificate Using HTTPS (TLS)
######1.5.1 Good
######1.5.2 Revoked
######1.5.3 Unknown
TODO: Describe the use case for an unsigned OCSP request for a single certificate using TLS and what the desired response should look like.   
TODO: Describe the test procedure needed to verify the response.

#####1.6 Handle a Signed OCSP Request for a Single Certificate Using HTTPS (TLS)
######1.6.1 Good
######1.6.2 Revoked
######1.6.3 Unknown
TODO: Describe the use case for a signed OCSP request for a single certificate using TLS and what the desired response should look like.  
TODO: Describe the test procedure needed to verify the response.

#####1.7 Handle an Unsigned OCSP Request for Multiple Certificates Using HTTPS (TLS)
######1.7.1 Good
######1.7.2 Revoked
######1.7.3 Unknown
TODO: Describe the use case for an unsigned OCSP request for multiple certificates using TLS and what the desired response should look like.   
TODO: Describe the test procedure needed to verify the response.

#####1.8 Handle a Signed OCSP Request for Multiple Certificates Using HTTPS (TLS)
######1.8.1 Good
######1.8.2 Revoked
######1.8.3 Unknown
TODO: Describe the use case for a signed OCSP request for multiple certificates using TLS and what the desired response should look like.  
TODO: Describe the test procedure needed to verify the response.

#####1.9 Download CRL or Pre-signed Responses Using HTTP
TODO: Describe the use case for downloading CRL or pre-signed responses using HTTP.  
TODO: Describe the test procedure needed to verify the operation.

#####1.10 Download CRL or Pre-signed Responses Using LDAP
TODO: Describe the use case for downloading CRL or pre-signed responses using LDAP.  
TODO: Describe the test procedure needed to verify the operation.

