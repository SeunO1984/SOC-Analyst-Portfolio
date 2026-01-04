## Incident Summary
A user mailbox was reviewed following concern that it may have been targeted by a phishing attempt. The purpose of the review was to confirm that no mailbox changes had been made that could allow an attacker to stay hidden or continue accessing email content after the initial message was dealt with.

## Detection / Reason for Review
Phishing attacks sometimes involve more than just a single email. If a user interacts with a message, attackers may create inbox rules, enable forwarding, or modify permissions to maintain access. This review was triggered to confirm that no such persistence methods were present.

## Scope of Investigation
The investigation focused on mailbox-level settings that are commonly abused after phishing activity. This included inbox rules, automatic forwarding settings, and mailbox permissions. Only areas visible through Microsoft 365 and Exchange administrative views were reviewed.

## Mailbox Rule Review
Inbox rules were checked to identify any rules that could automatically delete, move, or hide incoming messages. Particular attention was given to rules targeting security notifications, replies, or messages from external senders. No suspicious or unexpected rules were identified during the review.

## Mailbox Forwarding Review
Mailbox forwarding settings were reviewed to confirm that emails were not being automatically sent to another internal or external address. Forwarding was not enabled in a way that would allow email data to be exfiltrated from the mailbox.

## Mailbox Permission Review
Mailbox permissions were reviewed to confirm that no additional users or service accounts had been granted access. This included full access, send-as, and send-on-behalf permissions. No unexpected or unauthorised access was identified.

## Correlation and Validation
The findings across rules, forwarding, and permissions were reviewed together to ensure there were no indicators of persistence. The absence of changes across multiple mailbox settings supported the conclusion that no post-phish persistence had been established.

## Findings
The review did not identify any malicious inbox rules, forwarding configurations, or mailbox permissions. There were no indicators suggesting that the mailbox had been modified to maintain unauthorised access.

## Response and Outcome
No remediation actions were required as the mailbox configuration appeared clean. The mailbox was assessed as low risk based on the results of the investigation, with continued monitoring recommended.

## Incident Closure
The incident was closed after confirming there were no signs of mailbox persistence or ongoing risk. No further actions were required beyond standard security monitoring.

## Lessons Learned
Mailbox persistence checks are an effective follow-up after phishing-related incidents. Reviewing rules, forwarding, and permissions can quickly confirm whether an attacker attempted to maintain access beyond the initial email.

## Evidence Collected (Screenshots)
