# VeChain General Grant Application - Praise, Recognize. Rewarrd. Repeat

## Project Overview

* **Project:** Praise
* **Team Name:** General Magic
* **Payment Address:** 0x0b7246ef74ca7b37fdc3d15be4f0b49876622f95 (givepraise.eth)

### Overview

* **A brief description of the project.**

Introducing Praise for VeChain: a game-changing, community-driven reputation and rewards platform that will revolutionize the way we engage within the VeChain ecosystem! Praise empowers community members to celebrate each other's contributions and ignite a spirit of collaboration like never before.

Get ready to unlock a whole new world of possibilities with features such as customizable reputation tokens, seamless reward distribution, cutting-edge analytics, and seamless integration with popular communication channels like Discord. With Praise for VeChain, we're not just building a thriving ecosystem—we're creating a movement that will fuel project success, inspire innovation, and foster a culture of gratitude and mutual support.

* **An indication of why your team is interested in creating this project within the VeChain Ecosystem.**

**Our team is incredibly excited to bring the Praise to the VeChain ecosystem for several key reasons:**

1. **Synergy with VeChain's vision:** VeChain's commitment to building a trust-free and distributed ecosystem aligns perfectly with Praise's objectives of fostering a transparent, community-driven reputation and rewards system. We believe that integrating Praise into the VeChain ecosystem will significantly enhance user experience and engagement.
2. **Robust infrastructure:** VeChain's established infrastructure, with its fast and scalable blockchain technology, provides an ideal foundation for Praise to thrive.
3. **Wide adoption and vibrant community:** VeChain's vast and diverse ecosystem, spanning multiple industries and applications, offers a fantastic opportunity for Praise to make a tangible impact across numerous communities. We envision Praise becoming a critical component in enhancing collaboration, project success, and overall satisfaction for the VeChain community.
4. **Mutual growth and innovation:** By integrating Praise into the VeChain ecosystem, we aim to drive continuous improvement and innovation for both platforms. As Praise evolves and expands its offerings, it will contribute to the growth and success of the VeChain ecosystem, while simultaneously benefiting from the advancements made within the VeChain community.

* **If relevant, an indication of how you will integrate tools and features (e.g., Sync2/Connex, fee delegation protocols, MTT, etc) to enhance your project.**

To enhance the Praise project within the VeChain ecosystem, we plan to integrate several key tools and features, which will provide an optimized and seamless experience for users:

* **Sync2/Connex integration:** Sync2 and Connex provide a powerful combination of wallet and dApp interaction capabilities. We plan to leverage these technologies to offer a smooth user experience for community members as they interact with Praise. By integrating Sync2/Connex, users can easily manage their reputation tokens, NFT badges, and other rewards directly through their VeChain wallets, fostering a more cohesive and secure environment.
* **Integration with VeChain's ecosystem partners:** To maximize Praise's impact and reach, we plan to explore collaborations with VeChain's ecosystem partners. By partnering with projects already established within the VeChain ecosystem, Praise can expand its use cases and enhance the value it offers to both new and existing communities.

By integrating these tools and features into the Praise project, we aim to provide a seamless, efficient, and enjoyable experience for users within the VeChain ecosystem. This will ultimately contribute to the growth and success of Praise, VeChain, and their respective communities.

### Ecosystem Fit

Are there any other projects similar to yours? If so, how is your project different?

There are several projects with similarities to ours in the web3 reputation and rewards ecosystem. However, our project stands out due to several unique features and competitive advantages. Here's a brief comparison:

* **Data Source:** Our project can capture data from a variety of sources, such as Discord, Telegram, and Slack. This flexibility sets us apart from competitors that rely on specific platforms, API integrations, or custom integrations.
* **Reputation Scores:** Our system calculates reputation scores for users, a feature shared by some competitors like Karma, Deep Skills, and Gitpoap, but not all.
* **Reward Distribution:** We support reward distribution, which not all competitors offer. For instance, Coordinape and Deep Skills do provide this feature, but others like Lighthouse and Graph Commons do not.
* **Cultural Build:** Our project emphasizes building a strong community culture, which is a unique selling point compared to other projects focused solely on reputation scores or contribution graphs.
* **Profile Generation**: We generate comprehensive user profiles, similar to Disco.xyz, Gitcoin, Deep Skills, and Gitpoap.
* **Contribution Graph:** Our project offers visual contribution graphs, which is a feature not available in many other platforms like Lighthouse, Otterspace, or Coordinape.
* **Attestation:** We provide various forms of attestation, including NFTs, badges, and verifiable credentials. Some competitors offer only one or two forms of attestation.
* **Open Source:** Our project is open source, making it easily accessible for developers and organizations to integrate, modify, or extend its features.

### Project Details

* [Mockups/designs of any UI components](https://miro.com/app/board/uXjVMXmS_5k=/)
* API specifications of the core functionality

## Overview

The Praise Reputation Minter App API is designed to provide core functionality for the Praise Reputation Minter App on the VeChain ecosystem. The API allows developers to interact with the app and perform various operations, such as creating and managing reputation scores, minting reputation tokens, and querying user profiles.

## Core Endpoints

### Reputation Management

* POST /api/reputation/create: Creates a new reputation score for a user.
* PUT /api/reputation/update: Updates an existing reputation score for a user.
* DELETE /api/reputation/delete: Deletes a reputation score for a user.
* GET /api/reputation/:user: Retrieves the reputation score for a user.

### Token Minting

* POST /api/token/mint: Mints new reputation tokens for a user based on their reputation score.
* GET /api/token/balance/:user: Retrieves the current balance of reputation tokens for a user.

### User Profiles

* POST /api/profile/create: Creates a new user profile.
* PUT /api/profile/update: Updates an existing user profile.
* GET /api/profile/:user: Retrieves a user profile by user ID.

## Authentication & Authorization

All API requests should include an authentication token in the header, using the format Authorization: Bearer . This token can be obtained by registering an account and generating an API key from the Praise Reputation Minter App dashboard.

* **An overview of the technology stack to be used**

1. **Smart Contracts:** Written in Solidity, leveraging the Ethereum Virtual Machine (EVM) compatibility of the VeChainThor blockchain.
2. **VeChain SDKs and Tools:** Utilize VeChain’s Connex, Sync2, and other relevant SDKs to facilitate interaction with the VeChainThor blockchain, handle wallet management, and enable seamless integration of the app with the VeChain ecosystem.
3. **Backend:** Node.js and Express.js for building and deploying the backend server, which will handle API requests, manage the database, and interact with the smart contracts on the VeChainThor blockchain.
4. **Database:** MongoDB or PostgreSQL to store user profiles, reputation data, and other relevant information.
5. **Frontend:** React.js or Vue.js for building a user-friendly and responsive web interface for the Reputation Minter App, allowing users to easily manage their reputation scores, mint tokens, and interact with their profiles.
6. **API:** RESTful API built using Express.js to expose the core functionality of the app, such as managing reputation scores, minting tokens, and querying user profiles.
7. **Deployment and Hosting:** Services like AWS, Google Cloud Platform, or Heroku for hosting the backend server and database, and services like Netlify or Vercel for deploying and hosting the frontend web application.
8. **Version Control and Collaboration:** Git and GitHub for version control, code reviews, and collaboration among team members.

* **Documentation of core components, protocols, architecture, etc. to be deployed**

1. **Reputation Management:** The reputation management component handles creating, updating, and deleting reputation scores for users. It will interact with the smart contracts to maintain an accurate and up-to-date representation of users’ reputation scores.
2. **Token Minting:** This component is responsible for minting new reputation tokens based on users’ reputation scores. It will interact with the smart contracts to mint tokens and update users’ token balances accordingly.
3. **User Profiles:** The user profile component will store and manage user-related data, such as their reputation scores, token balances, and personal information. This data will be stored in a database, with access controlled by the backend server.
4. **VeChain Integration:** The project will leverage VeChain’s SDKs and tools, such as Connex and Sync2, to facilitate seamless integration with the VeChainThor blockchain and enable wallet management and other crucial functions.

* **PoC/MVP or other relevant prior work or research on the topic**

Praise is live as a product check it out [here!](https://givepraise.xyz/)

**Milestone 1: Smart Contracts Development ($10,000)**

Estimated Duration: 2 weeks

Week 1:

* Develop and deploy ERC-20 reputation token smart contract on VeChain.
* Create token factory smart contract.

Week 2:

* Test smart contracts and ensure they function as expected.
* Provide documentation and a testing guide for the smart contracts.

**Milestone 2: API Development ($7,500)**

Estimated Duration: 2 weeks

Week 1:

* Develop Praise API with endpoints for managing contract addresses, distributions, and other necessary functionality.

Week 2:

* Thoroughly test the API.
* Ensure proper integration with the smart contracts.
* Provide documentation and a testing guide for the API.

**Milestone 3: Frontend Development ($7,500)**

Estimated Duration: 4 weeks

Week 1-2:

* Design and develop the frontend for the token creation wizard.
* Implement the reputation minting wizard.
* Ensure seamless integration with the Praise API.

Week 3:

* Develop the overview page, including minting and distribution summary and other relevant information.

Week 4:

* Conduct thorough testing of the frontend, ensuring proper functionality and user experience.
* Create a user guide or demo video showcasing the features of the application.
* Finalize the project and prepare for deployment.

## Team

### Team members

Praise is a project built by[ General Magic](https://generalmagic.io/) with a lot of support from rockstar DAO OGs. [@kristoferlund](https://twitter.com/kristoferlund) and [@JCukini](https://twitter.com/JCukini) are the project leads with design by[ @markoprljic](https://twitter.com/markoprljic), development by [@nebsaas](https://twitter.com/nebsaas), [@Vyvy_viM](https://twitter.com/Vyvy_viM), [@mhmdksh](https://twitter.com/mhmdksh?t=AUwTFQg7Wr-q22T6ESWcsw&s=09) and[ @thegrifft](https://twitter.com/thegrifft) as the product owner. [@anamarie_com](https://twitter.com/anamarie_com), [@AAbugosh](https://twitter.com/aabugosh),[ @ZeptimusQ](https://twitter.com/zeptimusQ), and Giveth, Commons Stack and the Token Engineering Commons are all supporting the effort as well.

### Team Website

* https://givepraise.xyz/

### Team's experience

The Praise team is composed of experienced Web3 professionals with a strong background in the Ethereum ecosystem, offering comprehensive product development for impact-driven projects. Our diverse team includes talented designers, developers, system architects, researchers, writers, and seasoned Web3 experts who have a deep understanding of the unique challenges and requirements of the blockchain space.

We have experience in developing and launching similar projects and products, ensuring our ability to execute on our vision for Praise within the VeChain ecosystem.

Praise is being used by many communities in the ethereum ecosystem to mention some:

* Giveth
* Token Engineering Commons
* BanklessDAO
* Dappnode
* Gnosis

### Team Code Repos

* https://github.com/givepraise/praise
* https://github.com/kristoferlund

### Team LinkedIn Profiles

|Name|LinkedIn|
| --- | --- |
|Ahmad|https://www.linkedin.com/in/ahmadabugosh/|
|Marko|https://linkedin.com/in/markoprljic|
|Nebs|https://www.linkedin.com/in/nestojanovic/|
|Vyvyy|https://www.linkedin.com/in/vyvy-vi/|
|Justina|https://www.linkedin.com/in/justina-svitraite|
|Nuggan||
|Kristoffer|https://www.linkedin.com/in/kristoferlund/|
