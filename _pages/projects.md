---
layout: page
permalink: /projects/
title: Projects
---

<h1 align="center">[Bruno Collections for CyberArk Identity Security REST API](https://github.com/IAM-Jah/CyberArk-REST-API-Bruno/tree/main)</h1>

<table>
<tr>
<td>
  
Bruno Collection and Environment files for **CyberArk Identity Security** REST API testing and automation. 945 REST API requests are included in the Collections, which cover Self-Hosted PAM, Privilege Cloud - Standard, Privilege Cloud on Identity Security Platform for Shared Services (ISPSS/Shared Services), and many shared services from the SaaS platform.

Each API request includes small optimizations to help get you up and running quickly, for example:
  * Authentication requests test for and store the resulting tokens as Environment variables.
  * Authentication token is automatically populated to request headers where necessary.
  * Documentation links and important notes are stored inside each request's 'Docs' section.
  * Mandatory URI parameters are selected by default and vice-versa.
  * Central Credential Provider 'GetPassword' request included with every Collection.

![Bruno Collection OIDC Authentication](https://github.com/IAM-Jah/CyberArk-REST-API-Bruno/blob/main/assets/brunoCollectionOIDCAuth.png)

</td>
</tr>
</table>

## Installation

##### To import from JSON (Easiest method):
1. Download the latest version of both the 'Environment' and 'Collection' JSON files that correspond to your environment:
  * Privilege Cloud and/or Shared Services:
    * [Collection](https://github.com/IAM-Jah/CyberArk-REST-API-Bruno/blob/main/Privilege%20Cloud%20and%20Shared%20Services%20REST%20API/Privilege%20Cloud%20and%20Shared%20Services%20REST%20API.json)
    * [Environment](https://github.com/IAM-Jah/CyberArk-REST-API-Bruno/blob/main/Privilege%20Cloud%20and%20Shared%20Services%20REST%20API/Privilege%20Cloud%20Shared%20Services%20Environment.json)

  * Self-Hosted PAM:
    * [Collection](https://github.com/IAM-Jah/CyberArk-REST-API-Bruno/blob/main/CyberArk%20Self-Hosted%20REST%20API/CyberArk%20Self-Hosted%20REST%20API.json)
    * [Environment](https://github.com/IAM-Jah/CyberArk-REST-API-Bruno/blob/main/CyberArk%20Self-Hosted%20REST%20API/Self-Hosted%20Environment.json)
2.  From the Bruno start page, click 'Import Collection' > 'Bruno Collection' and select the Collection JSON file.

> [!IMPORTANT]  
> You must use Bruno v1.19 or later to import JSON files.

3.  Once the Collection is imported, expand the Collection tree down and select any API request. Press 'ctrl'+'e' on the request page to open the Environments menu.

4. Click 'Import' in the lower left then select the Environment JSON file to use with the Collection.

##### To import Bruno Collection natively (Advanced):
1.  Uploading native .bru project files is on the roadmap.

## Collections

#### CyberArk Privilege Cloud and Shared Services REST API:
  This Collection is meant to help CyberArk Privilege Cloud and CyberArk Identity administrators manage and explore the CyberArk Shared Services/SaaS environment with REST API. For ease of use, the Environment JSON file is alphabetized and includes only relevant environment variables. All default services that are part of the Shared Services platform are included:

  * CyberArk Privilege Cloud - Standard
  * CyberArk Privilege Cloud - Shared Services
  * CyberArk Identity - Shared Services
  * Connector Management
  * Dynamic Privileged Access (DPA)
  * Secure Cloud Access (SCA)
  * Remote Access V2
  * EPM SaaS (for EPM LCD)
  * Secrets Hub
  * Central Credential Provider (CCP)
  * Conjur Cloud

  Current up to Privilege Cloud v14.2 (August 2024)

#### CyberArk Self-Hosted REST API:
  This Collection is meant to help self-hosted CyberArk PAM administrators manage and explore the PAM environment with REST API. For ease of use, the Environment JSON file is alphabetized and includes only relevant environment variables. The following services are included:

  * Self-Hosted PAM
  * Central Credential Provider (CCP)
  * Remote Access V2
  * EPM On-Prem

  Current up to Password Vault Web Access (PVWA) v14.2 (Aug 2024) and EPM On-Prem v11.5.6 (Feb 2023/final version).

## Roadmap

- [x] Add Privilege Cloud Collections (28 Jul 2024)
- [x] Add Self-Hosted PAM Collection (4 Aug 2024)
- [x] Add Identity and Shared Services to SaaS Collection: (18 Aug 2024)
    - [x] Identity on Shared Services (28 Jul 2024)
    - [x] Secure Infrastructure Access (10 Aug 2024)
    - [x] Connector Management (10 Aug 2024)
    - [x] Remote Access (10 Aug 2024)
    - [x] Endpoint Privilege Manager (For LCD) (10 Aug 2024)
    - [x] Secure Cloud Access (17 Aug 2024)
    - [x] Identity - Workforce Password Management (17 Aug 2024)
    - [x] Identity - SCIM (17 Aug 2024)
    - [x] Secrets Hub (17 Aug 2024)
    - [x] Conjur Cloud (18 Aug 2024)
- [x] Add additional services to Self-Hosted Collection: (30 Aug 2024)
    - [x] Remote Access (30 Aug 2024)
    - [x] Endpoint Privilege Manager (30 Aug 2024)
- [x] Add usage guide (14 Oct 2024)
- [ ] Upload native .bru project files
- [ ] UX enhancements:
    - [ ] Expand documentation
    - [ ] Improve examples for params
    - [ ] Improve examples for bodies
    - [ ] Expand tests and scripts

## Contact

Maintained by Eli Hopkins, [@IAM-Jah](https://github.com/IAM-Jah). Contact information is located in my profile.

## Acknowledgements

This project would not have been possible without the wealth of knowledge made available by Joe Garcia, [@infamousjoeg](https://github.com/infamousjoeg), and others at CyberArk Software.

## License

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

# [CyberArk Program Acceptance Toolkit](https://github.com/IAM-Jah/CyberArk-Program-Acceptance-Toolkit)

Welcome to the CyberArk Program Acceptance Toolkit! This repository offers a comprehensive collection of resources designed to assist CyberArk Administrators and Program Managers in promoting user adoption and engagement.

## Read the article for background!

This repository is a supporting resource to my article titled ["Winning Hearts and Minds: Driving User Acceptance in PAM Programs"](https://www.linkedin.com/pulse/winning-hearts-minds-driving-user-acceptance-pam-hopkins-cissp-qipic). For context on why certain materials were included, or how to utilize them in your own PAM program, go read the article and reach out if you still have questions.

## Repository Structure

The repository is organized into the following directories:

- **Automation**: Scripts and tools to automate various CyberArk tasks.
- **Compliance**: Guidelines and documents to ensure adherence to compliance standards.
- **Configuration**: Best practices and templates for configuring CyberArk environments.
- **Diagrams**: Visual representations and architecture diagrams of CyberArk deployments.
- **Email Templates**: Pre-crafted email templates to facilitate communication with stakeholders.
- **Planning**: Resources to aid in the planning and implementation of CyberArk projects.
- **Videos**: Instructional videos and tutorials for better understanding and training.

## Getting Started

To get started with the resources in this repository:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/IAM-Jah/CyberArk-Program-Acceptance-Toolkit.git

2. **Explore the Directories**: Navigate through the directories to find the resources pertinent to your needs. Each directory contains a README.md file with detailed information about its contents.

## Contributions

Contributions to enhance and expand the toolkit are welcome. If you have suggestions or resources to add:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/YourFeatureName
3. Make your changes: Add your contributions and commit your changes with clear and descriptive messages.
4. Push to your fork:
   ```bash
   git push origin feature/YourFeatureName
5. Submit a pull request.

## Contact

Maintained by Eli Hopkins, [@IAM-Jah](https://github.com/IAM-Jah). Contact information is located in my profile.

## Acknowledgements

Thank you for utilizing the CyberArk Program Acceptance Toolkit. I hope these resources prove valuable in your efforts to drive user adoption and engagement within your CyberArk programs.

## License

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Disclaimer

This repository is for informational purposes and does not constitute legal advice. Ensure to consult with compliance and legal professionals for specific guidance. This is an unofficial repository and is not affiliated with CyberArk Software, Ltd.

---