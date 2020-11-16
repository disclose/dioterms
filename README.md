# The disclose.io Terms

> Note: While we've engaged the legal opinion of many, this does not constitute legal advice. Please consult your legal counsel for the specific suitability of the disclose.io terms in your organization.)

## Navigating the dioterms Repo
- Core terms: The core terms are the primary documents in the repo. The language in these terms is designed to provide maximum flexibility whilst maintaining bi-lateral safety and readability, and accomodating varying legal environments for both the finder and the vendor. Note that while the [bug bounty terms](core-terms-bbp.md) are a subset of the [vulnerability disclosure policy VDP terms](/core-terms-vdp.md) with additional fields regarding rewards and scope, we've chosen to seperate them to avoid ambiguity between a VDP and a bug bounty.
  - [Core modules](/core-modules/): The core modules are derived from the Core terms, which are the basis for language and regional legal translation. 
-  [Regionalized terms](regional): The regionalized terms have been contributed by PSIRTS, disclosure platforms, security policy advocates, and vendor program operators.
-  [Archive](/archive): This folder contains deprecated or archived terms for posterity and easy reference.

## Choosing terms 
Organizations should first choose the boilerplate that is the best fit to their organization. The dioterms repo contains a number of different options:

* Core terms for [VDP](/core-terms-vdp.md) and [BBP](core-terms-bbp.md) designed to provide maximum flexibility whilst maintaining bi-lateral safety and readability,
* [Regionalized terms](https://github.com/disclose/dioterms/tree/master/regional) which accommodate the laws and languages of country or jurisdiction of the organization,
* [Verticalized terms](https://github.com/disclose/dioterms/tree/master/vertical) which take the nuances of different industries or use-cases (e.g. election infrastructure) into account, and
* [Simple Safe Harbor](https://github.com/disclose/dioterms/tree/simple-safeharbor/simple-safe-harbor.md) which is designed to add Safe Harbor language to VDPs and bug bounty programs which are already in place.

### About Safe Harbor

The core requirements for disclose.io's definition of **Full Safe Harbor** are for the policy to provide:
- Authorization against anti-hacking laws
- Exemption from anti-circumvention laws 
- Exemption from violation of the TOS/AUP during security testing
- A statement acknowledging good-faith.

The intention of Safe Harbor language provided by disclose.io is for it to be followed specifically, with minor, if any, modifications. If modifications are made, the four tenets laid out above are the most important to address in your policy.

Policies missing any of the core tenets above, but that still contain a good-faith statement committing not to pursue legal action on security researchers, meet the criteria for **Partial Safe Harbor**.

### Disclosure types

- **Coordinated Disclosure**: A researcher can share details of the vulnerability after a fix has been applied and the program owner has provided permission to disclose or after a clearly-stated time has passed from submission, whichever is sooner;
- **Discretionary Disclosure**: The researcher or the program owner can request mutual permission to share details of the vulnerability after approval is explicitly received; or
- **Non-Disclosure**: Researchers are required to keep vulnerability details and the existence of the program itself confidential, regardless of the fix or any conversations between them and the vendor. Note that non-disclosure is considered inappropriate and generally ineffective as a disclosure type for VDPs.

### Disclose.io dioseal Status
Disclose.io maintains four levels of best-practice attainment:
- **Basic**: A publicly available Policy and Official Channel exist.
- **Partial**: Basic, with the addition of **Partial Safe Harbor** provisions.
- **Full**: Basic, with the addition of **Full Safe Harbor** provisions.
- **Full with CVD**: Full, with the addition of a **Coordinated Disclosure Policy** that includes a proactive disclosure timeline.

### Additional terms

In each template we've also provided boilerplate examples for the additional section.  
- **Scope** (Required) – A complete list of "In-Scope" properties for which the organization is explicitly allowing and encouraging good-faith security research. Keep in mind that a true vulnerability disclosure program considers the entire attack surface of the organization running the program, so erring on the side of inclusiveness is best practice with respect to scope.
- **Out-of-Scope** (Optional) - A non-exhaustive list of systems and security testing activities that the organization strongly wishes to discourage testing against, and
- **Rewards** (Optional) – Information on whether or not the program offers payment for valid, unique issues, as well as the type and parameters of that compensation.
- **Official Communication Channels** (Required) – A full list of the communication methods that are made available by the organization to receive and communicate about vulnerability submissions.
- **Disclosure Policy** (Required) – A clear policy outlining the conditions under which a researcher can disclose the details of a reported issue to third parties. 

## Next steps 

Once you've published your policy, you can:  
- Add the appropriate [disclose.io seal](https://github.com/disclose/dioseal) to your public program brief,
- Submit a pull request to add your program to the [open-source disclose.io program list](https://github.com/disclose/diodb),
- Let the world know you're joining the initiative!
- Contribute back to the [disclose.io](https://disclose.io) project! 

## License

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">disclose</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://disclose.io" property="cc:attributionName" rel="cc:attributionURL">disclose.io</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.
