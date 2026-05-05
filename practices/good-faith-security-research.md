<!--
Originally published by NextJenSecurity, 2026.
Reproduced here as part of the disclose.io Framework practices reference.
Author retains rights; not CC0.
-->

# Accepted Practices for "Good-Faith Security Research"

*Originally published by NextJenSecurity, 2026.*

## TL;dr

Laws and policies that address the security of online systems should support research activities that are undertaken to benefit society by deterring the trespass of online systems and the theft or destruction of data. In reality, however, often this is not the case, and security researchers face enormous personal risk of criminal prosecution or civil litigation. Lawmakers, law enforcement, and systems operators face challenges distinguishing between beneficial, good faith security research and activities conducted with criminal intent, which can result in unwarranted claims being leveled against legitimate security research. This document is designed to help good faith security researchers to navigate this uncertainty and authentically defend their activities as a public good.

## The Legislative Landscape

Malicious cyber activity that extorts, defrauds, steals from, or otherwise intentionally harms victims must be prohibited to protect society. The annual cost of cybercrime on the global economy is estimated in the trillions of dollars, and extensive disruption to critical services such as healthcare, water treatment, education, and food provision has significant impact on safety and quality of life. These threats must be taken seriously and deterred as permitted by the law.

Part of defending against these threats is identifying opportunities for malicious actors and understanding the dynamics and dimensions of attacks. This can involve defenders and security researchers undertaking similar activities to those of malicious actors. Such activities serve a public good by identifying and mitigating the technical vulnerabilities and misconfigurations that create opportunities for malicious actors, as well as investigating and documenting the evolving techniques of attackers. While the goal of this legitimate security research is to reduce cyber risk for society, the economy, and national security, it can easily be mistaken as malicious.

Security research is critical for increasing the security and resilience of connected systems and mitigating damage or disruption of those systems, yet such research is often hindered by the complex legal landscape surrounding laws governing access to computer systems. So, a challenge lies in helping system owners and law enforcement differentiate between legitimate researchers and malicious actors where their core activities appear the same. How can governments support the work of legitimate researchers without also creating a potential defense for malicious actors? Can researchers adopt practices that will help distinguish between malicious cyber activities and research that is intended to be beneficial?

Importantly, some governments are acknowledging this challenge while also recognizing the importance and legitimacy of security research. In May 2022, the U.S. Department of Justice (DoJ) issued guidance to federal prosecutors that they, *"Should decline prosecution if available evidence shows the defendant's conduct consisted of, and the defendant intended, good-faith security research."*

The guidance described the characteristics of "good-faith security research" in terms similar to those previously defined and adopted in the Digital Millennium Copyright Act (DMCA) by the Register of Copyrights in [Section 1201 Rulemaking: Eighth Triennial Proceeding to Determine Exemptions to the Prohibition on Circumvention, at 258 (Oct. 2021)](https://cdn.loc.gov/copyright/1201/2021/2021_Section_1201_Registers_Recommendation.pdf). It states that:

> *"… "good faith security research" means accessing a computer solely for purposes of good-faith testing, investigation, and/or correction of a security flaw or vulnerability, where such activity is carried out in a manner designed to avoid any harm to individuals or the public, and where the information derived from the activity is used primarily to promote the security or safety of the class of devices, machines, or online services to which the accessed computer belongs, or those who use such devices, machines, or online services. Security research not conducted in good faith—for example, for the purpose of discovering security holes in devices, machines, or services in order to extort the owners of such devices, machines, or services—might be called "research," but is not in good faith."*

The DMCA is intended to protect copyright owners. Its exemption applies to security research conducted on devices owned by and in the possession of the researcher and conducted in non-production environments. These parameters are fairly clear-cut and easy for researchers, law enforcement, and copyright owners to apply.

By contrast, the US' [Computer Fraud and Abuse Act (CFAA - 18 U.S.C. § 1030)](https://www.law.cornell.edu/uscode/text/18/1030) addresses accessing computer systems "without authorization" or "exceeding authorized access" placing the activity firmly in murky waters. Under the CFAA, the sometimes nebulous line between authorized and unauthorized conduct, as well as the limitations of such authorization, are central to distinguishing between good faith research and malicious activity. Security researchers are better positioned to operationalize the DoJ guidance by clarifying within the researcher community how legitimate research is conducted.

The US is not the only government that has addressed this issue in recognition of the importance of security research. [Recital 75 of the European Union's Cyber Resilience Act (CRA - Regulation (EU) 2024/2847)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32024R2847#rct_75) urges EU Member States *"to address, to the extent possible, the challenges faced by vulnerability researchers, including their potential exposure to criminal liability, in accordance with national law."*

To date, four EU members - Belgium, Malta, The Netherlands, and Portugal have enacted legislation that codifies the importance of security research and creates protections or carve outs for the related activities, within specific boundaries. These countries are leading the way and we applaud them. More EU member states are currently reviewing their related laws and we hope to see more legislative reform to support security research in the future. If you know of other countries that have implemented legal protections or carve outs for security research, please let us know and we will update our list.

As with the US approach, these legal carve outs or protections typically include some parameters for "legitimate activity"; a way of determining that research is indeed conducted in good faith and not for more nefarious purposes. This document is written to broadly align with these parameters.

## Further Complications

As with any document addressing legal considerations, there are of course some caveats…

### Different Laws in Different Jurisdictions: Your Mileage May Vary

It is important to note that while government, law enforcement, and industry attitudes towards good faith security research may be maturing, they are doing so at an uneven rate and with varying outcomes in different jurisdictions. Given the cross-border nature of the internet, the extraterritorial application of some countries' laws, and the availability of technology products across different markets and jurisdictions, it may be necessary to familiarize yourself with legal considerations in multiple regions and proceed with caution.

### There's Nothing Civil about Civil Suits

Legal carve outs for security research in those jurisdictions that have them are most likely to address criminal enforcement actions, not civil ones. Many countries have legislation permitting civil lawsuits for unauthorized security research. For example, the DoJ charging guidance described in this document only relates to law enforcement action. It does not address civil actions under section 1030(g) of the CFAA, which states: *"(g) Any person who suffers damage or loss by reason of a violation of this section may maintain a civil action against the violator to obtain compensatory damages and injunctive relief or other equitable relief."*

Nonetheless, while this document primarily focuses on helping researchers meet a standard for protection from criminal prosecution, we hope that following the principles will also defend against civil claims against researchers. Above all, we recommend you document every stage of the research and disclosure process (including interaction with the vendor), and minimize the potential of research activities to cause disruptions or other harms.

### What is a Researcher?

One of the challenges policymakers face around this issue is that it can be hard to draw a clear box around the category of "Researcher". Formal paid security researcher roles can be hard to come by, and rarely follow a set mold or job description. Many people that regularly and intentionally conduct security research do so in their free time, and what they do with findings, and their expectations of rewards or outcomes will vary. Legislating to cover that is certainly a challenge.

Additionally, any research exemption should make provision for incidental or accidental discoverers – sometimes referred to simply as "technology users" – to disclose any valid findings. These users can spam a huge spectrum from professional system administrators to [five-year old gamers](https://www.bbc.co.uk/news/technology-26879185). Incidental/accidental discoverers cannot be expected to follow standard industry practices or be familiar with the law in this area. However, it is still to the benefit of society for the issue they discover to be disclosed to the technology supplier and users so it can be appropriately mitigated. Law enforcement and policymakers should recognize this need.

### In the AI of the Beholder

AI technologies are evolving rapidly and much has been made of their potential use for vulnerability discovery, verification, exploitation, and patching. The law is yet to catch up with this and it will take time. Regardless of what tooling you are using, the principles detailed in the document apply. Above all, take steps to minimize the risk of causing harm. Automating processes might be seen as being at odds with this goal, particularly if your automation tool of choice is still somewhat untested.

## Basic Security Research Principles

First and foremost, if you are conducting security research, we strongly recommend you familiarize yourself with any relevant anti-hacking and/or disclosure laws applying to the jurisdiction you are in, and that of the headquarters of the company that owns or makes the system/product you are testing. If you are researching security issues related to a regulated sector, there may also be sector-specific regulations of which to be aware.

### Conducting Vulnerability Discovery Research

- Activity should be designed to minimize the potential for harm, damage, disruption, or loss of confidentiality, availability, or integrity of company and/or user data. Where possible, test in non-production environments.
- Where possible, start by familiarizing yourself with any research policies of the technology manufacturer or operator. Some organizations may run bug bounty programs or have vulnerability disclosure policies with clear guidelines for research. Others may have processes for seeking permission to test their systems. You may also need to check licensing agreements. The existence (or lack) of a bug bounty program or permissive policy need not dictate your actions, but it can be a good indicator of how a vendor may respond to research or which systems may be considered more sensitive. This can help you plan how you want to proceed.
- Researchers should ensure they are adhering to data protection and privacy laws and standards as much as possible. Very minimal data should be accessed, copied, or exfiltrated - only the minimum required to investigate and confirm, demonstrate, and/or mitigate a security flaw or vulnerability.
- Functionality of the systems being researched, or any systems accessed through them, should not be disrupted, significantly altered, or directly result in downtime resulting in the interruption of the business processes. Changes or additions should not be made to code or any information accessed.
- Security research is not a defense for stealing information or money, nor for extorting technology manufacturers or users. Nor for exploiting access for any other nefarious activity, such as spying or planting crypto miners. Withholding findings unless payment is made (or even requesting payment before a vulnerability is mitigated) could appear extortionate. If you expect the vendor to pay for research, it is recommended that you stick to vendors that run public bug bounty programs or sign up to participate with private bounty programs. In these instances, you will need to operate within the parameters of those programs. There should be no expectation of other vendors to pay for security research.

### Conducting Internet-Wide Mass Port Scanning Research

Much of the guidance for conducting port scanning research will follow similar lines to those above. In addition, you may want to consider implementing the following:

- Do not conduct scanning that will or is highly likely to disrupt or impair the operation of a system, even temporarily.
- Provide a way for people to easily identify where the traffic is coming from and that it is not malicious. This could be a whois lookup that points to a webpage that explains the purpose of the research.
- A webpage describing the research may include how findings will be used; whether effort is made to specifically identify or conversely pseudonymize IP and domain owners; how long the research is expected to run and how long findings will be kept.
- Provide an easy way for IP address owners to opt out of participating, and honor such requests. If you plan to limit the time that the request will be honored - which is reasonable given the nature of IP address - it is advisable to state that upfront where you provide details on how to request an opt out.
- GDPR and other data protection regulations include elements around the right to be forgotten. You may want to provide a way for entities to request that their personally identifiable information (which may include their IP address) can be deleted.

### Conducting Threat or Forensic Research

This section covers research designed to quantify and/or assess the actual real-world impact of active exploitation of an identified vulnerability or abuse of a known weakness. Such research uses free/public services that gather information (ie VT, URL Scan, Censys, etc)

- Similar to vulnerability research, threat or forensic research should minimize the potential for harm, damage, or disruption to impacted companies and users.
    - In the case of forensic research, one stand out in this area exists around interacting with any artefacts left by an adversary. For example, interacting with a residual webshell could result in triggering unexpected functionality and unintended consequences, or alert the asset's creator/owner. This kind of research should be approached with considerable caution.
- As previously stated, researchers should ensure they are adhering to data protection and privacy laws and standards as much as possible. Information collected on potential victims should be limited and anonymized or pseudonymized as far as possible.
- Whenever it is feasible, researchers should inform any impacted companies or victims prior to sharing their information, even if you believe the information is adequately anonymized.
- Researchers should respect requests to remove any victim information from reporting.
- Third party technical assets are often leveraged in attacks and probing them to collect data could create privacy implications for their owners, who may themselves be victims of cybercrime.

### Research That Does Not Yield Findings

Sometimes research does not deliver results. In these situations it is advisable to still follow the guidance above, and to record/document your processes as thoroughly as possible. That way, if any of your actions trigger an investigation, you can show 1) the process you took; 2) the effort made to minimize harm; and 3) the rigor and discipline with which you approached the effort.

### Disclosing Findings (Reporting and Publishing)

#### Reporting Vulnerabilities to Technology Vendors

- Findings should be confidentially disclosed as soon as is practical after confirmation of the security issue. Where possible, communicate any vulnerabilities or associated details using the most secure method possible, for example exchanging PGP keys or through a secure portal.
- Researchers should conduct appropriate research to identify the technology manufacturer or vendor. Initial disclosure should not be made to user/customer organizations. In some cases, you may need to look for a parent company website to find a path for reporting.
    - Any efforts made to contact the vendor should be included in your record of activity to demonstrate good faith.
- Initial disclosure should be made confidentially either to the technology manufacturer or infrastructure owner, or their designated receiver if applicable, or a relevant government coordinating authority. If you are participating in a bug bounty, follow the guidelines provided by the program manager or vendor.
    - Not every country has a clearly defined government coordinating authority for research disclosures. However, [Article 12(1) of the European Union's NIS2 Directive](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:02022L2555-20221227&qid=1777567952824#enc_1) requires EU Member States to assign a designated Computer Security Incident Response Team (CSIRT) to facilitate the communication between a researcher disclosing a vulnerability and a manufacturer/provider.
- If additional disclosure is intended (e.g. if you intend to disclose to both the manufacturer and a government coordinating authority, and potentially any additional key stakeholders), a timeline for this disclosure should be provided to both/all parties.
- To ensure the vulnerability is triaged appropriately, reports must include all technical information and steps required to reproduce your findings. Withholding details at the request of payment could be construed at extortion.
- If you have a timeline in mind for public disclosure, that should also be provided during your initial disclosures. Otherwise, the timeline should be agreed through coordination with key stakeholders as far as reasonably possible, and prioritizing the security of users.
    - Consider what a realistic timeline for mitigation may be. Setting too short a timeline may seem like an intentional act of bad faith, while agreeing to too long a timeline may result in the vendor dragging their feet or taking evasive action. An appropriate timeline may also vary depending on the complexity of the problem and product, whether coordination with 3rd parties is required, and the reasonable availability of resources for mitigation (big companies likely have more resources than smaller ones!). These factors could be considered, as could standard practices for leading organizations, some of which we have linked to in the resources section of this document.
- Even if a vulnerability is not very severe, researchers should still consider notifying the vendor. It may not warrant public disclosure, but notifying the vendor gives them a chance to learn from the issue, and hopefully mitigate it in future releases.

#### Public Disclosure of Vulnerability Findings

- Wait a reasonable amount of time before publicly disclosing any security flaw or vulnerability derived from such activity, taking into consideration the following:
    - (I) the severity of the vulnerability,
    - (II) the difficulty of mitigating the vulnerability,
    - (III) whether all information is needed in the disclosure or details could be held back,
    - (IV) industry best practices, and
    - (IV) the willingness and ability of the owner of the protected computer to mitigate the vulnerability;
- If sensitive or confidential information was accessed during the research process, this should only be disclosed to the technology owner/operator or information owner/operator, unless it triggers a whistleblower response. Any confidential data accessed should be deleted following disclosure, and this process should be documented by the finder.
- Public disclosures of vulnerabilities should, where possible, be made in collaboration with the technology manufacturer or operator, and should provide pragmatic and realistic details on severity and mitigations in order to enable affected users to protect themselves.
- Additional information on the workings of the vulnerability will help the technology and security community learn from your findings and hopefully reduce the prevalence of such vulnerabilities in the future.
    - When providing this detail, consider how best to frame the information to minimize the potential for being accused of arming attackers, while still providing sufficient detail to aid defenders. This is a particularly challenging balance.
- Evidence of exploitation in the wild will likely accelerate the disclosure timeline. Where possible, this should still be coordinated with the manufacturer in order to reduce confusion and give those affected a clearer path to mitigation.
- Where vendors are resistant to disclosure or mitigating vulnerabilities, researchers should use their best judgment on when and how to disclose, prioritizing protecting users and minimizing security and safety risk in the manner and tone of disclosure. Working with a vulnerability coordination entity such as a CERT may help with this.

## Seeking Legal Assistance

Should you find yourself subject to legal proceedings resulting from good faith security research activities, we recommend you seek specialist legal counsel as soon as possible. There are some organizations that offer free legal support for qualifying researchers, detailed here. These offerings tend to be country-specific. If you know of free researcher legal services not included below, let us know and we'll add them.

- [The Electronic Frontier Foundation (EFF)](https://www.eff.org/pages/legal-assistance#main-content) - USA
- [Pwn.Legal](https://help.pwn.legal/) - United Kingdom

If you are unable to take advantage of free legal counsel and need assistance covering the costs of legal counsel for the defense of good faith security research, check out the [Security Research Legal Defense Fund (SRLDF)](https://srldf.org/).

## Additional Reading and Resources

### Vulnerability Disclosure and Handling Guidances and Policies

- [CERT/CC](https://vuls.cert.org/confluence/display/Wiki/Vulnerability+Disclosure+Policy)
- [European Union](https://www.enisa.europa.eu/publications/coordinated-vulnerability-disclosure-policies-in-the-eu)
- [ISO/IEC 29147](https://www.iso.org/standard/72311.html): Vulnerability disclosure requirements and recommendations for vendors
- [ISO/IEC 30111](https://www.iso.org/standard/69725.html): Vulnerability handling processes for vendors
- [JPCERT/CC](https://www.jpcert.or.jp/english/vh/vul-coordination-disclosure-policy_2019.pdf)
- [NCSC Netherlands](https://www.ncsc.nl/en/services/report-a-vulnerability)
- [Luta Security Vulnerability Coordination Maturity Model](https://www.lutasecurity.com/_files/ugd/a77f63_af8a64f8728e42ed8b79587c6e4a8057.pdf)
- [Project Zero](https://googleprojectzero.blogspot.com/2020/01/policy-and-disclosure-2020-edition.html)
- [Rapid7](https://www.rapid7.com/security/disclosure/)
- [U.S. Department of Homeland Security](https://www.dhs.gov/sites/default/files/2023-05/22_1222_vdp-policy-roe-approved.pdf)
- [ZDI](https://www.zerodayinitiative.com/advisories/disclosure_policy/)

### Discussions/Campaigns for Shifting Legal Parameters or Practices

- [EFF Coders' Rights Project](https://www.eff.org/issues/coders)
- [The Hacking Policy Council](https://www.centerforcybersecuritypolicy.org/hacking-policy-council)
- [UK CyberUp Campaign](https://www.cyberupcampaign.com/)
- [Where Are the Red Lines? Towards Ethical Server-Side Scans in Security and Privacy Research](https://swag.cispa.saarland/papers/hantke2024redlines.pdf), F. Hantke, S. Roth, R. Mrowczynski, C. Utz, B. Stock
- [The Conscience of a Hacker](https://phrack.org/issues/7/3) (AKA Hacker's Manifesto), The Mentor, 1986

## Legislative or public policy language for researcher protections

### Text from the [DOJ charging guidance](https://www.justice.gov/d9/press-releases/attachments/2022/05/19/cfaa_policy_may_19_0.pdf):

> "The attorney for the government should decline prosecution if available evidence shows the defendant's conduct consisted of, and the defendant intended, good-faith security research. For purposes of this policy, the attorney for the government should apply the definition of "good-faith security research" recommended by the [Register of Copyrights in Section 1201 Rulemaking: Eighth Triennial Proceeding to Determine Exemptions to the Prohibition on Circumvention, at 258 (Oct. 2021)](https://cdn.loc.gov/copyright/1201/2021/2021_Section_1201_Registers_Recommendation.pdf). That is: "good faith security research" means accessing a computer solely for purposes of good-faith testing, investigation, and/or correction of a security flaw or vulnerability, where such activity is carried out in a manner designed to avoid any harm to individuals or the public, and where the information derived from the activity is used primarily to promote the security or safety of the class of devices, machines, or online services to which the accessed computer belongs, or those who use such devices, machines, or online services. Security research not conducted in good faith—for example, for the purpose of discovering security holes in devices, machines, or services in order to extort the owners of such devices, machines, or services—might be called "research," but is not in good faith. CCIPS can consult with prosecutors about specific applications of this factor.

### Language developed by [Harley Geiger as a proposed amendment](https://www.rapid7.com/blog/post/2021/06/04/proposed-security-researcher-protection-under-cfaa-2/) for the CFAA, again, based on the language in the DMCA exemption:

The term "good faith security research" means good faith testing or investigation to detect one or more security flaws or vulnerabilities in software, hardware, or firmware of a protected computer for the purpose of promoting the security or safety of the software, hardware, or firmware.

(A) The person carrying out such activity shall

- (i) carry out such activity in a manner reasonably designed to minimize and avoid unnecessary damage or loss to property or persons;
- (ii) take reasonable steps, with regard to any information obtained without authorization, to minimize the information the person obtains, retains, and discloses to only that information which the person reasonably believes is directly necessary to test, investigate, or mitigate a security flaw or vulnerability;
- (iii) take reasonable steps to disclose any security vulnerability derived from such activity to the owner of the protected computer or the Cybersecurity and Infrastructure Security Agency prior to disclosure to any other party
- (iv) wait a reasonable amount of time before publicly disclosing any security flaw or vulnerability derived from such activity, taking into consideration the following:
    - (I) the severity of the vulnerability,
    - (II) the difficulty of mitigating the vulnerability,
    - (III) industry best practices, and
    - (IV) the willingness and ability of the owner of the protected computer to mitigate the vulnerability;
- (v) not publicly disclose information obtained without authorization that is
    - (I) a trade secret without the permission of the owner of the trade secret; or
    - (II) the personally identifiable information of another individual, without the permission of that individual; and
- (vi) does not use a nonpublic security flaw or vulnerability derived from such activity for any primarily commercial purpose prior to disclosing the flaw or vulnerability to the owner of the protected computer or the [government vulnerability coordination body].

(B) For purposes of subsection (A), it is not a public disclosure to disclose a vulnerability or other information derived from good faith security research to the [government vulnerability coordination body].

### Research carve-out language in [Washington State's anti hacking](https://app.leg.wa.gov/RCW/default.aspx?cite=9A.90&full=true) law (again, developed by Harley Geiger):

(11) "White hat security research" means accessing a data program, service, or system solely for purposes of good faith testing, investigation, identification, and/or correction of a security flaw or vulnerability, where such activity is carried out, and where the information derived from the activity is used, primarily to promote security or safety.

(12) "Without authorization" means to knowingly circumvent technological access barriers to a data system in order to obtain information without the express or implied permission of the owner, where such technological access measures are specifically designed to exclude or prevent unauthorized individuals from obtaining such information, but does not include white hat security research or circumventing a technological measure that does not effectively control access to a computer. The term "without the express or implied permission" does not include access in violation of a duty, agreement, or contractual obligation, such as an acceptable use policy or terms of service agreement, with an internet service provider, internet website, or employer. The term "circumvent technological access barriers" may include unauthorized elevation of privileges, such as allowing a normal user to execute code as administrator, or allowing a remote person without any privileges to run code.

### Relevant translated text from [Portugal's security research safe harbor](https://diariodarepublica.pt/dr/detalhe/decreto-lei/125-2025-962603401):

**Article 7**

Addition to Law 109/2009 of 15 September

Article 8-A is added to the Cybercrime Law, approved by Law 109/2009 of 15 September, in its current wording, with the following text:

**Article 8-A**

Acts not punishable due to public interest in cybersecurity

1 — Acts that could constitute the crimes of unlawful access and unlawful interception, as set out in articles 6 and 7 respectively, are not punishable if all of the following circumstances are cumulatively met:

> a) The individual acts with the sole intention of identifying vulnerabilities in an information system or in information and communication technology products or services, which were not created by them or by any third party on whom they depend, and with the purpose of contributing to cyberspace security through their disclosure.
>
> b) The individual does not act with the intention of obtaining an economic advantage or a promise of economic advantage arising from their action, without prejudice to any remuneration received as compensation for their professional activity.
>
> c) The individual immediately reports any vulnerabilities identified to the owner or to the person designated by the owner to manage the information system, product, or information and communication technology service, as well as to the holder of any data obtained that is protected under applicable personal data protection legislation, namely the General Data Protection Regulation (GDPR), approved by Regulation (EU) 2016/679 of the European Parliament and of the Council of 27 April 2016, Law 26/2016 of 22 August (as amended), Law 58/2019 of 8 August, and Law 59/2019 of 8 August.
>
> d) The individual's actions are proportionate to their purposes and strictly limited to them, consisting only of what is necessary to identify the vulnerabilities and not causing:
>
> > i) Any disruption or interruption of the system or service;
> >
> > ii) The deletion or deterioration of computer data or its unauthorized copying;
> >
> > iii) Any harmful or adverse effect on the person or entity affected, directly or indirectly, or on any third parties, excluding effects inherent to the unlawful access or unlawful interception itself, as defined in articles 6 and 7, as well as effects that would, with high probability, already result from the vulnerability detected or its exploitation.
>
> e) The individual's actions do not constitute a violation of personal data protected under applicable personal data protection legislation, namely Regulation (EU) 2016/679 of the European Parliament and of the Council of 27 April 2016, Law 58/2019 of 8 August, and Law 59/2019 of 8 August.

2 — The notification referred to in point c) above must also be made to the national cybersecurity authority, which shall forward it to the Polícia Judiciária whenever it may have criminal relevance.

3 — When assessing whether the individual acted proportionately, consideration must be given to whether the action was necessary to detect the vulnerability and whether the scope of systems or data accessed, viewed, and/or copied was strictly required by the aim of contributing to cyberspace security. The following practices are expressly prohibited:

> a) Denial of service (DoS) or distributed denial of service (DDoS) mechanisms;
>
> b) Social engineering, defined as deceiving system owners or users in order to obtain sensitive or confidential information;
>
> c) Phishing and its variants;
>
> d) Theft of passwords or other sensitive information;
>
> e) Intentional deletion or alteration of computer data;
>
> f) Intentional infliction of damage to the information system;
>
> g) Installation and distribution of malicious software.

4 — Without prejudice to the applicable data protection rules, any computer data communicated to the owner or person responsible for managing the information system, product, or ICT service, or to the national cybersecurity authority, must be deleted within 10 days from the moment the vulnerability is corrected, and its confidential nature must be ensured throughout the process.

5 — Acts performed with the consent of the owner or administrator of the information system, product, or ICT service are also not punishable, without prejudice to the obligation to notify the national coordinating authority responsible for responding to cybersecurity incidents of any vulnerabilities identified, in accordance with the legal framework on cybersecurity.
