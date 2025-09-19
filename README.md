# EX-02-Cross-Platform-Prompting-Evaluating-Diverse-Techniques-in-AI-Powered-Text-Summarization
### NAME : SUJAN S B
### REGISTER NUMBER : 212222060262

## AIM
To evaluate and compare the effectiveness of prompting techniques (zero-shot, few-shot, chain-of-thought, role-based) across different AI platforms (e.g., ChatGPT, Gemini, Claude, Copilot) in a specific task: text summarization.

## Scenario:
You are part of a content curation team for an educational platform that delivers quick summaries of research papers to undergraduate students. Your task is to summarize a 500-word technical article on "The Basics of Blockchain Technology" using multiple AI platforms and prompting strategies.

Your goal is to determine which combination of prompting technique + platform provides the best summary in terms of:

Accuracy – Correctness of technical details

Coherence – Logical flow and readability

Simplicity – Ease of understanding for undergraduate students

Speed – Response time for generating the summary

User experience – Ease of prompt creation and AI interaction

## Algorithm
## Article : The Basics of Blockchain Technology

```
What is blockchain technology?
Blockchain technology is an advanced database mechanism that allows transparent information sharing within a business network. A blockchain database stores data in blocks that are linked together in a chain. The data is chronologically consistent because you cannot delete or modify the chain without consensus from the network. As a result, you can use blockchain technology to create an unalterable or immutable ledger for tracking orders, payments, accounts, and other transactions. The system has built-in mechanisms that prevent unauthorized transaction entries and create consistency in the shared view of these transactions.

Why is blockchain important?
Traditional database technologies present several challenges for recording financial transactions. For instance, consider the sale of a property. Once the money is exchanged, ownership of the property is transferred to the buyer. Individually, both the buyer and the seller can record the monetary transactions, but neither source can be trusted. The seller can easily claim they have not received the money even though they have, and the buyer can equally argue that they have paid the money even if they haven’t.

To avoid potential legal issues, a trusted third party has to supervise and validate transactions. The presence of this central authority not only complicates the transaction but also creates a single point of vulnerability. If the central database was compromised, both parties could suffer.

Blockchain mitigates such issues by creating a decentralized, tamper-proof system to record transactions. In the property transaction scenario, blockchain creates one ledger each for the buyer and the seller. All transactions must be approved by both parties and are automatically updated in both of their ledgers in real time. Any corruption in historical transactions will corrupt the entire ledger. These properties of blockchain technology have led to its use in various sectors, including the creation of digital currency like Bitcoin.

How do different industries use blockchain?
Blockchain is an emerging technology that is being adopted in innovative manner by various industries. We describe some use cases in different industries in the following subsections:

Energy
Energy companies use blockchain technology to create peer-to-peer energy trading platforms and streamline access to renewable energy. For example, consider these uses:

Blockchain-based energy companies have created a trading platform for the sale of electricity between individuals. Homeowners with solar panels use this platform to sell their excess solar energy to neighbors. The process is largely automated: smart meters create transactions, and blockchain records them.
With blockchain-based crowd funding initiatives, users can sponsor and own solar panels in communities that lack energy access. Sponsors might also receive rent for these communities once the solar panels are constructed.
Finance
Traditional financial systems, like banks and stock exchanges, use blockchain services to manage online payments, accounts, and market trading. For example, Singapore Exchange Limited, an investment holding company that provides financial trading services throughout Asia, uses blockchain technology to build a more efficient interbank payment account. By adopting blockchain, they solved several challenges, including batch processing and manual reconciliation of several thousand financial transactions.

Media and entertainment
Companies in media and entertainment use blockchain systems to manage copyright data. Copyright verification is critical for the fair compensation of artists. It takes multiple transactions to record the sale or transfer of copyright content. Sony Music Entertainment Japan uses blockchain services to make digital rights management more efficient. They have successfully used blockchain strategy to improve productivity and reduce costs in copyright processing.

Retail
Retail companies use blockchain to track the movement of goods between suppliers and buyers. For example, Amazon retail has filed a patent for a distributed ledger technology system that will use blockchain technology to verify that all goods sold on the platform are authentic. Amazon sellers can map their global supply chains by allowing participants such as manufacturers, couriers, distributors, end users, and secondary users to add events to the ledger after registering with a certificate authority. 

```
# ChatGPT:

### Zero Shot Prompting:

#### Prompt:
“Summarize the following article on blockchain technology in simple terms for undergraduate students."

#### Output:
Blockchain is a secure, tamper-proof database that stores data in linked blocks. It allows transparent transactions without needing a central authority.
Importance: It ensures trust, reduces fraud, and updates all parties in real time.

Uses:
Energy: Peer-to-peer electricity trading.
Finance: Faster, reliable payments and accounts.
Media: Track copyrights and pay artists fairly.
Retail: Verify product authenticity and supply chains.

### Few Shot Prompting:

#### Prompt:
Example : Here is a summary of a technical article on AI: ‘AI is a technology that enables machines to perform tasks that normally require human intelligence.’

Now summarize the following article on blockchain technology in the same simple style for undergraduate students:

#### Output:
Blockchain is a technology that allows secure and transparent recording of transactions in a way that cannot be altered. It removes the need for a central authority and is used in areas like energy trading, finance, media copyright management, and retail supply chain tracking.

### Chain-of-Thought:
#### Prompt:
“Read the following article on blockchain technology: 
First, explain the main points step by step. Then, provide a concise summary suitable for undergraduate students.”
#### Output:
Step-by-step explanation of main points
What is Blockchain Technology?
Blockchain is a special type of database.
Data is stored in “blocks” that are linked in a “chain.”
Once added, data cannot be changed or deleted without network consensus.
This makes the system secure, transparent, and tamper-proof.
It’s used to track orders, payments, accounts, and other transactions.
Why is Blockchain Important?
Traditional systems require a trusted third party (like a bank) to validate transactions.
Without a central authority, disputes can happen, e.g., a buyer or seller could lie about payment.
Centralized systems are vulnerable: if hacked, all parties suffer.
Blockchain creates a decentralized ledger:
Each party has a copy of the ledger.
Transactions are approved by all parties.
Any tampering corrupts the entire ledger.
This ensures security, transparency, and trust.
Example: used in digital currencies like Bitcoin.
How Industries Use Blockchain:
Energy:
Peer-to-peer electricity trading between homeowners.
Automated transactions via smart meters.
Crowdfunding community solar projects.
Finance:
Banks and exchanges use blockchain for payments, accounts, and trading.
Reduces manual errors and processing delays.
Media & Entertainment:
Manage copyright data efficiently.
Ensure artists are paid fairly.
Example: Sony Music uses blockchain for digital rights management.
Retail:
Track goods from suppliers to buyers.
Verify product authenticity.
Example: Amazon uses blockchain to track global supply chains.

Concise Summary for Undergraduate Students
Blockchain is a secure and tamper-proof database that stores data in linked blocks. It removes the need for a central authority and ensures trust and transparency in transactions. Industries use it in different ways: energy companies for peer-to-peer electricity trading, banks for faster payments, media for copyright management, and retail for supply chain tracking and product verification.


### Role-Based:
#### Prompt:
“You are a university professor teaching first-year students. Summarize the following article on blockchain technology in simple, clear terms, highlighting the key concepts:"

#### Output:
What is Blockchain?
Blockchain is a type of database that stores information in “blocks” which are linked together like a chain. Once something is recorded, it cannot be changed without agreement from everyone in the network. This makes it secure, transparent, and reliable for tracking transactions, payments, or accounts.
Why is Blockchain Important?
In traditional systems, transactions rely on a central authority, like a bank, to prevent disputes. This can be slow, costly, and risky if the central system is hacked. Blockchain solves this by giving everyone a shared, tamper-proof ledger. For example, in a property sale, both buyer and seller have a copy of the ledger, and all transactions are automatically updated in real time, making cheating or errors almost impossible.
How Industries Use Blockchain:
Energy: Homeowners with solar panels can sell extra electricity to neighbors. Crowdfunding allows communities to build solar projects.
Finance: Banks and stock exchanges use blockchain to make payments and trading faster, accurate, and less manual.
Media & Entertainment: Companies like Sony Music track copyrights and ensure artists are paid fairly.
Retail: Retailers like Amazon verify product authenticity and track supply chains globally.
In short: Blockchain is a secure, decentralized system that helps industries record, share, and verify transactions efficiently and transparently.


# Gemini:

### Zero Shot Prompting:

#### Prompt:
“Summarize the following article on blockchain technology in simple terms for undergraduate students."
#### Output:
Blockchain is a decentralized database that stores data in linked, chronological blocks, creating a tamper-proof and immutable ledger for transactions. Its primary purpose is to eliminate the need for a central, trusted authority, which can be a single point of failure. Instead, a network of users validates all transactions through consensus, making the system more secure and transparent. Various industries are adopting this technology, including finance for streamlined payments, retail for tracking product authenticity, and media for managing digital copyrights. This decentralized approach builds trust and efficiency across business networks.

### Few Shot Prompting:

#### Prompt:
Example : Here is a summary of a technical article on AI: ‘AI is a technology that enables machines to perform tasks that normally require human intelligence.’

Now summarize the following article on blockchain technology in the same simple style for undergraduate students:

#### Output:
Blockchain is a technology that creates a secure, decentralized, and tamper-proof ledger for transparent data sharing.


### Chain-of-Thought:
#### Prompt:
“Read the following article on blockchain technology: 
First, explain the main points step by step. Then, provide a concise summary suitable for undergraduate students.”
#### Output:
Main Points of the Article
Here is a step-by-step breakdown of the core concepts and applications of blockchain technology as described in the article.
1. What is Blockchain Technology?
Blockchain is an advanced database system that stores data in blocks linked together in a chronological chain. This structure ensures that the data is unalterable and immutable, as any changes or deletions require a consensus from the entire network. This makes it a transparent and reliable ledger for tracking transactions.
2. Why is Blockchain Important?
Traditional transaction systems rely on a central, trusted third party (like a bank), which creates a single point of vulnerability and can complicate transactions. Blockchain solves this by creating a decentralized, tamper-proof system. It provides all parties with a shared, real-time ledger, eliminating the need for a middleman and increasing trust and security.
3. How Different Industries Use Blockchain
Energy: Used for peer-to-peer energy trading platforms and crowdfunding renewable energy projects.
Finance: Employed to manage online payments and interbank accounts, improving efficiency and reducing manual reconciliation.
Media and Entertainment: Helps manage copyright data and streamline digital rights, ensuring fair compensation for artists.
Retail: Utilized to track the movement of goods in a supply chain to verify product authenticity and prevent fraud.

Concise Summary for Undergraduate Students
Blockchain is a decentralized database technology that creates a secure, unalterable record of transactions, eliminating the need for a central authority and enabling transparent data sharing across various industries.


### Role-Based:
#### Prompt:
“You are a university professor teaching first-year students. Summarize the following article on blockchain technology in simple, clear terms, highlighting the key concepts:"

#### Output:
What is Blockchain?
Imagine a digital notebook for transactions. Instead of a single person holding the notebook, thousands of people all have an identical copy. That's the basic idea of blockchain.
It's a special kind of database where information is stored in "blocks." These blocks are then securely linked together in a long, chronological "chain." The key takeaway is that once a piece of information is recorded, you can't go back and change or delete it without everyone in the network agreeing. This makes the record tamper-proof and incredibly reliable.
Why is it So Important?
The main reason blockchain is a big deal is because it eliminates the need for a middleman you have to trust. Think about buying a house; a bank or lawyer acts as a central authority to ensure the transaction is legitimate. With blockchain, the network itself acts as the authority. All parties have a shared, constantly updated copy of the ledger, which builds trust and removes the single point of failure that a traditional central database can have.
Where is it Used?
While it's famous for creating cryptocurrencies like Bitcoin, blockchain has many other practical uses:
Finance: Banks can use it to make payments between different institutions faster and more efficient.
Supply Chains: Companies can track products from the factory to the store to make sure they're authentic.
Media: Artists can use it to prove ownership of their work and ensure they're properly compensated for its use.

## Conclusion :

ChatGPT outperformed Gemini in terms of simplicity, coherence, and user-friendliness, making it the preferred platform for educational text summarization.

## Result :

#### ChatGPT: 
Produced summaries that were accurate, coherent, simple, and easy to understand, making it ideal for undergraduate students.
#### Gemini:
Summaries were accurate and coherent, but slightly less simple and easy to read compared to ChatGPT.

Scoring Key (1–5):
5 = Excellent, 4 = Good, 3 = Average, 2 = Poor, 1 = Very Poor

<img width="1100" height="153" alt="image" src="https://github.com/user-attachments/assets/7c40675c-15f6-4337-8f88-00cb0ad99932" />

ChatGPT outperformed Gemini in terms of simplicity, coherence, and user-friendliness, making it the preferred platform for educational text summarization.
