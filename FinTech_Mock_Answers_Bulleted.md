# FinTech Mock Questions — Model Answers (Bullet-Point Version)

*Sources: blockchain, cryptocurrency, and stablecoin points draw on Imran Bashir,* Mastering Blockchain *(4th ed., Packt, 2023). FinTech and Cambodia-specific points come from general course material.*

---

## Part A — Financial Technology (FinTech) Fundamentals

### 1. What is FinTech, and how has it changed the way individuals and businesses access and use financial services?

**Definition:**
- FinTech = using modern software, the internet, and mobile devices to deliver, improve, and automate financial services.
- Covers mobile payments, digital wallets, online lending, robo-advisors, insurance tech ("insurtech"), and blockchain-based finance.

**How it changed financial life:**
- **Access** — moved from the bank branch to the smartphone; you can open an account, transfer money, pay bills, or invest from anywhere with a connection.
- **Disintermediation** — services that once needed a bank, broker, or clearing house in the middle can now happen directly between parties, cutting cost and friction.
  - Bashir: a blockchain is a platform where peers exchange value "without the need for a centrally trusted arbitrator."
- **Speed and personalisation** — apps use data and automation for instant decisions (e.g. instant loan approval) and tailored services banks were too slow to offer.
- **For businesses** — lower transaction costs, faster settlement, and the ability to reach customers who never had a bank account.

### 2. How have FinTech solutions improved the efficiency, speed, and accessibility of financial transactions compared to traditional banking?

- **Starting point:** traditional banking relies on layered intermediaries — correspondent banks, clearing houses, reconciliation — which add delay and cost.
  - Bashir: a shared ledger "does not require a lengthy process of verification, reconciliation, and clearance because a single version of agreed-upon data is already available."
- **Efficiency** — automation replaces manual paperwork; a loan or payment is processed by software, not staff, cutting overhead and error.
- **Speed** — transactions that took days (cheque clearing, wire transfers) are now near-instant; mobile payments settle in seconds, and cross-border transfers that took 3–5 days can finish in minutes.
- **Accessibility** — a branch has fixed hours and a location; an app is available 24/7 from a phone. This is the single largest change for rural users and those who never qualified for an account.

### 3. Discuss the role of mobile applications and internet technologies in the growth and adoption of FinTech in developing countries such as Cambodia.

- Mobile phones spread far faster and wider than bank branches in developing countries.
- Cambodia has high mobile and internet penetration but historically low traditional-bank coverage, so the phone became the main gateway to financial services — a "mobile-first" (often "mobile-only") market.
- Mobile apps cut the cost of serving a customer to almost zero, making it economical to reach low-income and rural users a physical bank could never profitably serve.
- Internet technologies — cloud computing, APIs, QR codes, real-time payment rails — let providers launch fast and connect to each other.
- **Cambodian examples:** Wing, TrueMoney, ABA Mobile, ACLEDA Mobile, Pi Pay, plus the Bakong system (National Bank of Cambodia) and the national KHQR code standard.
- Note: Bakong is built on distributed-ledger / blockchain technology of the kind Bashir's textbook describes.

### 4. In what ways has FinTech contributed to financial inclusion, especially for rural or underserved areas?

- **Financial inclusion** = giving previously "unbanked" or "underbanked" people access to useful, affordable services.
- **Lower barriers to entry** — opening a digital wallet needs only a phone number and basic ID, not a minimum deposit or branch visit.
- **Reach** — mobile networks cover areas with no bank branches, so a farmer in a remote province can receive, save, and transfer money.
- **Affordability** — digital transactions cost far less than handling cash or travelling to a distant bank.
- **Building credit histories** — transaction and payment data let lenders assess people with no formal credit record, opening access to small loans.
- **Agent networks** — cash-in/cash-out agents (local shops acting for providers) bridge cash and digital money in rural areas.
- Ties to Bashir's theme: decentralised, shared systems cut the need for costly intermediaries, which makes serving low-value rural customers viable.

### 5. Provide detailed examples of commonly used FinTech services in Cambodia and explain how they benefit users and providers.

- **Mobile money / e-wallets (Wing, TrueMoney, ABA Mobile, ACLEDA Mobile):** store money, transfer, top up phone credit, pay merchants.
  - *User benefit:* convenience, no full bank account needed.
  - *Provider benefit:* low-cost customer acquisition, fee and float income.
- **QR-code payments (KHQR standard):** one national QR standard lets any participating bank/wallet customer scan one code to pay any merchant.
  - *User benefit:* fast cashless payment, no card machine.
  - *Provider/merchant benefit:* cheaper than card terminals, no cash-handling risk.
- **Bakong (National Bank of Cambodia):** central, interoperable, blockchain-based payment backbone connecting banks and wallets instantly.
  - *User benefit:* send across institutions for free or low cost.
  - *Provider benefit:* shared infrastructure instead of building their own.
- **Digital lending and savings apps:** small loans and savings products via phone.
  - *User benefit:* fast credit access.
  - *Provider benefit:* data-driven risk assessment and scale.
- **Overall:** users gain convenience, speed, and inclusion; providers gain lower costs, fee income, and a larger market.

### 6. Analyse the impact of FinTech on traditional banks — competitor, collaborator, or both?

- **Answer: both — and increasingly a collaborator.**
- **As a competitor:**
  - FinTechs attack the most profitable, customer-facing parts of banking — payments, transfers, lending — with cheaper, faster, more user-friendly services.
  - They erode bank fee income and customer relationships.
- **As a collaborator:**
  - Banks have licences, capital, regulatory experience, and large customer bases; FinTechs have technology and agility.
  - Result is partnership: banks build their own apps, buy or invest in startups, and connect through shared rails.
  - Cambodia: Bakong is a clear collaboration example — the central bank provides shared infrastructure that banks and wallets plug into.
- **Bashir's framing:** blockchain could disintermediate banks, but he also expects a "collaborative future where connectivity between CeFi [centralised finance] and DeFi exists."
- **Realistic outcome:** coexistence and convergence — the line between "bank" and "FinTech" blurs.

### 7. What are the main challenges or limitations FinTech companies face in emerging markets?

- **Regulation and licensing** — rules are often unclear or developing; FinTechs must meet AML and KYC requirements.
  - Bashir notes regulation is one of blockchain's hardest problems, with AML and CFT rules imposed on financial platforms.
- **Trust and adoption** — users used to cash may distrust digital money or fear fraud.
- **Infrastructure gaps** — patchy internet, unreliable electricity, and low smartphone ownership in rural areas limit reach.
- **Cybersecurity and fraud** — digital systems are targets for hacking, scams, and identity theft.
- **Financial and digital literacy** — many users lack the skills to use apps safely.
- **Interoperability** — Bashir lists this as a major limitation; fragmented systems struggle to work together.
- **Capital and scale** — startups need funding and a large user base to become profitable.

---

## Part B — Digital Payment Systems

### 8. What are digital payment systems, and how do they function in facilitating transactions between consumers and businesses?

- **Definition:** an electronic method of transferring value from payer to payee without physical cash.
- **Participants:** the consumer (wallet/card/account), the merchant, both parties' financial institutions, and a payment network/switch that routes and settles.
- **The flow:**
  - Consumer authorises payment (card, app, or QR scan).
  - Request sent to the payment network.
  - System verifies funds and authenticates the user.
  - Network instructs the banks to move the money.
  - Merchant is credited; consumer's balance is debited.
  - **Clearing** (matching transactions) and **settlement** (moving funds) complete the process.
- In a blockchain-based system (Bashir), settlement happens through a shared ledger updated by consensus rather than a central clearing house — which makes it fast and intermediary-free.

### 9. Explain how mobile banking apps and QR-code payments operate to make transactions faster and more convenient.

- **Mobile banking apps:**
  - Connect the user's phone to their bank/wallet account over the internet through secure APIs.
  - User logs in (biometrics or PIN), then checks balances, transfers money, and pays bills in real time.
  - Convenience comes from removing branch/ATM visits.
- **QR-code payments:**
  - Encode payment information (merchant account identifier, sometimes the amount) into a Quick Response code.
  - Customer opens the wallet app, scans the merchant's code (or shows their own), confirms the amount, authorises payment.
  - Transaction routes and settles instantly through the payment network.
  - Popular in markets like Cambodia because it needs no expensive card terminal — just a printed code.
  - Cambodia's KHQR is a single interoperable standard, so one code works across all participating banks and wallets.

### 10. Compare and contrast digital payments with cash-based transactions in terms of speed, security, and convenience.

| Dimension | Digital Payments | Cash |
|---|---|---|
| **Speed** | Near-instant, even at a distance or across borders | Instant in person, but slow/impossible remotely |
| **Security** | No physical theft risk; protected by encryption and authentication, but exposed to fraud, hacking, scams | Vulnerable to physical theft and loss; no recovery if lost |
| **Convenience** | Pay anytime, anywhere; no change needed; full transaction record | Universally accepted, no device or signal needed; but bulky and hard to track |
| **Traceability** | Fully recorded — good for accounting, but reduces privacy | Anonymous — better privacy, but enables tax evasion and crime |
| **Dependency** | Needs power, internet, and a device | Works with nothing but the note itself |

- **Summary:** digital payments win on speed, record-keeping, and remote convenience; cash wins on universal acceptance, privacy, and resilience when technology fails.

### 11. How do digital payment systems improve operational efficiency and customer experience for small and large businesses?

- **Faster settlement and cash flow** — funds arrive quickly rather than after days of clearing, improving liquidity.
- **Lower handling costs** — no counting, storing, transporting, or securing cash; fewer errors.
- **Automatic record-keeping** — every transaction logged, simplifying accounting, tax, and inventory.
- **Better customer experience** — faster checkout, no need for exact change, loyalty-program support, and the ability to sell online or accept remote payment.
- **Scalability** — large businesses process huge volumes automatically; small businesses accept payment with just a QR code and a phone.
- **Data insights** — transaction data helps businesses understand customers and tailor offers.
- Bashir's point applies: a shared, agreed ledger removes "verification, reconciliation, and clearance" overhead — less manual reconciliation means more efficiency.

### 12. Discuss the importance of security measures (encryption, authentication) in maintaining trust in digital payment platforms.

- **Trust is the foundation** — users must believe their money and data are safe, or they won't use the platform.
- **Encryption** — scrambles data so that even if intercepted it cannot be read.
  - Bashir's "Cryptography layer": cryptographic protocols provide data integrity, non-repudiation, and data-origin authentication, so transactions can't be secretly altered or forged.
- **Authentication** — verifies the person initiating a transaction really is the account holder (passwords, PINs, biometrics, two-factor / one-time codes).
- **Together they provide:**
  - **Confidentiality** — only authorised parties see the data.
  - **Integrity** — the transaction isn't tampered with.
  - **Non-repudiation** — a user can't deny a transaction they signed (the role of digital signatures in blockchain).
- Without them, fraud and theft would destroy confidence and the platform would fail — which is why regulators also require strong security alongside AML/KYC.

### 13. What are the potential risks and disadvantages of relying heavily on digital payment systems?

- **Cybersecurity threats** — hacking, data breaches, phishing, account takeover.
- **System failures and outages** — if network, power, or internet goes down, payments stop entirely — a single point of failure cash doesn't have.
- **Fraud and scams** — social engineering tricks users into authorising payments; reversals can be hard.
- **Loss of privacy** — every transaction is tracked, creating surveillance and data-misuse concerns.
- **Financial exclusion of some groups** — people without smartphones, internet, or digital skills (often elderly or very poor) can be left behind in a cashless economy.
- **Over-reliance and lock-in** — dependence on a few providers concentrates risk.
- **Errors and irreversibility** — a payment sent to the wrong recipient, especially on an irreversible system like blockchain, may be impossible to recover.

### 14. Provide real-life examples of how digital payment technologies are used in Cambodia.

- **Shopping** — customers in markets, cafés, and shops scan a KHQR code with ABA Mobile, Wing, or TrueMoney to pay merchants directly, with no cash or card terminal.
- **Bill payments** — utility bills (electricity, water), phone top-ups, and school fees paid in-app through wallets and bank apps.
- **Money transfers** — workers send money to family in other provinces instantly via Wing or Bakong, which lets users of different banks and wallets transfer through one interoperable system.
- **Salary and merchant settlement** — businesses pay staff and receive customer payments digitally, reducing cash handling.
- **Standout example:** Bakong — a central-bank-operated, blockchain-based backbone interconnecting the country's financial institutions, illustrating the distributed-ledger payment infrastructure Bashir describes.

### 15. Explain the concept of a digital wallet and describe how it stores, manages, and processes financial transactions.

- **Definition:** a software application that securely stores a user's payment credentials and enables electronic transactions.
  - Bashir (blockchain context): "a wallet is a generic program that can store private keys and, based on the addresses stored within it, can compute the existing balance … by querying the blockchain."
- **Stores** — holds payment information: linked bank accounts, card details, or (in crypto wallets) the cryptographic private keys controlling the user's funds.
  - Important: a crypto wallet doesn't "hold" coins like cash; it holds the keys that authorise spending of balances recorded on the ledger.
- **Manages** — tracks balances, transaction history, and linked accounts, and secures access with PINs or biometrics.
- **Processes** — when the user pays, the wallet authenticates them, signs/authorises the transaction (a digital signature for crypto), and sends it to the payment network or blockchain for verification and settlement.
- **Examples:** mobile-money wallets (Wing, ABA) to crypto wallets (MetaMask, which Bashir cites as the developer's tool of choice).

---

## Part C — Cryptocurrency and Blockchain

### 16. What is cryptocurrency, and how does it differ from traditional money issued by governments and central banks?

- **Definition:** a digital currency secured by cryptography and (typically) issued and transferred on a decentralised blockchain rather than by a central authority.
  - Bitcoin (Satoshi Nakamoto's 2008 paper *Bitcoin: A Peer-to-Peer Electronic Cash System*) was, in Bashir's words, "the very first fully decentralized digital currency."
- **Differences from fiat money:**
  - **Issuer** — fiat is issued/controlled by a central bank; crypto is created by a protocol (e.g. mining) with no central issuer.
  - **Trust model** — fiat relies on trust in the state and banks; crypto relies on cryptography and consensus, with "no central controller in the network."
  - **Supply** — many cryptocurrencies have a fixed/capped supply (Bitcoin's 21 million); fiat supply is managed by monetary policy.
  - **Form** — crypto exists only as ledger entries; fiat exists as physical notes/coins and bank records.
  - **Volatility** — Bashir notes Bitcoin is "remarkably secure and valuable … despite being highly volatile"; fiat is comparatively stable.
  - **Reversibility/regulation** — crypto transactions are generally irreversible and harder to regulate; fiat can be reversed and is tightly regulated.
- **Middle ground:** Central Bank Digital Currency (CBDC) — Bashir's "centralized and regulated form of digital currency issued by a central bank": digital, but state-controlled.

### 17. Describe the underlying concept of blockchain technology and explain how it supports the operation and security of cryptocurrencies.

- **Bashir's two definitions:**
  - *Layman's:* "an ever-growing, secure, shared recordkeeping system in which each user of the data holds a copy of the records, which can only be updated if a majority of parties involved in a transaction agree."
  - *Technical:* "a peer-to-peer, distributed ledger that is cryptographically secure, append-only, immutable (extremely hard to change), and updateable only via consensus among peers."
- **Key properties:**
  - **Peer-to-peer** — no central controller; nodes deal directly.
  - **Distributed ledger** — every node holds a full copy.
  - **Cryptographically secure** — protected against tampering.
  - **Append-only / immutable** — data added in time order, practically impossible to alter.
  - **Updatable only via consensus** — changes require majority agreement.
- **Structure:** transactions are bundled into blocks; each block contains the hash of the previous block, chaining them so altering any past block breaks every block after it.
- **How it supports cryptocurrency:**
  - **Records ownership** without a bank — balances and transfers live on the shared ledger.
  - **Prevents double-spending** — once a coin is spent, the immutable, consensus-validated ledger reflects it everywhere.
  - **Secures transactions** with digital signatures (only the private-key holder can spend) and cryptographic hashing.
  - **Removes the need for a trusted third party** — value moves directly between peers, validated by consensus.

### 18. Discuss how cryptocurrencies can be used as an alternative for sending money, especially for cross-border remittances.

- **Problem with traditional transfers:** pass through chains of correspondent banks, take several days, charge high fees.
- **Crypto alternative:** Bashir notes blockchain "can be used to facilitate cross-border and local payments in a decentralized and secure manner," peer-to-peer and "without third-party involvement, such as by a bank."
- **Advantages for remittances:**
  - **Speed** — transfers settle in minutes rather than days.
  - **Lower cost** — removing correspondent banks and clearing houses cuts fees (Bashir's "cost-saving").
  - **24/7 availability and global reach** — no banking-hours or geographic limits.
  - **Access for the unbanked** — recipient needs only a wallet, not a bank account.
- **Drawbacks:**
  - Price **volatility** (value can change between sending and receiving).
  - Regulatory uncertainty.
  - Both parties need an exchange to convert to/from local currency.
  - Irreversibility of mistaken transfers.
- **Stablecoins (Q21)** are often used to solve the volatility problem.

### 19. Explain how workers abroad could use cryptocurrency to send money home to families in Cambodia more efficiently.

- **Baseline:** a Cambodian working abroad normally uses a slow, high-fee money-transfer operator.
- **Crypto process:**
  1. Worker buys cryptocurrency (often a stablecoin pegged to the US dollar, to avoid volatility) on an exchange using local wages.
  2. Sends it directly to the family member's wallet address — a peer-to-peer transfer that settles in minutes, at low cost, any time of day.
  3. Family in Cambodia converts it to riel or US dollars through a local exchange/wallet, or spends it directly where accepted.
- **Efficiency gains:** lower fees, faster delivery, no need for the recipient to have a bank account — consistent with Bashir on decentralisation, cost-saving, and disintermediation.
- **Stablecoin advantage:** removes the risk the amount loses value before the family receives it.
- **Practical limits:** access to a trustworthy exchange, conversion costs, regulatory rules in both countries, and digital literacy.

### 20. Compare the advantages and disadvantages of cryptocurrency versus traditional banking for international payments.

**Advantages of cryptocurrency:**
- Faster settlement (minutes vs. days).
- Lower fees (no correspondent-bank chain).
- 24/7, borderless availability.
- Accessible to the unbanked.
- Peer-to-peer, no central gatekeeper (Bashir's decentralisation/disintermediation).

**Disadvantages of cryptocurrency:**
- **Volatility** — value can swing sharply (mitigated by stablecoins).
- **Regulatory uncertainty** and possible legal restrictions.
- **Irreversibility** — mistakes or fraud are hard to undo.
- **Complexity** — managing private keys and exchanges is harder than banking; losing keys means losing funds.
- **Limited acceptance** — not all recipients can convert or use it.

**Advantages of traditional banking:**
- Stable value, strong regulation, consumer protection, reversibility/dispute resolution.
- Wide acceptance and familiarity.

**Disadvantages of traditional banking:**
- Slow, costly cross-border transfers; banking hours; exclusion of the unbanked.

- **Conclusion** (mirrors Bashir's CeFi/DeFi view): the two will likely coexist — crypto for fast, cheap transfers; banks for stability and regulatory assurance.

### 21. What are stablecoins, and how do they reduce the volatility associated with cryptocurrencies like Bitcoin?

- **Definition:** a cryptocurrency designed to hold a steady value by being pegged to a stable reference asset — usually a fiat currency (e.g. the US dollar), sometimes commodities or other assets.
  - Bashir: "stablecoins in the DeFi world are based on/pegged to the traditional financial world's assets and fiat currency," and reserves "could be kept in the CeFi traditional financial world."
- **How they reduce volatility:**
  - Each coin is backed with reserves — for every stablecoin issued, the issuer ideally holds an equivalent amount of the reference asset, so it can be redeemed 1-for-1.
  - This anchors the price and removes the wild swings of Bitcoin.
  - Makes stablecoins suitable for payments, remittances, and as a stable unit of account in DeFi.
- **Examples (Bashir):** USDC, DAI, USDT.
- **Risks (Bashir):** "liquidity risk, solvency risk, and regulatory risk."
  - Crucially: "if the demand for the stablecoin increases, there may not be enough reserve assets to meet the demand, leading to a drop in its value" — the peg can break if reserves are inadequate or not genuinely backed.

---

## Part D — Benefits, Risks, Regulation, and the Future

### 22. Discuss the major advantages of digital financial services (convenience, speed, accessibility) in modern economies.

- **Convenience** — available 24/7 from a smartphone; no branch visits, queues, or banking hours; bills, transfers, and purchases in a few taps.
- **Speed** — payments and settlements near-instant, even across borders, improving business cash flow and consumer immediacy (Bashir's "faster dealings").
- **Accessibility / inclusion** — anyone with a phone can access services, bringing unbanked and rural populations into the formal economy.
- **Cost-saving** — lower fees and overheads (Bashir's "cost-saving" through removing intermediaries) benefit users and providers.
- **Transparency and record-keeping** — automatic, tamper-resistant records aid accounting, audit, and trust (Bashir's "transparency and trust" and "immutability").
- **Economic growth** — easier payments and credit stimulate commerce, entrepreneurship, and productivity.

### 23. Identify and explain the risks associated with financial technologies (cybersecurity, fraud, system failures).

- **Cybersecurity threats** — hacking, malware, data breaches, and phishing target systems holding money and personal data.
  - Bashir notes attacks like the "sandwich attack" and DeFi exploits — even advanced systems are targeted.
- **Fraud** — scams, social engineering, identity theft, and fake apps; irreversible transactions make recovery hard.
- **System failures** — outages of internet, power, or infrastructure can halt payments — a single point of failure absent in cash.
- **Operational and key-management risk** — in crypto, losing a private key means permanently losing funds.
- **Regulatory and compliance risk** — weak AML/KYC controls invite money laundering and legal penalties.
- **Stablecoin and market risk** — liquidity, solvency, and regulatory risks can break a stablecoin's peg (Bashir).
- **Privacy risk** — concentrated transaction data can be misused or leaked.
- **Mitigation:** strong encryption, authentication, regulation, user education, and system redundancy.

### 24. Analyse the legal and regulatory challenges governments face with new financial technologies such as cryptocurrencies.

- **Bashir's core point:** "due to its decentralized nature, regulation is almost impossible on blockchain," and the absence of a regulatory authority "is an inhibiting factor for many consumers," who lose the assurance that "if something goes wrong they can hold someone accountable."
- **Main challenges:**
  - **Decentralisation and jurisdiction** — with no central issuer and a global, borderless network, it's unclear which country's laws apply or who is accountable.
  - **Anti-money-laundering and terrorism financing** — pseudonymous transactions can be misused. Governments respond by legalising and supervising exchanges (e.g. US Bank Secrecy Act), requiring AML, Counter-Financing of Terrorism (CFT), and strict record-keeping/reporting.
  - **Consumer protection** — volatility, scams, and irreversible transactions expose consumers, with no deposit insurance or dispute mechanism.
  - **Taxation** — tracking and taxing crypto gains is difficult.
  - **Financial stability** — large, unbacked stablecoins or crypto markets could pose systemic risk.
  - **Balancing innovation and control** — over-regulation stifles innovation; under-regulation invites abuse.
- **Government response:** exchange licensing, AML/KYC rules, stablecoin regulation, and issuing CBDCs — a "centralized and regulated form of digital currency" that captures the benefits while keeping state oversight.

### 25. Looking ahead, what future trends do you expect in FinTech, and how might they transform financial services in Cambodia over the next decade?

- **Mainstreaming of blockchain applications** — Bashir notes DeFi, NFTs, and tokenisation are already used by millions and expects DeFi to "stabilize into a mature mainstream technology," with more focus on regulation and standardisation; expect asset tokenisation and smart-contract services to spread.
- **Central Bank Digital Currencies (CBDCs)** — Cambodia is already a pioneer with Bakong; expect deeper adoption, full interoperability, and possibly cross-border CBDC links for cheaper remittances.
- **Greater interoperability and scalability** — Bashir highlights layer-2/multi-chain solutions and zero-knowledge proofs as the response to scalability and privacy limits, making payments faster, cheaper, and more private.
- **AI- and data-driven services** — smarter credit scoring, fraud detection, and personalised products.
- **Deeper financial inclusion** — continued growth of mobile money and QR payments brings more rural and unbanked Cambodians into the formal economy.
- **Stronger regulation and security** — Bashir: "further maturity is required, especially from a regulation and security perspective"; Cambodia will likely develop clearer FinTech, crypto, and consumer-protection rules.
- **CeFi–DeFi convergence** — traditional banks and FinTech/blockchain services will increasingly connect rather than compete in isolation.
- **For Cambodia specifically:** the next decade will likely bring a largely cashless, mobile-first economy on interoperable rails like Bakong and KHQR, with cheaper cross-border remittances, wider credit access, and growing — but still maturing — crypto and digital-asset regulation.
