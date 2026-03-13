This collection of GCP Logging queries is specifically engineered to detect "Session Anchoring"—the primary post-compromise tactic used by threat actors like Shiny Hunters (Scattered Spider/Lapsus clusters).

In 2026, attackers pivot from initial credential theft (via phishing or vishing) to creating permanent backdoors within Google Cloud. These queries provide high-fidelity detection for:

Service Account Weaponization: Identification of unauthorized .json key generation for high-privilege service accounts, bypassing standard password resets.

Shadow IAM Escalation: Real-time monitoring for the addition of "Owner" or "Security Admin" roles to unrecognized or external identities.

Cloud Shell Abuse: Flagging anomalous usage of the Google Cloud Shell terminal by non-technical identities—a common method for bypassing IP-based exfiltration controls.

Data Center Proxies: Specific filtering for known data center/VPS egress IPs (e.g., Dallas-based Hostwinds) performing reconnaissance via Get and List methods.
