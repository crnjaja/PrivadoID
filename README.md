
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
        <li><a href="#know-your-customer">Know your customer</a></li>
        <li><a href="#airdrop">Airdrop</a></li>
        <li><a href="#dapps">dApps</a></li>
      </ul>
    </li> 
    <li>
      <a href="#ssi-technology">SSI Technology</a>
      <ul>
        <li><a href="#virtual-credentials">Virtual credentials</a></li>
        <li><a href="#digital-wallet">Digital wallet</a></li>
        <li><a href="#digital-agent">Digital agent</a></li>
        <li><a href="#digital-wallet">Digital wallet</a></li>
        <li><a href="#decentralized-identifiers">Decentralized Identifiers</a></li>
        <li><a href="#decentralized-key-management">Decentralized key management</a></li>
        <li><a href="#governance-framework">Governance framework</a></li>
        <li><a href="#ssi-architecture">SSI architecture</a></li>
        <li><a href="#cryptography-techniques">Cryptography techniques</a></li>
      </ul>
    </li> 
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



### General

This section should list any major frameworks/libraries used to bootstrap your project. Leave any add-ons/plugins for the acknowledgements section. Here are a few examples.


<!-- BLOCKCHAIN -->
## Blockchain

check if needed

<!-- TOKENIZATION -->
### Token

check if needed

<!-- SMART CONTRACTS -->
### Smart Contracts

Smart contracts are simple programs that run on blockchain platforms, such as Ethereum. They are designed to execute specific actions automatically when predefined conditions are met. These contracts run in virtual machines, like the Ethereum Virtual Machine (EVM) or Ethereum Flavored WebAssembly (eWASM), ensuring that they are secure and tamper-proof.

Key Features of Smart Contracts :
- Autonomous Execution: Once deployed, smart contracts operate autonomously. They do not require human intervention to execute their instructions.
- Cost and Efficiency: Running smart contracts involves transaction fees, paid in the blockchain's native cryptocurrency (e.g., Ether on Ethereum). The fees, calculated in units called gas, ensure that the network remains sustainable and efficient.
- Interoperability: Smart contracts can interact with each other, enabling complex chains of actions and logic. This interoperability supports various applications, from simple wallets to sophisticated identity systems.
- Ownership and Control: Smart contracts can be owned by individuals, groups, or be entirely autonomous. The ownership model influences how the contract can be interacted with and controlled.
- Transparency and Security: The operations of smart contracts are transparent and verifiable by anyone on the network. This transparency enhances security and trust among participants.

Smart contracts play a pivotal role in decentralized identity systems. For example, ERC 725 v2 and ERC 1056 are specific types of smart contracts designed to support identity management on the Ethereum blockchain:

<!-- ZKP -->
### Zero Knowledge Proof

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

### Identity Models

 #### Centralized Identity Model
The centralized identity model is a traditional approach where a single, central authority manages and controls identity information. This model is prevalent in systems where government agencies, social media platforms, or service providers issue and maintain identification data. In this setup, individuals create accounts with the central entity, linking their identity to these accounts. The central authority owns and controls the identity data, making decisions about its use and access. This model is characterized by a single point of control, where the central entity oversees the creation, update, and deletion of identity records.

One of the significant issues with this model is privacy. Users have limited control over their personal data, and the central authority can use or share this data without the user's explicit consent. Additionally, centralized databases are attractive targets for cyberattacks, leading to potential data breaches and identity theft. Despite these risks, the centralized model remains widely used due to its simplicity and historical precedence.

#### Federated Identity Model
The federated identity model aims to address some of the limitations of the centralized model by allowing multiple organizations to share and verify identity information through a trusted third party known as an Identity Provider (IDP). This model enables Single Sign-On (SSO) capabilities, where users can access multiple services using one set of login credentials managed by the IDP.

In a federated system, users benefit from improved convenience and reduced redundancy, as they don't need to create separate accounts for each service. However, this model still presents privacy concerns since the IDP can potentially track user activities across different services. Furthermore, the dependency on the IDP means that if it is compromised, all relying parties are affected. Interoperability issues can also arise when different IDPs use varying standards and protocols.

#### Decentralized Identity Model
The decentralized identity model, inspired by blockchain technology, represents a paradigm shift from centralized control to user-centric identity management. In this model, individuals have full control over their identity data and manage it independently. This approach uses Decentralized Identifiers (DIDs) and Verifiable Credentials (VCs) to establish and verify identities without relying on a central authority.

Decentralized identity systems allow for peer-to-peer relationships, where identities are managed directly between individuals and organizations. This model enhances privacy and security, as users can selectively disclose only the necessary information for a transaction or interaction. However, the decentralized model introduces technical complexity and requires new infrastructure and widespread adoption to become fully effective. Users must also manage their cryptographic keys securely to prevent identity loss.

### Know Your Customer / Know Your Business

### Airdrop

### dApps

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Your Name - [@your_twitter](https://twitter.com/your_username) - email@example.com

Project Link: [https://github.com/your_username/repo_name](https://github.com/your_username/repo_name)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 
