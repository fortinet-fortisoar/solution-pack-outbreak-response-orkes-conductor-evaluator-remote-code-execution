| [Home](../README.md) |
 | -------------------------------------------- |

# Contents

The **Outbreak Response - Orkes Conductor Evaluator Remote Code Execution** solution pack contains the following resources.

## Outbreak Alerts Record Set

| Name | Description |
|:-------------------------|:------------------|
| Orkes Conductor Evaluator Remote Code Execution | Attackers are actively targeting Orkes Conductor servers vulnerable to CVE-2026-58138, a critical unauthenticated remote code execution vulnerability in its GraalVM script evaluators. FortiGuard telemetry is observing active attack attempts targeting vulnerable Orkes Conductor deployments.

The vulnerability allows an unauthenticated attacker to submit a malicious workflow definition containing JavaScript or Python expressions to the Conductor workflow API. Because vulnerable evaluators can be configured with unrestricted host access, the attacker can escape the intended scripting environment and execute arbitrary operating system commands with the privileges of the Conductor process.

Public proof-of-concept exploit code is available, including a working exploit targeting Conductor v3.23.0. Exploit material has also been published through Exploit-DB, increasing the likelihood of opportunistic scanning and exploitation of exposed deployments. |

## Threat Hunt Rules Record set

| Name | Rule Type |
|:-------------------------|:------------------|
| FortiAnalyzer Threat Hunting - Orkes Conductor RCE Event-Handler | Fortinet Fabric |


 <table><th>NOTE</th><td>These SIGMA and Yara rules are sourced from public community repositories are not independently verified or validated by Fortinet. While community-contributed rules can be valuable for timely threat detection, they may vary in quality, accuracy, and relevance. Fortinet is not responsible for any inaccuracies, errors, or omissions in these rules, nor for any damage or loss that may result from their application. We encourage users to conduct their own validation and adapt these rules as necessary to meet specific security needs and contexts</td></table> 

# Next Steps
| [Installation](./setup.md#installation) | [Configuration](./setup.md#configuration) | [Usage](./usage.md) |
| ----------------------------------------- | ------------------------------------------- | --------------------- |