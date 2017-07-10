# Digital Dollar - Asset-backed blockchain Token - Technical Workshops

## Summary

Project initiation is through a series of workshops attended by Blockchain experts in Sydney to address the **design options, trade-offs (business implications) and the technical challenges** of issuing a digital dollar (or any fiat currency, or asset-backed token) on blockchain/distributed ledger technology.

The first application is the digital Australian dollar - for practical reasons.  Such reasons include a relatively known legal landscape and a strong local appetite for this technology to be realized.

##Background

The design of this system is guided by the **immediate goal of creating a (Australian) blockchain dollar**, however the principles of these designs should apply to any other fiat currency and, in fact - **_any blockchain assets backed by - or redeemable for - 'real world' securities/assets_**.

**The majority of fiat (e.g. dollar) transactions and custodial funds are _already_ 'digital'**- i.e. they merely exist in bank computers/databases and have enjoyed the benefits of digitisation already for a long time.

**Virtual currencies have also existed for some time** - such as 'Linden Dollars' in the game _Second Life_, or to some extent loyalty point schemes.  However, since the economics, rules and value of these are entirely dependent on one organization (or small group of organizations) - their utility is limited.  The rules may change, the company may discontinue the program, confiscate or dilute the points at any time.  Their longevity is tied to the company's and its systems.  Additionally there are very few ways in which to interact with these toy credits, hence the economies around them have had very limited scope.

Crypto-currencies - by contrast - rely on game theory, mathematics (particularly cryptography) - and resources such as electricity - to create scarcity without However tokenizing these on a blockchain allows these assets - to become **smart, programmable property** and to interact with other financial instruments in a much more fluid and flexible manner, and in ways that are only know being invented.

Innovations and advantages that previously applied only to crypto-currencies and abstract tokens can now be applied to traditional currencies and assets with direct implications in the traditional financial system, _blurring the distinction between 'on-chain' and 'off-chain'_.

There are many different solutions for creating a digital currency as they are all solving different problems. 

Bitcoin is designed to work in an untrusted (potentially adversarial) environment where a third party is unavailable or cannot be trusted to perform the transaction on behalf of two participants.  The network takes the role of this trusted third party.  The identity of the participants _may_ be unknown, however - once revealed - there is a permanently transparent record for that identity which, which may also uncover information about its counter-parties and about other transactions.  Therefore in some instances, the (unmodified) Bitcoin network is likely too transparent for many real-world applications, especially in the world of traditional finance.

Ethereum is designed to be a general computing platform that operates in an open, untrusted (potentially adversarial) environment.  Ethereum allows more complex code (known as contracts) to execute, by removing the need for the counter parties to trust each others' execution and trust the Ethereum blockchain's execution instead..  Ethereum transactions at a basic level are also transparent to most participants in a given Ethereum blockchain instance, however there is scope for more complex data and logic to be included in transactions, which may allow finer-grained control of access to potentially sensitive data.

Monero - unlike Ethereum - does not offer a 'trustless' execution environment, but offers an improved privacy model.  In Monero, the participants in a transaction know its details (and can use the blockchain to prove it), however third parties are unable to decode these details, despite the data being available to them.  This employs 'ring signature' technology.  Additionally a third party may be provided a key to view the details of an otherwise opaque transaction, e.g. for auditing purposes. 

Z-Cash is one of several systems to employ 'zero knowledge proofs' (zk-SNARKS) - which allows statements (proofs) to be asserted as correct or incorrect without revealing the underlying data for the assertions.

Tether is a company that issues tokens (USDT, EURT, GBPT) which are backed by currency deposits.  On-ramps and off-ramps to the Tether bank accounts require AML/KYC.  The tokens are issued in a meta-data on the Bitcoin blockchain via Omnilayer, which allows tokens to be issued on top of bitcoin transactions.  The total supply can be interregated (although somewhat clumsily) from analysis of the bitcoin blockchain, and the supposed balance of the bank account(s) is published by Tether to assure the public that all tokens are backed by their equivalent fiat currency.

However, the _current_ smart-contract capabilities, settlement times and throughput capabilities of the Bitcoin blockchain have been overtaken by other systems and the technical capabilities are generally limited.  Additionally Tether suffers from being closely associated with one particular exchange (BitFinex), so that _perceived_ counterparty risk related to the exchange also have - at times - had notable effects on the value of the Tether peg to its currency counterpart.

**Some high level goals include:**

 - Enable smart-contract code to deal with and manipulate 'real-world' assets backed by currency in the traditional financial system - blurring the distinction between what was previously _'on chain'_ vs _'off chain'_
 - Allow markets (exchanges) to offer trading between crypto-assets, dollars, fiat currencies and other 'real-world' assets, _without major changes to their platform_
 - Allow DEXs (decentralized exchanges) to handle trading and order matching of fiat and other traditional assets
 - Allow traditional financial institutions access to benefits of blockchain technology, such as real-time auditing and faster settlement 
 - Allow an ecosystem of custodial institutions ("Deposit Receipt Gateways") to evolve and compete, based on capabilities and trust
 - Improve liquidity and ease of settlement for the emerging world of fintech startups who wish to settle/transact in instruments *other than existing crypto-currencies*
 - Provide a minimum-viable product (MVP) base platform: consisting of a design model, and a code framework which can be used to **kick-start real-world implementations**
 - Open technology - use _existing open technology platforms and IP_, especially where the roadmap of those technologies aligns with the goals of this project, or whose limitations are known to be resolvable in future.  Similarly the results of this work and the possibility to improve it should be open to anyone.
 - Low barriers to entry: becoming a participant in the system should be easy, possible over the internet, and not require the permission of others.  As an example: transacting in the system may require only ownership of tokens.  Custodial gateway participants (by nature) have more work to do in their roles - but can become general participants immediately. 

Examples of digital fiat-backed blockchain assets exist already, both privately issued (such as Tether - i.e. USDT, EURT), as well as private 'consortium' efforts - usually in the form of closed-door trials and experiments by players that include:
* The Bank of England (BoE)
* The People's Bank of China
* Monetary Authority of Singapore (MAS) - Project Ubin
* Bank of Canada's Project Jasper
* Santander Group of banks
* Barclays Bank
* Commonwealth Bank of Australia (CBA)


The goal of the workshop is to survey the wider landscape of emergen

## Problem statement
*How to tokenise dollars (or fiat currency) to create blockchain assets that can be transacted within distributed economies, across financial institutions and within smart-contracts*

## Requirements


## Terms

| **GLOSSARY TERM** | Description and Usage in our context|
| DR | "Depository Receipts" (custody tokens) provided by a participant, backed by assets (e.g. dollars) in custody |
| (Private) Nodal logic | Programmable logic that is owned by and *automatically* executed by a participant in the system but whose execution is private and internal to other participants.  Private nodal logic can only verified by its inputs and outputs.  Most web services (e.g. HTTP APIs) execute private nodal logic. |
| Crypto-currency | An asset (token) whose trust, concensus and economic model comes *solely* from the game-theory and economics of a DL (blockchain) system, enforced by rules shared by all participants rather than privately or externally |
| Virtual Digital currency | See above |
| Participant | Any actor (natural, company or autonomous code) within the system |
| Account | An identifier who is the owner/principal or recipient of tokens/funds at any time |
| MRB | Minimum Reserve balance - an amount that a custodial institution (bank) is required by regulation to hold to be compliant. |
| Keychain | Also known as a 'wallet' in crypto-currency.  Private keys used to sign transactions or execute logic. |
| Smart Contract | Programmable logic that is executed in a distributed environment (blockchain typically). Amongst other benefits this moves the trust, counterparty risk and integrity of its execution to the blockchain platform and away from a smaller group of counterparties.  Smart contract are *usually* transparent, allowing participants to verify logic matches their expectations and agreements, although there are methods to (deliberately) remove some of that transparency where desired |


Below are the function and non functional requirements the technical workshops are trying to solve for.

### Functional Requirements
|Requirement|Description|
|-----------|-----------|
| Legally compliant | The system must be compliant with Australian laws, *and broadly with international laws*. |
| Low barrier to participation | Joining the network should not require permission from any central authority, although other functions may require their co-operation. |
| Fungible | Any token must be 
| Identified parties | Participants must be able to identify who they are transacting with. |
| Open | is open to any individual or entity. Is not limited to use between a limited number of financial institutions. |
| No mediation | A holder of digital dollars can transfer dollars directly to another party without mediation by a third party.|
| Pegged | one digital dollar’s value closely pegged the value of one dollar held by the central bank.|
| Trust | The holders of the collateral that backs the digital dollar need to be trusted. |
| Private | only the parties involved in a transactions can see the parties, their balances and transaction amount.|
| Finality | Transactions must be final and irrevocable |
| Micro transactions | Can support sub 1 cent transactions |
| Delivery versus Payment | Digital assets (tokens) can be exchanged with a digital dollar in one atomic transaction.|
| Escrow | can be held in escrow by parties or programs (smart contracts).|
| Time aware | Transactions can be linked to time. e.g. transfer at a point in time, escrow until a point in time.|
| Oracles | External data can be used to as inputs to transactions. For example, the result of an event  |

## Future Integrations
| Integration | Description |
| Participant metadata | Participants (accounts) may attach descriptions of themselves and their assets, e.g. identify fields, or the current usage state of an asset, e.g. debt/mortgage, savings |
| AML/KYC capability | Allow use of AML/KYC services to certify identities used in the system |
| Identity query | Participants may issue permission to other participants to query identity meta-data *OR* check that a held meta-data field matches that from an identity authority |

### Non functional Requirements
|Requirement|Description|
|-----------|-----------|
|1000 txs/sec|1000 transactions per second is what Australia's New Payment Platform (NPP) was initially sized to.|
|sub sec latency| Transactions  |
|1 million nodes| EFTPOS is closing in on 1 million terminals in Australia|
|Machine/Mobile/IoT|Transactions can be signed on devices with low computing power.|

## Technical Challenges
 There are number of technical challenges that need to be solved in order to meet the functional and non functional requirements.
 
|Challenge|Description|
|---------|-----------|
| Privacy | Privacy of parties, transactions and balances |
| Performance |Scaling the number of participants, transaction throughput and reducing the transaction latency|
| Trust | Securing the collateral that pegs the value|
| Identity | Managing the identity of the participants which can be people, machines or things|
| Key management | Private keys used for signing transactions must be securely stored |

