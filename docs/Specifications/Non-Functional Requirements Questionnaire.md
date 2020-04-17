# Non-Functional Requirement Questionnaire

This questionnaire is based on the Enterprise Ethereum Alliance's (EEA) Non-Functional Requirement (NFR) Survey that was developed by the EEA Mainnet Working Group - Use Cases Task Force. The EEA Mainnet Working Group Task Force's survey can be accessed [here](https://forms.gle/gCv5WZK9yiaCK5Y86) and will remain open for the community to submit their responses until **May 1, 2020**. 

The purpose of this document is to serve as a reference to a methodology that can be used to gathering and communicate NFRs to stakeholders. 

## Table of Contents

* [Barriers and Challenges](https://github.com/EnvisionBlockchain/baseline/blob/specs/docs/Non-Functional%20Requirements%20Questionnaire.md#barriers-and-challenges)  
* [General](https://github.com/EnvisionBlockchain/baseline/blob/specs/docs/Non-Functional%20Requirements%20Questionnaire.md#general)  
* [Performance](https://github.com/EnvisionBlockchain/baseline/blob/specs/docs/Non-Functional%20Requirements%20Questionnaire.md#performance)  

## Barriers and Challenges
The sections below ([Technology](https://github.com/EnvisionBlockchain/baseline/blob/specs/docs/Non-Functional%20Requirements%20Questionnaire.md#technology-barriers), [Compliance](https://github.com/EnvisionBlockchain/baseline/blob/specs/docs/Non-Functional%20Requirements%20Questionnaire.md#compliance-barriers), and [Business](https://github.com/EnvisionBlockchain/baseline/blob/specs/docs/Non-Functional%20Requirements%20Questionnaire.md#business-barriers)) may act as significant barriers to implementation or adoption of your application on Mainnet. Go through each section and check off everything that applies. Please feel free to add anything else that's not included.

### Technology Barriers
Check off all that apply below:
- [ ] **Scaling Problem**: My application requires hundreds or thousands of transactions per section, which public chains can't handle
- [ ] **Speed and Latency Problem**: Our CRM and ERP systems don’t need the kind of Transaction Per Second speeds of a Visa or Mastercard (and even they get those TPS rates through parallelization...can’t fool me). But long wait times for round-trip + consensus makes things I might do with mainnet a bad user experience.
- [ ] **Noisy Neighbors must not disrupt my operations**: As an enterprise conducting mission-critical operations that rely on predictable operation timing, I need to be comfortable that a “cryptokitty” event isn’t a possibility. I need to know that, even though the Mainnet is a public utility, there is reasonable assurance by some means that the reads, writes and computations I need to conduct business on the Mainnet will not be reduced to a crawl by the activities of others.
- [ ] **Finality Problem**: Mainnet is an “eventual consistency”. If that’s changing with Eth2.0, I don’t understand it...something about a magical fast finality something. I dunno. What I do know is that all my systems are ones where a change to data is final the second it’s written.

### Compliance Barriers
Check off all that apply below:
- [ ] **Data Locality Problem**: GDPR requires that I can account for where PII data is stored, even when it is encrypted. And I need to be able to delete that data permanently upon request. If the data is sitting permanently on any number of nodes not controlled by me everywhere...yeah.
- [ ] **Responsible Party Problem**: My legal structure requires that there be a responsible party handling all aspects of my data and business logic. If I put data on the Mainnet, I lose a key responsible party.
- [ ] **Opt-In KYC**: I need to know who I'm transacting with, and to register a Mainnet address/identity with KYC/AML: "TSA Precheck" for Identity.

### Business Barriers
Check off all that apply below:
- [ ] **Cost Problem**: It’s not about how much it costs per transaction or that our company isn’t yet set up to hold ETH for “gas.” It’s also about the unpredictability of the cost. And I don’t want to have to go back for my degree in finance to understand stablecoins just to manage IT.
- [ ] **Gas Reserves**: As a company whose treasury still isn’t comfortable holding cryptocurrency, I need an easy and safe way to maintain gas reserves necessary to conduct operations. (This does not include custodianship of coins and tokens held as assets or currency, but rather as a commodity needed to run non-financial operations, store data and proofs, generate shield contracts and other cryptographic methods, and power transactions that may or may not be conducting financial transfers.).
- [ ] **Private Data Problem**: Eighty percent of our data is considered sensitive, internal or personally identifiable client, customer or user data. Encryption isn’t enough. Any data can be deanonymized and decrypted given time. And anyone with a full node has forever to crunch the bits on the ledger.  So I don't like putting even encrypted data on a public chain.
- [ ] **Strategy Leaks Problem**: Transaction metadata can be used to game the system or collect / analyze for strategic counterintelligence or corp. espionage. In the age of AI, any trace activity done on a permanent, public ledger can be used to figure out who is doing what, even if it’s just little changes to Merkle tries.
- [ ] **Confidential Code Problem**: You can’t just hide the data with something like ZK-SNARKS and think that everything is ok from a corporate perspective. Many business agreements are embodied in code... business logic. If a machine can execute a smart contract, it can decompile and look at the logic, and that can leak sensitive info.
- [ ] **Non-Rational (Power) Problems**: IBM, Oracle, SAP and others are telling me what to use. They have intimated that if I don't promote their version of private, permissioned blockchain, they might be less interested in selling my offerings to their customers, and we rely on that.  [Or any number of other reasons why one might not choose Mainnet, even if one believed it was a good technical fit.]
- [ ] **Emotional**: Bitcoin and Ethereum are for criminals and terrorists.  I don't want to be associated with that, and I'm afraid of what might happen if government cracked down on public blockchains.

## General

### Which vertical or horizontal is your use case in?
Check off the vertical or horizontal that that applies:
- [ ] Finance
- [ ] Insurance
- [ ] Media
- [ ] Gaming & Entertainment
- [ ] Education
- [ ] Energy
- [ ] Healthcare
- [ ] Manufacturing
- [ ] Supply Chain
- [ ] Transportation
- [ ] Retail
- [ ] Real Estate
- [ ] Food & Beverage
- [ ] Hospitality
- [ ] Telecommunications
- [ ] Technology

### Please describe your application/use case involving Mainnet in as much detail as possible.

> A description of your application or use case goes here. 

### What systems does your use case need to integrate with?

> List specific systems such as CRM, ERP, IMS, etc.

### Please list the types of user roles in your use case.

> User roles that will need to interact with the application. For example in an Procurement use cases you may have a Buyer and a Supplier.

### What are your concerns about using Mainnet in this application?

> Similar to the Barriers and Challenges section above, but will allow for an open ended answer to collect feedback.

### What are the business processes and user journeys that are most critical?

> Narratives and diagrams are a good way to explain your business process and user journey. To see an example of the procurement use case defined in the Radish34 demo click [here](https://docs.baseline-protocol.org/radish34/radish34-workflow).

### If you have a preferred architectural stack in mind for this use case, please explain.

> Please include any considerations for cloud technologies, software components, etc. 

### How would you like to provide access to users of the system?

> Please include any considerations for where end users would access the system. Check all that apply: 

- [ ] Web/Mobile Interface
- [ ] Desktop Application
- [ ] Command Line Interface (CLI)
- [ ] Integrated natively into an existing system

## Performance


### Do you have performance requirements regarding transaction completion time for your use case?

> Please explain any specific requirements that involve transaction completion time. For example, a work flow may require a transaction to complete before starting.

### Do you have performance requirements regarding user interface responsiveness, data updates, queries, etc? Please explain.

> Please explain any specific requirements that involve transaction completion time. For example, a workflow may require a transaction to complete before starting a new state.

### How many write transactions per year do you anticipate for your use case?

> Think about your use case process flow and try to quantify the number of write transactions. You can think in terms of days, weeks, or months. 

### How do you anticipate transaction volume changing in the future?

> Try to imagine how you number of write transactions will change over the next year, 2 years, 5 years, etc. 

### What is the impact of not meeting the performance requirement for use case? Please explain.

> This question intends to capture the impact of the application not meeting performance requirements. For example, you can think in terms of monetary impact such as dollar loss.

### How important is the ability to prevent unauthorized changes (writes) or viewing access (reads) to data to your use case? What would be the legal and cost implications if an unauthorized change occurred.

> For example, is it a regulatory factor? Be as descriptive as possible. 

### Do you have any Service Level Agreements (SLA) that need to be met for your use case?

> Explain any SLAs that your use case will need to honor.

### Are there any specific blockchains your use case would need to be interoperable with?

> This could include any public blockchain and private blockchain.




