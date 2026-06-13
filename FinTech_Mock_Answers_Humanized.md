# FinTech Mock Questions — Model Answers

*A note on sources: the blockchain, cryptocurrency, and stablecoin answers lean on Imran Bashir's* Mastering Blockchain *(4th ed., Packt, 2023). The broader FinTech and Cambodia-specific material comes from general course notes, since Bashir's book really only deals with blockchain.*

---

## Part A — Financial Technology (FinTech) Fundamentals

### 1. What is FinTech, and how has it changed the way individuals and businesses access and use financial services?

FinTech is really just shorthand for using modern software, the internet, and mobile devices to deliver financial services — and to do it better, faster, and more cheaply than the old way. It stretches across a lot of ground: mobile payments, digital wallets, online lending, robo-advisors, insurance tech (people call it "insurtech"), and blockchain-based finance.

The way I'd describe its impact, it has changed everyday financial life in about three big ways. The first is access. You used to have to walk into a branch to do anything; now the bank basically lives on your phone. Opening an account, sending money, paying a bill, even investing — all of it can happen from wherever you are, as long as you've got a connection. The second is cutting out the middleman. A lot of services that used to need a bank or a broker or a clearing house sitting in the middle can now happen directly between two people, which strips out cost and hassle. Bashir makes this point at the technical level when he describes a blockchain as a platform where peers can exchange value "without the need for a centrally trusted arbitrator." The third is speed and personalisation — FinTech apps use data and automation to make decisions on the spot (think instant loan approval) and tailor things in a way banks were always too slow to manage. For businesses, the payoff is lower transaction costs, money that settles faster, and the ability to reach customers who never had a bank account in the first place.

### 2. How have FinTech solutions improved the efficiency, speed, and accessibility of financial transactions compared to traditional banking?

Traditional banking is built on layers of middlemen — correspondent banks, clearing houses, reconciliation steps — and every one of those layers adds time and cost. Bashir puts it well: a shared ledger means the system "does not require a lengthy process of verification, reconciliation, and clearance because a single version of agreed-upon data is already available," which is exactly where the speed and the savings come from. FinTech takes that same idea and runs with it.

On efficiency, software does the work that used to fall on staff. A digital loan or payment gets processed by code rather than by a person shuffling paperwork, so there's less overhead and fewer mistakes. On speed, things that used to drag on for days — cheque clearing, wire transfers — now happen almost instantly. Mobile payments settle in seconds, and a cross-border transfer that once took three to five days can be done in minutes. And on accessibility, the difference is hard to overstate: a branch has fixed hours and a fixed location, but an app is in your pocket 24/7. For people in rural areas, or anyone who never qualified for a bank account, that's the single biggest change of all.

### 3. Discuss the role of mobile applications and internet technologies in the growth and adoption of FinTech in developing countries such as Cambodia.

In a lot of developing countries, phones spread much faster and much further than bank branches ever did. Cambodia is a clear case — very high mobile and internet penetration, but historically pretty thin traditional-bank coverage. So the phone, not the branch, became the front door to financial services. People sometimes call it a "mobile-first" market, though "mobile-only" is closer to the truth for many users.

What makes this work economically is that serving a customer through an app costs almost nothing. That's the whole reason it suddenly makes sense to reach low-income and rural users a brick-and-mortar bank could never have served at a profit. Internet technologies — cloud computing, APIs, QR codes, real-time payment rails — let providers launch quickly and plug into one another. In Cambodia you can see it in services like Wing, TrueMoney, ABA Mobile, ACLEDA Mobile, and Pi Pay, plus the Bakong system the National Bank of Cambodia runs and the national KHQR code standard. Bakong is worth flagging because it's actually built on the same distributed-ledger technology Bashir's textbook spends its chapters on.

### 4. In what ways has FinTech contributed to financial inclusion, especially for rural or underserved areas?

Financial inclusion is about getting people who were "unbanked" or "underbanked" into a position where they can use genuinely useful, affordable financial services. FinTech pushes this forward on a few fronts.

For one, it lowers the bar to get started — opening a digital wallet usually takes a phone number and some basic ID, not a minimum deposit and a trip to a branch. It also extends reach into places banks never went: mobile coverage exists where branches don't, so a farmer out in a remote province can receive payments, save, and send money. It's cheaper, too — moving money digitally costs far less than handling cash or travelling to a distant bank. There's a knock-on benefit around credit: transaction and payment history gives lenders something to assess, so people with no formal credit record can start getting access to small loans. And agent networks — local shops acting on a provider's behalf for cash-in and cash-out — bridge the gap between physical cash and digital money out in rural areas.

All of this ties back to Bashir's broader theme that decentralised, shared systems cut the need for expensive intermediaries. That's precisely what makes serving low-value, rural customers viable in the first place.

### 5. Provide detailed examples of commonly used FinTech services in Cambodia and explain how they benefit users and providers.

A few stand out. The mobile-money and e-wallet apps — Wing, TrueMoney, ABA Mobile, ACLEDA Mobile — let people store money, send it to others, top up phone credit, and pay merchants. For the user that means convenience and no need for a full bank account; for the provider it's cheap customer acquisition plus income from fees and float.

Then there's QR-code payments under the KHQR standard. The clever part is that one national QR standard means a customer from any participating bank or wallet can scan a single code to pay any merchant. The user gets fast, cashless payment with no card machine involved, and the merchant gets something cheaper than a card terminal with no cash to handle or worry about.

Bakong, run by the National Bank of Cambodia, sits underneath a lot of this — a central, interoperable, blockchain-based payment backbone that lets different banks and wallets move money to each other instantly. Users can send across institutions for free or close to it, and providers get to share infrastructure instead of each building their own. On top of that there are digital lending and savings apps offering small loans and savings products over the phone, which give users fast credit access and give providers data-driven risk assessment and scale.

The common thread: users win on convenience, speed, and inclusion, and providers win on lower operating costs, fee income, and access to a much bigger market.

### 6. Analyse the impact of FinTech on traditional banks — competitor, collaborator, or both?

It's both, and honestly it's been drifting more and more toward collaborator.

As competitors, FinTech firms go straight for the most profitable, customer-facing slices of banking — payments, transfers, lending — usually with something cheaper, faster, and easier to use. That eats into bank fee income and, just as importantly, into the bank's relationship with the customer. But as collaborators, the two sides turn out to need each other. Banks have the things FinTechs often lack: licences, capital, regulatory know-how, and big existing customer bases. FinTechs have the technology and the speed. So you get partnership — banks building their own apps, buying or investing in startups, connecting through shared rails. Bakong is the obvious Cambodian example, with the central bank providing shared infrastructure that banks and wallets all plug into.

Bashir frames the underlying technology the same way. Blockchain *could* disintermediate banks, but he also points to a likely "collaborative future where connectivity between CeFi [centralised finance] and DeFi exists." The realistic outcome is coexistence and convergence — the line between "bank" and "FinTech" just keeps blurring.

### 7. What are the main challenges or limitations FinTech companies face in emerging markets?

Quite a few, and they tend to reinforce each other. Regulation and licensing is a big one — the rules are often unclear or still being written, and FinTechs have to satisfy anti-money-laundering (AML) and know-your-customer (KYC) requirements regardless. Bashir flags regulation as one of blockchain's hardest problems, and notes that authorities push AML and Counter-Financing-of-Terrorism (CFT) rules onto financial platforms.

Beyond that, there's the matter of trust: people used to cash may simply distrust digital money or worry about fraud. Infrastructure can be patchy too — unreliable internet, unreliable electricity, and low smartphone ownership in rural areas all cap how far a service can reach. Cybersecurity and fraud are a constant, since digital systems are obvious targets for hacking, scams, and identity theft. There's also a literacy gap — plenty of users don't yet have the skills to use these apps safely. Interoperability is another sticking point; Bashir lists it as a major limitation, because fragmented systems make it hard for services to work together. And finally, capital and scale: a startup needs both funding and a large user base before it ever turns a profit.

---

## Part B — Digital Payment Systems

### 8. What are digital payment systems, and how do they function in facilitating transactions between consumers and businesses?

A digital payment system is just an electronic way of moving value from a payer to a payee without any physical cash changing hands. It works through a chain of participants: the consumer (with a wallet, card, or bank account), the merchant, both of their financial institutions, and a payment network or switch that routes the transaction and settles it.

The flow goes roughly like this. The consumer authorises a payment — by card, app, or QR scan. That request gets sent to the payment network. The system checks the funds are there and confirms the user is who they say they are. The network then tells the banks to move the money, the merchant gets credited, and the consumer's balance gets debited. Behind the scenes, two final steps wrap it up: clearing (matching the transactions) and settlement (actually moving the funds). In a blockchain-based system, as Bashir explains, that settlement happens through a shared ledger updated by consensus rather than through a central clearing house — which is the whole reason it's fast and free of intermediaries.

### 9. Explain how mobile banking apps and QR-code payments operate to make transactions faster and more convenient.

Mobile banking apps connect your phone to your bank or wallet account over the internet through secure APIs. You log in — usually with a fingerprint, face, or PIN — and from there you can check balances, move money, and pay bills in real time. The convenience is simply that you never have to visit a branch or an ATM to do any of it.

QR-code payments work by packing the payment information — the merchant's account identifier, and sometimes the amount — into a Quick Response code. You open your wallet app, scan the merchant's code (or show your own to be scanned), confirm the amount, and authorise it. The transaction then routes and settles instantly through the payment network. The reason QR has taken off in markets like Cambodia is that it needs no expensive card terminal at all — just a printed code — which makes it cheap for a small merchant and instant for the customer. And because Cambodia's KHQR is a single interoperable standard, one code works across every participating bank and wallet.

### 10. Compare and contrast digital payments with cash-based transactions in terms of speed, security, and convenience.

The two have genuinely different strengths, so it's worth laying them side by side:

| Dimension | Digital Payments | Cash |
|---|---|---|
| **Speed** | Near-instant, even at a distance or across borders | Instant in person, but slow or impossible remotely |
| **Security** | No physical theft risk; protected by encryption and authentication, but exposed to fraud, hacking, and scams | Vulnerable to physical theft and loss, with no recovery once it's gone |
| **Convenience** | Pay anytime, anywhere; no change needed; full transaction record | Universally accepted, needs no device or signal — but bulky and hard to track |
| **Traceability** | Fully recorded, which helps accounting but reduces privacy | Anonymous, which is better for privacy but enables tax evasion and crime |
| **Dependency** | Needs power, internet, and a device | Works with nothing but the note itself |

The short version: digital payments win on speed, record-keeping, and remote convenience, while cash holds onto its advantages in universal acceptance, privacy, and sheer resilience when the technology falls over.

### 11. How do digital payment systems improve operational efficiency and customer experience for small and large businesses?

The biggest gain is around money and time. Funds settle quickly instead of sitting in clearing for days, which is a real boost to cash flow and liquidity. Handling costs drop too — there's no cash to count, store, transport, or guard, and fewer errors creep in. Every transaction gets logged automatically, which makes accounting, tax, and inventory management far less painful.

On the customer side, checkout is faster, nobody's hunting for exact change, loyalty programs are easy to bolt on, and a business can sell online or take payment remotely. It scales nicely in both directions: a large business can process enormous volumes automatically, while a small one can accept payment with nothing more than a QR code and a phone. And all that transaction data gives businesses a clearer read on their customers, so they can tailor what they offer.

Bashir's point about a shared, agreed ledger removing "verification, reconciliation, and clearance" overhead applies squarely here — the less manual reconciliation a business has to do, the more efficient it gets.

### 12. Discuss the importance of security measures (encryption, authentication) in maintaining trust in digital payment platforms.

Trust is the whole foundation. People have to believe their money and their data are safe, or they simply won't use the platform. Two security pillars carry most of that weight.

Encryption scrambles data so that even if someone intercepts it, they can't read it. Bashir makes the same point about blockchain in his "Cryptography layer" — cryptographic protocols deliver data integrity, non-repudiation, and data-origin authentication, which together stop transactions from being secretly altered or forged. Authentication is the other pillar: it confirms that the person starting a transaction really is the account holder, whether through a password, a PIN, biometrics, or a two-factor or one-time code.

Put together, these give you confidentiality (only authorised parties see the data), integrity (the transaction isn't tampered with), and non-repudiation (a user can't deny a transaction they signed — which is exactly the job digital signatures do in blockchain). Without them, fraud and theft would gut user confidence and the platform would collapse. That's also why regulators insist on strong security right alongside AML and KYC controls.

### 13. What are the potential risks and disadvantages of relying heavily on digital payment systems?

There's a real downside to putting all your eggs in this basket. Cybersecurity threats are constant — hacking, data breaches, phishing, account takeover. System failures are arguably worse: if the network, the power, or the internet goes down, payments just stop, which is a single point of failure that cash simply doesn't have. Fraud and scams are a persistent problem, because social engineering can trick people into authorising payments themselves, and reversing those can be hard or impossible.

There's also a privacy cost — every transaction is tracked, which raises real surveillance and data-misuse concerns. And there's an inclusion problem hiding in plain sight: people without a smartphone, internet, or digital skills — often the elderly or the very poor — risk being left behind in a fully cashless economy. Lean too hard on a handful of providers and you concentrate risk in a few points of failure. Finally, errors can be unforgiving: a payment sent to the wrong recipient, especially on an irreversible system like a blockchain, may be impossible to claw back.

### 14. Provide real-life examples of how digital payment technologies are used in Cambodia.

You see it everywhere day to day. Shopping is the obvious one — in markets, cafés, and shops, customers scan a KHQR code with ABA Mobile, Wing, or TrueMoney to pay the merchant directly, no cash and no card terminal. Bill payments are just as common: utility bills like electricity and water, phone top-ups, and even school fees get paid in-app through wallets and bank apps. Money transfers are big too — workers send money home to family in other provinces instantly through Wing, or via Bakong, which lets people on different banks and wallets transfer to each other through one interoperable system. And on the business side, salary and merchant settlement increasingly happen digitally, with companies paying staff and taking customer payments without all the cash handling.

Bakong is the standout national example here — a central-bank-operated, blockchain-based backbone that interconnects the country's financial institutions. It's a textbook illustration, almost literally, of the distributed-ledger payment infrastructure Bashir describes.

### 15. Explain the concept of a digital wallet and describe how it stores, manages, and processes financial transactions.

A digital wallet is a piece of software that securely holds your payment credentials and lets you transact electronically. In Bashir's blockchain context, "a wallet is a generic program that can store private keys and, based on the addresses stored within it, can compute the existing balance … by querying the blockchain." A consumer wallet runs on the same idea but covers more ground.

On the storing side, it holds your payment information — linked bank accounts, card details, or, in a crypto wallet, the cryptographic private keys that control your funds. This is the part people often get wrong: a crypto wallet doesn't actually "hold" coins the way a leather wallet holds cash. It holds the keys that authorise you to spend balances recorded on the ledger. On the managing side, it keeps track of your balances, transaction history, and linked accounts, and locks access behind a PIN or biometrics. And on the processing side, when you make a payment the wallet authenticates you, signs or authorises the transaction (with a digital signature, in the crypto case), and sends it off to the payment network or blockchain to be verified and settled.

Examples run from mobile-money wallets like Wing and ABA all the way to crypto wallets like MetaMask, which Bashir cites as the developer's tool of choice.

---

## Part C — Cryptocurrency and Blockchain

### 16. What is cryptocurrency, and how does it differ from traditional money issued by governments and central banks?

A cryptocurrency is a digital currency secured by cryptography and — usually — issued and moved around on a decentralised blockchain rather than by any central authority. Bitcoin, which Satoshi Nakamoto introduced in the 2008 paper *Bitcoin: A Peer-to-Peer Electronic Cash System*, was in Bashir's words "the very first fully decentralized digital currency."

It parts ways with traditional, or "fiat," money on several fronts. The issuer is different: fiat is created and controlled by a government's central bank, while a cryptocurrency is created by a protocol — through mining, for instance — with no central issuer at all. The trust model is different: fiat depends on trust in the state and the banks, whereas crypto rests on cryptography and consensus among peers, with "no central controller in the network." Supply works differently too — many cryptocurrencies have a fixed or algorithmically capped supply (Bitcoin's famous 21 million), while fiat supply gets managed through monetary policy. There's a difference in form, since crypto exists purely as entries on a distributed ledger while fiat exists as physical notes and coins plus bank records. They behave differently as well: Bashir notes Bitcoin is "remarkably secure and valuable … despite being highly volatile," where fiat is comparatively stable. And finally, crypto transactions are generally irreversible and harder to regulate, while fiat ones can be reversed and are tightly regulated.

Sitting between the two is the Central Bank Digital Currency (CBDC), which Bashir describes as "a centralized and regulated form of digital currency issued by a central bank" — digital, but still firmly under state control.

### 17. Describe the underlying concept of blockchain technology and explain how it supports the operation and security of cryptocurrencies.

Bashir offers two standard definitions, and they complement each other nicely. The layman's version: blockchain is "an ever-growing, secure, shared recordkeeping system in which each user of the data holds a copy of the records, which can only be updated if a majority of parties involved in a transaction agree." The technical version: it's "a peer-to-peer, distributed ledger that is cryptographically secure, append-only, immutable (extremely hard to change), and updateable only via consensus among peers."

Unpacking the key properties: it's peer-to-peer (no central controller — nodes deal with each other directly), it's a distributed ledger (every node holds a full copy), it's cryptographically secure (protected against tampering), it's append-only and immutable (data can only be added in time order and is practically impossible to alter after the fact), and it's updatable only via consensus (changes require agreement among the majority of nodes). Structurally, transactions get bundled into blocks, and each block carries the hash of the block before it, chaining them together so that tampering with any past block would break every block that follows.

All of that directly props up cryptocurrency. It records ownership without a bank, since balances and transfers live on the shared ledger. It prevents double-spending — once a coin is spent, the immutable, consensus-validated ledger reflects that everywhere. It secures transactions with digital signatures, so only the private-key holder can spend, and with cryptographic hashing. And it removes the need for a trusted third party, letting value move directly between peers and be validated by consensus.

### 18. Discuss how cryptocurrencies can be used as an alternative for sending money, especially for cross-border remittances.

Traditional cross-border transfers crawl through chains of correspondent banks, take several days, and charge steep fees. Cryptocurrencies offer a different route. As Bashir puts it, a blockchain "can be used to facilitate cross-border and local payments in a decentralized and secure manner," peer-to-peer and "without third-party involvement, such as by a bank."

For remittances specifically, the appeal is fairly concrete: transfers settle in minutes rather than days; removing the correspondent banks and clearing houses cuts the fees (Bashir's "cost-saving" benefit again); there are no banking-hours or geographic limits, so it's 24/7 and global; and the recipient only needs a wallet, not a bank account, which opens it up to the unbanked.

It's not without drawbacks, though. There's price volatility — the value can shift between sending and receiving — along with regulatory uncertainty, the need for both parties to reach an exchange to convert in and out of local currency, and the fact that a mistaken transfer can't be undone. Stablecoins (which Q21 covers) are the usual fix for the volatility problem in remittances.

### 19. Explain how workers abroad could use cryptocurrency to send money home to families in Cambodia more efficiently.

Picture a Cambodian working overseas. Normally they'd use a money-transfer operator that's slow and takes a hefty cut. With cryptocurrency, the process could look like this: first, the worker uses their local wages to buy crypto on an exchange — often a stablecoin pegged to the US dollar, specifically to dodge volatility. Then they send it straight to their family member's wallet address; that's a peer-to-peer transfer that settles in minutes, costs very little, and can happen at any hour. Finally, the family back in Cambodia converts it to riel or US dollars through a local exchange or wallet, or just spends it directly wherever it's accepted.

The efficiency gains are lower fees, faster delivery, and no requirement for the recipient to have a traditional bank account — all of which line up with Bashir's points about decentralisation, cost-saving, and disintermediation. Using a stablecoin matters here because it removes the risk that the amount loses value before the family ever receives it. The practical limits are real, though: you need access to a trustworthy exchange, there are conversion costs, the regulatory rules in both countries apply, and a certain amount of digital literacy is required on both ends.

### 20. Compare the advantages and disadvantages of cryptocurrency versus traditional banking for international payments.

Cryptocurrency's advantages are mostly about speed and reach. Settlement is fast (minutes versus days), fees are lower because there's no chain of correspondent banks, and it's available 24/7 across borders. It's accessible to the unbanked, and it's peer-to-peer with no central gatekeeper — Bashir's decentralisation and disintermediation themes once more.

Its disadvantages are equally real. Volatility means value can swing sharply (though stablecoins mitigate this). There's regulatory uncertainty and the possibility of outright legal restrictions. Irreversibility makes mistakes and fraud hard to undo. There's genuine complexity — managing private keys and exchanges is harder than ordinary banking, and losing your keys means losing your funds. And acceptance is still limited, since not every recipient can convert or use it.

Traditional banking, by contrast, offers stable value, strong regulation, consumer protection, and proper reversibility and dispute resolution, on top of wide acceptance and familiarity. Its weaknesses are the slow, costly cross-border transfers, the banking hours, and the way it leaves the unbanked out.

The honest conclusion mirrors Bashir's CeFi/DeFi view: the two are likely to coexist, with crypto handling the fast, cheap transfers and banks supplying the stability and the regulatory assurance.

### 21. What are stablecoins, and how do they reduce the volatility associated with cryptocurrencies like Bitcoin?

A stablecoin is a cryptocurrency built to hold a steady value by being pegged to a stable reference asset — usually a fiat currency like the US dollar, though sometimes commodities or other assets. Bashir explains that "stablecoins in the DeFi world are based on/pegged to the traditional financial world's assets and fiat currency," and that their reserves "could be kept in the CeFi traditional financial world."

The way they tame volatility is by backing each coin with reserves. For every stablecoin issued, the issuer ideally holds an equivalent amount of the reference asset, so the coin can always be redeemed one-for-one. That anchors the price and strips out the wild swings you see with Bitcoin, which is what makes stablecoins workable for payments, remittances, and as a stable unit of account inside DeFi. Bashir points to USDC, DAI, and USDT as common examples.

That said, he's clear they carry their own risks — "liquidity risk, solvency risk, and regulatory risk." The crucial catch is that "if the demand for the stablecoin increases, there may not be enough reserve assets to meet the demand, leading to a drop in its value." In other words, the peg can break if the reserves are inadequate or were never genuinely there to begin with.

---

## Part D — Benefits, Risks, Regulation, and the Future

### 22. Discuss the major advantages of digital financial services (convenience, speed, accessibility) in modern economies.

Start with convenience: these services are available 24/7 from a smartphone, with no branch visits, no queues, and no banking hours to work around — bills, transfers, and purchases all happen in a few taps. Speed is close behind, since payments and settlements are near-instant even across borders, which improves cash flow for businesses and gives consumers immediacy. Bashir's "faster dealings" benefit — losing the reconciliation and clearance delay — applies directly.

Then there's accessibility and inclusion: anyone with a phone can reach financial services, which pulls unbanked and rural populations into the formal economy. There's cost-saving too — lower fees and overheads (Bashir's "cost-saving" through removing intermediaries) that benefit users and providers alike. Transparency and record-keeping come along for the ride, since automatic, tamper-resistant records aid accounting, audit, and trust — Bashir's "transparency and trust" and "immutability" benefits. And taken together, easier payments and easier credit stimulate commerce, entrepreneurship, and productivity, which feeds economic growth across the board.

### 23. Identify and explain the risks associated with financial technologies (cybersecurity, fraud, system failures).

Cybersecurity threats sit at the top — hacking, malware, data breaches, and phishing all target the digital systems holding money and personal data. Bashir spends real time on blockchain security and points to attacks like the "sandwich attack" and various DeFi exploits, which shows even advanced systems get targeted. Fraud is the next layer: scams, social engineering, identity theft, and fake apps trick users into losing money, and irreversible transactions make recovery hard.

System failures are their own category — an outage of internet, power, or platform infrastructure can halt payments entirely, a single point of failure that cash never had. In crypto there's also operational and key-management risk, where losing a private key means losing your funds permanently. Regulatory and compliance risk matters too: weak AML/KYC controls invite money laundering and the legal penalties that follow. There's stablecoin and market risk, since (as Bashir notes) liquidity, solvency, and regulatory risks can break a peg. And there's privacy risk, with concentrated transaction data liable to be misused or leaked.

Mitigating all this comes down to strong encryption, solid authentication, sensible regulation, user education, and building redundancy into the system.

### 24. Analyse the legal and regulatory challenges governments face with new financial technologies such as cryptocurrencies.

Bashir is blunt that regulation is one of blockchain's hardest problems: "due to its decentralized nature, regulation is almost impossible on blockchain," and the absence of a regulatory authority "is an inhibiting factor for many consumers," who lose the comfort of knowing that "if something goes wrong they can hold someone accountable."

From there the challenges stack up. There's decentralisation and jurisdiction — with no central issuer and a global, borderless network, it's genuinely unclear whose laws apply or who's accountable. There's anti-money-laundering and terrorism financing, since pseudonymous transactions can be abused; Bashir notes governments respond by legalising and supervising exchanges (under the US Bank Secrecy Act, for example), requiring AML, Counter-Financing of Terrorism (CFT), and strict record-keeping and reporting. There's consumer protection, because volatility, scams, and irreversible transactions leave consumers exposed with no deposit insurance and no dispute mechanism. Taxation is awkward too — tracking and taxing crypto gains is difficult. There's financial stability, where large, unbacked stablecoins or crypto markets could pose systemic risk. And underneath all of it is the balancing act between innovation and control: over-regulate and you smother something useful; under-regulate and you invite abuse.

Governments are responding with exchange licensing, AML/KYC rules, stablecoin regulation, and by issuing their own CBDCs — a "centralized and regulated form of digital currency" that captures the benefits of digital money while keeping state oversight intact.

### 25. Looking ahead, what future trends do you expect in FinTech, and how might they transform financial services in Cambodia over the next decade?

Drawing on Bashir's outlook and the current direction of travel, a few trends look likely.

Blockchain applications should keep moving into the mainstream — Bashir notes that DeFi, NFTs, and tokenisation are already used by millions, and he expects DeFi to "stabilize into a mature mainstream technology" within a few years, with more attention paid to regulation and standardisation. Expect asset tokenisation and smart-contract-based services to spread. Central Bank Digital Currencies will likely deepen too, and Cambodia is already a pioneer here with Bakong; I'd expect wider adoption, full interoperability, and possibly cross-border CBDC links for cheaper remittances. There should be greater interoperability and scalability as well — Bashir highlights layer-2 and multi-chain solutions and zero-knowledge proofs as the answer to blockchain's scalability and privacy limits, and those will make digital payments faster, cheaper, and more private.

On top of that, AI- and data-driven services point toward smarter credit scoring, better fraud detection, and more personalised products. Financial inclusion should keep deepening as mobile money and QR payments pull more rural and unbanked Cambodians into the formal economy. Regulation and security will mature alongside it — as Bashir stresses, "further maturity is required, especially from a regulation and security perspective," so Cambodia will probably develop clearer FinTech, crypto, and consumer-protection rules. And CeFi and DeFi will keep converging, with traditional banks and blockchain services connecting rather than competing in isolation.

For Cambodia specifically, the next decade most likely brings a largely cashless, mobile-first economy running on interoperable rails like Bakong and KHQR — with cheaper cross-border remittances, wider access to credit, and crypto and digital-asset regulation that's growing up, even if it's still a work in progress.
