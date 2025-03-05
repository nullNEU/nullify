---
title: "Advisory Alert 02-03-2025"
date: 2025-02-03T23:30:36Z
draft: false
summary: Details about a phishing attack against the Research & Development Team at nullNEU.
---

### Introduction

Emails are the channel through which business transactions and personal undertakings occur, an avenue that threat actors delightedly exploit. Verizon's 2024 Data Breach and Investigations Report details that 3,661 incidents were associated with social engineering, of which 3,032 had a confirmed data disclosure. Overall, 31% of the total incidents were categorized as Phishing, with email being the primary vector across observed incidents [(Verizon, 2024)](https://www.verizon.com/business/en-gb/resources/reports/2024/dbir/2024-dbir-data-breach-investigations-report.pdf?msockid=0b2436fa44d26e2e005b237d457a6fcf).

### Incident Details

Approximately three weeks ago, the Research & Development (R&D) team at nullNEU was targeted by an unknown party with the intention of obtaining $2,000 in funds from the club. This involved sending an initial email requesting discretion, through the impersonation of the Research Lead (Devesh Chande).

{{< figure src="/images/Blog%20Post%20-%20First%20Email.PNG" alt="First email received on Fri, 10 Jan 2025 17:22:46 UTC" width="350" height="700" >}}

Email header analysis disclosed the 'From' and 'Return-Path' to be 'officecontactmail0@internet[.]ru', indicating the utility of the zero-cost email service provider Mail[.]ru, provided by VK [(LSE: VKCO)](https://finance.yahoo.com/quote/VKCO.ME/), a leading Russian technology company. The content of the email body provides two insights: (i) the Development Lead (Parthiv Menon) was the sole target and (ii) the Research Lead (Devesh Chande) was impersonated.

The domain 'internet[.]ru' is a valid, serviceable domain used by Mail[.]ru, resulting in successful authentication checks involving Sender Policy Framework (SPF), DomainKeys Identified Mail (DKIM), and Domain-based Message Authentication Reporting and Conformance (DMARC).

A subsequent reply was sent to the impersonator, resulting in the following email being delivered:

{{< figure src="/images/Blog%20Post%20-%20Second%20Email.PNG" alt="Second email received on Fri, 10 Jan 2025 22:11:19 UTC" width="350" height="700" >}}

At this point, out-of-band (OOB) communication was initiated to validate this activity, after which it was determined that this was a targeted phishing attack. No resources / assets belonging to the club or associated parties has been compromised, although we will continue to monitor the situation and provide updates as necessary.

Based on our internal investigation, we assess with medium confidence that the public nature (Search Open Websites/Domains - T1593) of our projects enabled the unknown party to map relationships (Gather Victim Org Information - T1591) at the club that potentially have access to funding and determine personal accounts associated with the team (Search Victim-Owned Websites - T1594). As a side note, we do not see indicators of the message being crafted using Artificial Intelligence (AI) language models. At the time of this publication, we are unaware of any additional factors that contributed towards the impersonation and targeting of the aforementioned members. Historically, The University of Freiburg [has reported](https://www.rz.uni-freiburg.de/en/rz-en/news-alerts/aktuell-en/2024-03-14-16-25-phishing-scam-fraudulent-emails-from-20-12-internet.ru) a similar phishing campaign in early 2024, in addition to the [University System of New Hampshire](https://www.usnh.edu/it/blog/2021/02/phishing-email-subject-can-you-handle-me) in early 2021.

To improve security efforts, the club has enacted the following changes:

- Our policy now dictates that all internal communication be held through official Northeastern accounts alone.
- External communication involving third-parties must be confirmed using an out-of-band communication platform that is open-source and end-to-end encrypted.

Additionally, the club has reported the incident to [Google](https://support.google.com/mail/answer/8253?hl=en) and the [Federal Trade Commission](https://reportfraud.ftc.gov/).

As a final note, no member of nullNEU will ever solicit offers requesting the exchange of gift cards - or any form of monetary asset. We are strictly a volunteer-based organization that believe cybersecurity is for everyone.

### [MITRE ATT&CK Enterprise](https://attack.mitre.org/matrices/enterprise/) Techniques:

- Gather Victim Org Information: Business Relationships (T1591.002)
- Gather Victim Org Information: Identify Business Tempo (T1591.003)
- Gather Victim Org Information: Identify Roles (T1591.004)
- Establish Accounts: Email Accounts (T1585.002)
- Search Victim-Owned Websites (T1594)
- Gather Victim Identity Information: Email Addresses (T1589.002)
- Search Open Websites/Domains: Social Media (T1593.001)
- Search Open Websites/Domains: Search Engines (T1593.002)
- Search Open Websites/Domains: Code Repositories (T1593.003)

### Technical Artifacts

- Email Address: officecontactmail0@internet[.]ru
