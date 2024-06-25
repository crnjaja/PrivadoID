<a name="readme-top"></a>
<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#general">General</a>
      <ul>
        <li><a href="#blockchain">Blockchain</a></li>
        <li><a href="#token">Token</a></li>
        <li><a href="#smart-contracts">Smart contracts</a></li>
        <li><a href="#zero-knowledge-proof">Zero knowledge proof</a></li>
        <li><a href="#identity-models">Identity models</a></li>
        <li><a href="#know-your-customer">Know Your Customer</a></li>
        <li><a href="#airdrop">Airdrop</a></li>
        <li><a href="#dapps">dApps</a></li>
      </ul>
    </li> 
    <li>
      <a href="#ssi-technology">SSI Technology</a>
      <ul>
        <li><a href="#decentralized-identifiers">Decentralized Identifiers</a></li>
        <li><a href="#virtual-credentials">Virtual credentials</a></li>
        <li><a href="#digital-wallet">Digital wallet</a></li>
        <li><a href="#digital-agent">Digital agent</a></li>
        <li><a href="#governance-framework">Governance framework</a></li>
        <li><a href="#decentralized-key-management">Decentralized key management</a></li>
        <li><a href="#cryptography-techniques">Cryptography techniques</a></li>
      </ul>
    </li> 
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>



### General

Edit the intro here


<!-- BLOCKCHAIN -->
## Blockchain

check if needed

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- TOKENIZATION -->
## Token

check if needed

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- SMART CONTRACTS -->
## Smart Contracts

Smart contracts are simple programs that run on blockchain platforms, such as Ethereum. They are designed to execute specific actions automatically when predefined conditions are met. These contracts run in virtual machines, like the Ethereum Virtual Machine (EVM) or Ethereum Flavored WebAssembly (eWASM), ensuring that they are secure and tamper-proof.

Key Features of Smart Contracts :
- Autonomous Execution: Once deployed, smart contracts operate autonomously. They do not require human intervention to execute their instructions.
- Cost and Efficiency: Running smart contracts involves transaction fees, paid in the blockchain's native cryptocurrency (e.g., Ether on Ethereum). The fees, calculated in units called gas, ensure that the network remains sustainable and efficient.
- Interoperability: Smart contracts can interact with each other, enabling complex chains of actions and logic. This interoperability supports various applications, from simple wallets to sophisticated identity systems.
- Ownership and Control: Smart contracts can be owned by individuals, groups, or be entirely autonomous. The ownership model influences how the contract can be interacted with and controlled.
- Transparency and Security: The operations of smart contracts are transparent and verifiable by anyone on the network. This transparency enhances security and trust among participants.

Smart contracts play a pivotal role in decentralized identity systems. For example, ERC 725 v2 and ERC 1056 are specific types of smart contracts designed to support identity management on the Ethereum blockchain.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ZKP -->
## Zero Knowledge Proof

Zero-Knowledge Proofs are a type of cryptographic protocol that allows one party (the prover) to convince another party (the verifier) that they know a value or possess certain information without disclosing any details about the value itself.

ZKP needs to have the following three properties :
- Completeness, if the statement is really true and both users follow the rules properly, then the verifier would be convinced without any artificial help.
- Soundness, in case of the statement being false, the verifier would not be convincedin any scenario.
- Zero-Knowledge, the verifier in every case would not know any more information.

Cryptographic Mechanisms
- Interactive Proof Systems: Early ZKPs were interactive, requiring multiple rounds of communication between the prover and verifier.
- Non-Interactive Zero-Knowledge Proofs (NIZK): These allow the proof to be generated and verified without interaction, often using a common reference string available to both parties.

Practical Implementations
- zk-SNARKs - Zero-Knowledge Succinct Non-Interactive Arguments of Knowledge: Used in blockchain technologies like Zcash for private transactions. They are efficient and allow for succinct proofs.
- zk-STARKs - Zero-Knowledge Scalable Transparent Arguments of Knowledge: Designed for scalability and transparency, eliminating the need for a trusted setup phase.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- IDENTITY MODELS -->
## Identity Models

 ### Centralized Identity Model
The centralized identity model is a traditional approach where a single, central authority manages and controls identity information. This model is prevalent in systems where government agencies, social media platforms, or service providers issue and maintain identification data. In this setup, individuals create accounts with the central entity, linking their identity to these accounts. The central authority owns and controls the identity data, making decisions about its use and access. This model is characterized by a single point of control, where the central entity oversees the creation, update, and deletion of identity records.

One of the significant issues with this model is privacy. Users have limited control over their personal data, and the central authority can use or share this data without the user's explicit consent. Additionally, centralized databases are attractive targets for cyberattacks, leading to potential data breaches and identity theft. Despite these risks, the centralized model remains widely used due to its simplicity and historical precedence.

### Federated Identity Model
The federated identity model aims to address some of the limitations of the centralized model by allowing multiple organizations to share and verify identity information through a trusted third party known as an Identity Provider (IDP). This model enables Single Sign-On (SSO) capabilities, where users can access multiple services using one set of login credentials managed by the IDP.

In a federated system, users benefit from improved convenience and reduced redundancy, as they don't need to create separate accounts for each service. However, this model still presents privacy concerns since the IDP can potentially track user activities across different services. Furthermore, the dependency on the IDP means that if it is compromised, all relying parties are affected. Interoperability issues can also arise when different IDPs use varying standards and protocols.

### Decentralized Identity Model
The decentralized identity model, inspired by blockchain technology, represents a paradigm shift from centralized control to user-centric identity management. In this model, individuals have full control over their identity data and manage it independently. This approach uses Decentralized Identifiers (DIDs) and Verifiable Credentials (VCs) to establish and verify identities without relying on a central authority.

Decentralized identity systems allow for peer-to-peer relationships, where identities are managed directly between individuals and organizations. This model enhances privacy and security, as users can selectively disclose only the necessary information for a transaction or interaction. However, the decentralized model introduces technical complexity and requires new infrastructure and widespread adoption to become fully effective. Users must also manage their cryptographic keys securely to prevent identity loss.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- KNOW YOUR CUSTOMER -->
## Know Your Customer

Know Your Customer - KYC and KYB Know Your Business - KYB are regulatory and due diligence processes used to verify the identity of clients and prevent illegal activities such as money laundering and fraud.

KYC involves a series of checks that financial institutions must conduct to verify the identity of their clients. This includes gathering information such as name, address, date of birth, and proof of identity (e.g., passport, driver's license). The aim is to ensure that clients are who they claim to be and to assess the risk they may pose. KYC procedures typically involve a Customer Indentification Program - CIP, collecting and verifying customer identification information, Customer Due Diligence - CDD, assessing the customer's risk profile based on their background and transactional behavior and continuous monitoring.

In the context of SSI and digital identity, KYC can be enhanced by using VCs allowing secure and real-time verification while maintaining privacy.

KYB is a similar process but focuses on verifying the legitimacy and details of businesses rather than individuals. Both KYC and KYB are essential components of anti-money-laundering- AML and counter financing - CTF frameworks, helping to mitigate risks and comply with regulatory requirements.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- Airdrop -->
## Airdrop

Airdrops are a distribution mechanisme in the cryptocurrency and blockchain ecosystem where tokens or coins are sent to user's wallets, typically for free. The purpose is often to promote new projects, increase the circulation of a token or reward loyal users.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- DAPPS -->
## dApps

Decentralized applications, commonly known as dApps, are software applications that run on a blockchain or decentralized network rather than being hosted on centralized servers. They utilize smart contracts to facilitate various functions, providing transparency, security, and trust without a central authority.

In the context of SSI, dApps can be used to create, manage, and verify decentralized identities. For example, a dApp could allow users to store their verifiable credentials in a digital wallet, manage access to their personal data, and prove their identity to service providers without relying on a centralized identity authority.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- SSI TECH -->
### SSI Technology

The Self-Sovereign Identity is often conceptualized as a four distinct layers architecture :

<div align="center">
    <img src="images/architecture.png" alt="architecture">
</div>

Layer 1 : the identifiers and public keys layer involves the creation and management of DIDs and public keys.

Layer 2 : provides the protocols and interfaces necessary for secure, private and efficient communication between entities

Layer 3 : deals with the issuance, management and verification of VCs

Layer 4 : provides the policies, rules and standard that ensure the interoperability, trustworthiness and compliance of the SSI ecosystem

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- DECENTRALIZED IDENTIFIERS -->
## Decentralized Identifiers

A Decentralized Identifier - DID is a new type of globally unique identifier that can be used to identify any entity, whether it be a person, organization, device, or other digital resource. Unlike traditional identifiers, DIDs are designed to be self-sovereign, fully under the control of the entity they identify.

DIDs are designed to be a permanent identifier that does not need to change even if the underlying system or service provider changes, aren't managed by any central authority and are cryptographically verifiable : the DID is associated with a public/private key pair, and control over the DID can be proven by demonstrating control over the corresponding private key.

A DID consists of three parts :

<div align="center">
    <img src="images/did.png" alt="DID">
</div>

The Scheme indicated that the identifier is a DID, the method defines how the DID and its associdated DID document are created, resolved, updates and deactivated and finally, and a unique string that identifies the specific entity within the context of the DID method. Here is an example with an Ethereum address :

```
did:ethr:0x123456789abcdef123456789abcdef123456789abcdef
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- VCs -->
## Virtual Credentials

Virtual Credentials - VCs refer to digital versions of traditional physical credentials. They are a cornerstone of SSI systems as they allow :

- Identity verification : VSs can be used for verifying identity in various contexts such as online banking, airport security, and digital onboarding processes. For example, a person could use a Virtual Credential issued by their government to verify their identity when opening a bank account online.
- Access control : VCs can control access to physical and digital spaces. For instance, employees could use Virtual Credentials to access office buildings or secure online resources, ensuring that only authorized personnel can enter or gain access.
- Compliance and certifications : educational institutions and professional organizations can issue VCs to certify qualifications, professional memberships, or compliance with industry standards. This allows individuals to prove their credentials easily and securely to potential employers or clients.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- DIGITAL WALLET -->
## Digital Wallet

These credentials can be kept in digital wallets capable of storing and managing such credentials but also providing security/encryption and backup/recovery options.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- DIGITAL AGENT -->
## Digital Agent

Digital wallets are often paired with digital agent, which act similarly to an operation system, mediating all interactions between the wallet, the user and other agents. Digital agents perform tasks such as generating cryptographic key pairs, initiating DID-to-DID connections, securing communication and managing credential issuance and verification.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GOVERNANCE FRAMWORK -->
## Governance framework

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- DECENTRALIZED KEY MANAGEMENT -->
## Decentralized key management

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CRYPTOGRAPHY TECHNIQUES -->
## Cryptography techniques

### Hash functions
### Encryption
### Digital Signatures
### Verifiable Data Structures
### Proofs
#### Zero-Knowledge Proofs

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTACT -->
## Contact

Your Name - [@your_twitter](https://twitter.com/your_username) - email@example.com

Project Link: [https://github.com/your_username/repo_name](https://github.com/your_username/repo_name)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


