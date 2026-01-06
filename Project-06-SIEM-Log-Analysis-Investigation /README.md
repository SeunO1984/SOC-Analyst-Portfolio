## Incident Summary
A security event was reviewed to investigate suspicious sign-in activity using log data. The aim of the investigation was to understand what caused the alert and determine whether the activity suggested unauthorised access or normal user behaviour.
## Detection / Alert Trigger
The investigation was triggered after authentication logs showed unusual sign-in behaviour. This included multiple failed login attempts followed by a successful sign-in, which can sometimes indicate password guessing or compromised credentials and therefore required further review.
## Scope of Investigation
The investigation focused solely on authentication and sign-in related log data. The review was limited to information visible within the SIEM, including sign-in attempts, success and failure results, timestamps, IP addresses, and location details. No endpoint, email, or mailbox data was included.
## Log Source Overview
The analysis used sign-in logs commonly ingested into a SIEM. These logs provided visibility into login attempts, authentication outcomes, source IP addresses, locations, and event timing. This data was used to build context around the alert and understand the user’s sign-in behaviour.
## Initial Log Review
Sign-in logs were reviewed to identify patterns such as repeated failed authentication attempts, successful sign-ins shortly after failures, access outside normal hours, or sign-ins from unfamiliar locations. Particular attention was given to whether the activity could indicate credential misuse rather than user error.
## SIEM Analysis and Correlation
Multiple log fields were reviewed together to better understand the activity. This included correlating timestamps, IP addresses, locations, authentication methods, and sign-in outcomes across events. Reviewing these details together helped determine whether the activity was isolated or potentially suspicious.
## Investigation Findings
The log review identified activity that justified investigation, but there was not enough evidence to confirm unauthorised access. The successful sign-in appeared consistent with the user’s normal behaviour, and no additional suspicious events were identified during the review period.
## Analyst Decision and Outcome
Based on the findings, no immediate response actions were required. The activity was assessed as low concern, and continued monitoring was recommended rather than escalation.
## Incident Closure
The incident was closed after completing log review and correlation. No further action was required, with monitoring in place to detect any similar behaviour in the future.
## Lessons Learned
Sign-in patterns involving repeated failures followed by a successful login should always be reviewed. Correlating multiple log fields helps distinguish between normal user behaviour and potential security issues, reducing unnecessary escalation while maintaining visibility of risk.
## Evidence Collected (Screenshots)
