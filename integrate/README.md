---
topic: overview
products:
  - azure
  - azure-blockchain	
---

# Integrate
![MIT license badge](https://img.shields.io/badge/license-MIT-green.svg)

Businesses are using blockchain and smart contracts to facilitate multi-party processes. Blockchain also delivers real-time transparency of the states and events of those contracts to appropriate participants.

End to end blockchain solutions require integration with data, software, and media that live “off chain”. External updates and events can trigger actions on smart contracts. Smart contract events and state changes can then trigger actions and data updates to “off chain” systems and data. These external systems and AI will also need the ability to query attestable data from smart contracts to inform action.

Specifically, there are two areas of integration where guidance is most needed - [smart contract interactions](#smart-contract-interaction) and [documents and media](#Documents-and-Media).

# Smart Contract Interaction
Getting blockchain off the whiteboard and into production means dealing with the realities of how counterparties interact today. That reality is that Enterprise integration is messy.

Microsoft brings our decades of experience in this area to blockchain. Our work with integrating Enterprise systems began almost two decades ago with the introduction of BizTalk server, and our focus on database integration traces back to our co-development of Open Database Connectivity (ODBC) in the 1990s. All of our experience has been captured and made available in Azure services. This includes 200+ connectors available in Logic Apps and Flow, and the robust capabilities in our data platform.

# Documents and Media
Documents and media do not belong on chain, but business processes often involve images, videos, audio, Office documents, CAD files for 3D printers or other file types.

The common pattern is to generate a unique hash of the media and the metadata that describes it. Those hashes are then placed on a public or private chain. If authenticity of a file is ever questioned, the “off chain” files can be re-hashed at a later time and that hash is compared to the “on chain” hash stored on the blockchain. If the hashes match, the document is authentic, but if so much as a pixel of an image or letter in a document is changed, the hashes will not match and this will make obvious that tampering has occurred.

The development kit includes a set of Logic Apps that enable the hashing of files and file related metadata. Also included are smart contracts for files and a file registry to store the hashes on chain.

Logic Apps have been created to deliver this functionality for files added to the most popular sources for documents and media, including Azure Storage, OneDrive, One Drive for Business, SharePoint, Box, Adobe Creative Cloud, and FTP.

## Integrate Samples
- [Azure Blockchain Workbench Samples](./WBSamples.md)
- [Ethereum Blockchain Connector for Logic Apps Samples](./EthereumLASamples.md)
- [Corda Blockchain Connector for Logic Apps Samples](./CordaLASamples.md)

