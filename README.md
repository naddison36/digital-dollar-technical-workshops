# Digital Dollar - Technical Workshops
A series of workshops attended by Blockchain experts in Sydney to address the technical challenges of issuing a digital dollar on Blockchain/distributed ledger.

## Problem statement
*How to create a digital Australian dollar that will power the next generation of distributed services.*

## Requirements
There are many different solutions for creating a digital currency as they are all solving for different requirements. For example, Bitcoin is designed to work in an untrusted environment where the identity of the participants is unknown. Ripple is designed to work with known deposit taking organisations. Ethereum is designed to be a general computing platform that operates in an open, untrusted environment.

Below are the function and non functional requirements the technical workshops are trying to solve for.

### Functional Requirements
|Requirement|Description|
|-----------|-----------|
| Legally compliant | The system must be compliant with the Australian laws. eg KYC/AML |
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
|---|---|
| Privacy | Privacy of parties, transactions and balances |
| Performance |Scaling the number of participants, transaction throughput and reducing the transaction latency|
| Trust | Securing the collateral that pegs the value|
| Identity | Managing the identity of the participants which can be people, machines or things|
| Key management | Private keys used for signing transactions must be securely stored |
