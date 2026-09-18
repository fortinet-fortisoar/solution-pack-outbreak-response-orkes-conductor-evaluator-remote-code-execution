# Release Information 

- **Version**: 1.0.0 
- **Certified**: No 
- **Publisher**: Fortinet 
- **Compatible Version**: FortiSOAR 7.4.0 and later 

# Overview 

Attackers are actively targeting Orkes Conductor servers vulnerable to CVE-2026-58138, a critical unauthenticated remote code execution vulnerability in its GraalVM script evaluators. FortiGuard telemetry is observing active attack attempts targeting vulnerable Orkes Conductor deployments.

The vulnerability allows an unauthenticated attacker to submit a malicious workflow definition containing JavaScript or Python expressions to the Conductor workflow API. Because vulnerable evaluators can be configured with unrestricted host access, the attacker can escape the intended scripting environment and execute arbitrary operating system commands with the privileges of the Conductor process.

Public proof-of-concept exploit code is available, including a working exploit targeting Conductor v3.23.0. Exploit material has also been published through Exploit-DB, increasing the likelihood of opportunistic scanning and exploitation of exposed deployments. 

 The **Outbreak Response - Orkes Conductor Evaluator Remote Code Execution** solution pack works with the Threat Hunt rules in [Outbreak Response Framework](https://github.com/fortinet-fortisoar/solution-pack-outbreak-response-framework/blob/release/2.3.0/docs/background-information.md#threat-hunt-rules) solution pack to conduct hunts that identify and help investigate potential Indicators of Compromise (IOCs) associated with this vulnerability within operational environments of *FortiSIEM*, *FortiAnalyzer*.

 The [FortiGuard Outbreak Page](https://www.fortiguard.com/outbreak-alert/orkes-conductor-rce) contains information about the outbreak alert **Outbreak Response - Orkes Conductor Evaluator Remote Code Execution**. 

## Background: 

Organizations using affected versions should upgrade to Conductor 3.30.2 or later, which addresses the vulnerability. 

## Announced: 

Because the vulnerability is unauthenticated and remotely exploitable, Internet-exposed instances should be treated as a high priority for remediation. 

## Latest Developments: 

September 9, 2026: FortiGuard released a Threat Signal Report.
https://www.fortiguard.com/threat-signal-report/6527/orkes-conductor-evaluator-remote-code-execution

August 9, 2026: Exploit-DB publication. A public unauthenticated RCE exploit for CVE-2026-58138 was published as EDB-52633, increasing the availability of weaponized exploit material.
https://www.exploit-db.com/exploits/52633 

# Next Steps
 | [Installation](./docs/setup.md#installation) | [Configuration](./docs/setup.md#configuration) | [Usage](./docs/usage.md) | [Contents](./docs/contents.md) | 
 |--------------------------------------------|----------------------------------------------|------------------------|------------------------------|
