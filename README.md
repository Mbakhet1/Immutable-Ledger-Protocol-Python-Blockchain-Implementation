# Immutable-Ledger-Protocol-Python-Blockchain-Implementation
Project Overview
This repository features a custom-built Blockchain protocol designed to demonstrate how decentralized systems ensure data security and immutability. By leveraging object-oriented programming in Python, the system creates a linear chain of blocks where each unit is cryptographically tied to its predecessor.

Key Technical Features
Cryptographic Hashing: Every block generates a unique digital fingerprint using the SHA-256 algorithm, ensuring that even a single character change in the data results in a completely different hash.

Sequential Integrity: Each new block stores the hash of the previous block, creating a secure, unbreakable chain.

Automated Validation: A built-in is_chain_valid function constantly monitors the ledger for inconsistencies, providing a real-time security audit.

The Tampering Test: Proof of Security
The primary strength of a blockchain is its resistance to unauthorized modification. To prove the effectiveness of this system, I performed a "Tamper Test" by manually altering data within an existing block and re-validating the chain.

Test Results
Standard Operation: When the ledger is functioning normally, the system confirms that all hashes align and the chain is "Valid".

Tampered State: Upon modifying a transaction, the cryptographic link is immediately severed. The system detects the hash mismatch and flags the ledger as "Invalid," as shown in the screenshot below.

[Insert Your Screenshot of the Tampered Data/Error Message Here]
Figure 1: Demonstration of the system detecting a hash mismatch after data tampering.

Technical Stack
Language: Python

Libraries: hashlib (for SHA-256), json (for data formatting), datetime (for block timestamps)

Environment: Jupyter Notebook

Key Insights
Data Immutability: Proved that once a transaction is added to the ledger, it is computationally impossible to alter it without detection.

System Resilience: Explored the logic of decentralized trust, where the system relies on mathematics rather than a central authority to verify facts.

How to Run
Clone the Repo: Download the blockchain.ipynb file.

Open in Jupyter: Launch the notebook and run the cells sequentially to see the blocks being generated and hashed in real-time.

Experiment: Try changing a transaction value in an early block and run the validation cell to see the security protocol in action.

About the Author
Mohamed A. Bakhet
Bachelor of Science in Business Analytics and Information Systems
University of South Florida (USF)

I am a data professional specializing in technical systems that prioritize data integrity and actionable business intelligence. My work focuses on bridging the gap between backend engineering and front-end analytics.  

Location: Sarasota, FL

LinkedIn: Mohamed Bakhet

Email: mbakhet833@gmail.com<img width="1045" height="778" alt="Screenshot 2026-05-13 100827" src="https://github.com/user-attachments/assets/8850ce97-bf89-4dfe-a59a-d11f05fb9961" />
