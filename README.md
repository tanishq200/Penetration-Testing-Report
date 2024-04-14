# Penetration Testing Report
### Group 6 - Coreprotectors

## Overview

This document outlines the comprehensive security assessment conducted by Coreprotectors for MaskedDJ in preparation for their high-profile 'unmasked' event. The primary objective was to test the security measures in place by attempting to access an early version of the MaskedDJ website and, by extension, identify potential security vulnerabilities.

## Objectives

- **Security Assessment**: To evaluate the security posture of MaskedDJ's network and digital infrastructure.
- **Identity Revelation**: To determine if it was possible to reveal the identity of MaskedDJ before its official disclosure through digital means.

## Methodology

The penetration test followed a structured approach, including:

1. **Port Scanning**: Identification of open ports and services across all networked machines.
2. **Enumeration and Vulnerability Scanning**: Detailed scanning of individual systems to identify security weaknesses.
3. **Exploitation**: Leveraging found vulnerabilities to gain unauthorized access.
4. **Post-Exploitation**: Assessing the level of access obtained and further exploiting the network to uncover additional vulnerabilities and access sensitive data.

## Key Findings

- **Successful Compromise**: The booking manager’s computer was compromised, providing a pivot point to further access the Windows Server and IT admin PCs.
- **Critical Misconfigurations**: Several critical misconfigurations were identified, including outdated software and improper security settings that facilitated network penetration.
- **Sensitive Data Access**: Access was gained to the development web server where sensitive information was stored.

## Recommendations

Immediate actions recommended include:
- **System Updates**: Upgrading all outdated and unsupported operating systems, especially Windows 7.
- **Patching**: Regularly updating systems with the latest security patches.
- **Stronger Password Policies**: Enforcing robust password policies to prevent easy brute-force attacks.
- **Encryption and Hashing**: Implementing advanced encryption for sensitive data and updating hashing algorithms to secure password storage.
- **Multi-Factor Authentication**: Introducing MFA to add a layer of security against compromised credentials.

## Tools Used

- **Nmap**: For port scanning and service identification.
- **Metasploit**: For exploiting known vulnerabilities like EternalBlue.
- **Hashcat**: For cracking password hashes.
- **Impacket**: For extracting and utilizing credentials.

## Conclusion

The penetration test successfully demonstrated several security flaws within MaskedDJ's network, which could potentially be exploited by malicious actors to compromise system integrity and confidentiality. It is imperative that MaskedDJ addresses these vulnerabilities promptly to safeguard against real-world attacks.
