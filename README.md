# Blockchain Identity


## Abstract
This whitepaper outlines a token-based platform that will allow users to connect with their friends and verify themselves across the web in a secure and pseudo-anonymous manner. This is achieved through an incentived smart-contract that rewards users for correctly verifying another user. Users will be able to send encrypted messages to one another, as well as encrypt private information, which they can selectively share or sell. Users will have a type of income called "Credibility", which determines the likeliness that the user is who they say they are. The main problem that this technology will solve, is the issue of identity fragmentation and leaked information. It's assumed that users are reluctant to have an identifiable online identity, due to the lack of security and the necessity of trusting an organization with your sensitive information. We intend to put users in control of their data and social networks. To do this we need a secure way of verifying users, but this can't be done using only primary identification, due to the likelihood that this identification can be replicated. Identity shouldn't be able to be replicated, but there are very few things that the users on the internet cannot replicate. High governmental authorities will use a combination of primary identity along with proof of your social network. ie. Passport recovery in Canada involves having 2 other citizens vouch for you. It is relatively easy to hack a server and steal identification, but it's very hard to hack someone's life and steal all their friends. On top of this, it's also difficult to steal a password that you don't have stored on a server. To put users in control of their own data and social networks, we will rely on a combination of primary identity, passwords and friendships. The user will want to vouch for their friends as they can verify their identity and in turn will receive credibility for correctly verifying their identity. Using different encryption algorithms we will implement private messaging, private data storage and eventually be able to verify sensitive information without displaying this information. Login protocols and age verification can be accomplished without necessarily leaking the exact age. This opens up an opportunity for an innovation in online identity, where a user's data can be proven without being shared, increasing both security and privacy. This type of identity system is referred to as [Self-Sovereign-Identity](http://www.coindesk.com/path-self-sovereign-identity/). There are two main hurdles to creating a self-sovereign-identity. How can we quantify the credibility of an entity and how do we know that the data truly belongs to them?  Credibility is defined as the probability that you are a real entity and that you are able to vouch for other entities you know are real. Data is defined as anything you use to tell the world who you are. Data can be bought and sold, whereas credibility is assumed to be scarce and cannot be sold.  A user requires credibility to store data, but also requires proof-of-data to gain credibility. Through these mechanisms we hope to build a platform that can supply users with simpler and more secure online verification process. 


## Economy of Credibility
The economy of credibility operates through financial gambles on another users' identity, creating a proof-of-trust in this person. Each user is required to gamble a percentage (or minimum amount) of their credibility on themselves. In this way, nodes will lose credibility when a majority of users are gambling against them. 
![Credibility](https://github.com/kyledewy/BlockchainVerify/blob/master/charts/credibilitymarket.png)
This gamble will hold a financial reward if the majority of nodes agree with the users' bet, whether it's yes or no. In this way there will be financial incentive to both verify your friends, and find nodes who don't indicate future credibility.  We refer to these users as nodes because each node may be a single entity of any type, such as a corporation, a group of people, or bot in the form of a smart contract. Although much of this platform is designed to reduce bots, I think it may be valuable to allow bots as long as they are properly identified as such. People may produce effective bots that are programmed to do positive things for the network, and as long as they are properly identified, they may be considered credible bots by the network. It's unclear what economic role bots would play, if they're allowed, since it's problematic to have them reinforcing particular users. Perhaps bots could be allowed, but only are allowed to vote "no" on other nodes. Remember Credibility doesn't necessarily indicate a degree of trustworthiness, but instead represents whether the network thinks you are who you say you are.
![Credibility Payout](https://github.com/kyledewy/BlockchainVerify/blob/master/charts/credibilitypayout.png). Credibility payouts will be made every x blocks. Each round a node is required to gamble "yes" on themselves, which they will earn back if the majority of nodes agree that you are credible. A problem with this approach is that when a node achieves 100% "yes" votes, the supporters will not receive any profits, since there is no one voting "no" and subsequently paying the winners. A solution is required for this problem as there remains no incentive to vote "yes" on somebody that has nobody voting "no", since there are no losers in this market. It's a small problem however, because reinforcing a node which already has 100% "yes" majority, may not pay off immediately, but your securing a safe bet incase of future attacks. The economics of this indicate that controversial nodes will be more profitable. The biggest payout a node can gain is to win a market with 51% of votes. This maximizes the amount of Credibility earned, but is inherently more risky. 


## Use Cases
The use cases of this technology are broadly concerned with situations where you would like to prove your information without sharing it. If a user would like to prove that they have enough Ethereum, they can use this platform to prove they have enough, without explicitly showing their balance. Crypto currency is moving towards implementations of [Zero-Knowledge-Proofs](https://en.wikipedia.org/wiki/Zero-knowledge_proof). This technology allows for the proof of information, without revealing this information. ![Zero-Knowledge-Proof](https://github.com/kyledewy/BlockchainVerify/blob/master/charts/zeroknowledge.png) This picture shows the basic concept of recursive prediction/result sequence. This technology can be used to check for minors, without publicly stating what their exact age is. The obvious use cases of this platform would be to secure login protocols and to implement verification protocols that don't unnecessarily store private information on servers. Eventually the platform can be used to eliminate bots on other platforms and create a stable reference point for users to find out the addresses of their friends wallets. Ideally as browser technology changes and IPFS/Blockstack begins to reshape the internet, we hope that other blockchain companies will utilize ad-block and the new Dapp payment structures, to put browsing data in the hands of the user. The use case then is to streamline and add security to current verification processes and to give users monetary control over their private information.


## Identity
Although this platform is heavily tied to identity, it doesn't encourage users to share the extent of their identities. The user would only have to share enough information that their friends would be able to verify them and strangers can feel assured that you are not fictional. Beyond this necessity, a user can increase his anonymity to leverage themselves to be able to monetize this data. A large area of our economy is concerned with decoding the spending habits of consumers, however using different anonymous wallets, users can successfully hide their spending habits if they so choose. This puts the power in the users hand, as they retain this useful data under their control and can therefore monetize it if somebody is interested in having it. The user regains control of their data and can profit off it by using our platform which offers permission-based-access to private information. The developing identity economy allows users to privatize their data and profit off of it, but it also means that the software we use is no longer free. Current models tend to offer a free service and then sell the data that is derived from users using the service. What could develop in the blockchain world is that services will tend to charge micro payments depending on how much of the service you would like to use. ie. Augur, PeerTracks, MyBit. Advertisers are left with a different landscape. Instead of a central service keeping track of it's users, there are going to be many services that can link activities to a public key (instead of cookie). The identity economy will be based around two tokenized-markets. Credibility and Data, which are not necessarily related but require one another. In this system credibility will be the profit margin between people gambling "yes" on the validity of your identity and the people gambling "no" on the validity of your identity. Your data will be everything you use to let the online world know who you are. Unline credibility, data can be bought and sold, but this data relies on the node being credible in the first place. In this way we would like to secure a network that reinforces credible nodes and then develop tools in which users can become autonomous and pseudo-anonymous over their online identity and financial operations.  
![Storing Data](https://github.com/kyledewy/BlockchainVerify/blob/master/charts/storingData.png)

## PGP
PGP is a time-tested mechanism for exchanging encrypted messages and provides an efficient way to encrypt data and send messages.
![Proof Of Data](https://github.com/kyledewy/BlockchainVerify/blob/master/charts/pgpProof.png)


## Identity Disputes
There may be situations where a node is credible but is claiming anothers persons data to be their own. This type of conflict will be solved by creating a special type of gambling market, where either side is allowed to present evidence and communicate with users invited to arbitrate the dispute. A vote will take place in which each user commits a minimum amount of Credibility and/or Ether in support of one side or the other. The user that reaches consensus in this vote will be rewarded with the Credibility/Ether and the loser will be eliminated from the network. This is done so that no duplicates exist on the network. Names can be duplicates, but they must be referring to seperate people. Most identity disputes will actually be users who have lost the password/private-keys to their previous accounts and are therefore forced to create a duplicate node of their previous self and start a dispute against that old node. In this case the old node won't be able to present any evidence and will sacrifice his Credibility/Ether to the new node. All people vouching for the old node will be invited to the market to indicate whether they support the challenging node, or the challengee node. ![Disputes](https://github.com/kyledewy/BlockchainVerify/blob/master/charts/disputes.png). Three outcomes can come from this. Either node 1 gets claim on data, node 2 gets claim on data, or neither has valid claim on the data which will subsequently erase the data from the network. This is a complex game theory problem that needs to be reviewed intensively. 


## Security 
The main problem with running an incentivized and decentralized service is the game theory problems that can open up. An obvious weakpoint is the ability for someone to create thousands of nodes and subsequently create a self-reinforcing ring of nodes that all verify eachother. This attack however, would cost a lot of money to start up and would rest on a very fragile foundation, since this credibility-network isn't diverse and can fall in a domino effect as the reinforcing nodes get discovered. Security against this attack would naturally be users who are looking for obvious collusion networks. As this platform grows so does the security, but so does the ambitions for cheating. 



## Problems To Be Solved
It will be vital for a new node on the network to sign up with a very credible node to avoid being gambled against by the network. The smart contracts could be coded, to allow for a multi-sig node that can do direct verification, such as encrypting drivers license numbers, proof of address or any of the typical centralized verification approaches. With token-incentivization, decentralization is an efficient way of delegating power and offers higher security, however, it is a difficult approach when the network is small. Crowdsourced economies work better when the crowd is large (ie. Wikipedia, Stack Exchange). For this reason it may be smart to have a pre-programmed centralized aspect that fades over time, as a way to transition into a fully decentralized identity platform. 

## Costs 
	The preliminary prototype will require the following functionality. A rough estimate is $3000, although the prototype could be stripped of messaging which would cut the cost. 
		Front-End/Ethereum node
			On browser encryption
			Ethereum node private/public key signing
		Smart Contract
			Credibility market (An escrow-like contract that resolves the ledger for current user bets)
			User profile functionality
			PGP verification
			Basic messaging functionality
			Store encrypted data (very expensive...will need to store this on IPFS/SWARM when off test network)

		
	The full proof of concept is only a concept at this point, and to make it a proof of this whitepaper we would need the following additions on top of the above prototype. Everything below is assumed to have extensive testing and should have some percentage of the total cost spent solely on testing. I recommend an abnormally high percentage of this projects budget be put to testing and bug bounties. This concept involves very complex game theory problems, and the novelty of autonomously incentivized organizations, requires a high investment in future security, due to the difficulty of updating smart contracts. 
		Encryption 
			Zero Knowledge Proof Research + possible implementation
		Smart Contract 
			credibility markets, credibility tokens,  
		Whisper 
			Messaging between Ethereum Nodes 
		PGP 
			A good system of verifying and sending messages using PGP
		IPFS/Swarm 
			Need to store expensive data structures on Swarm/IPFS
		ENS 
			Linked to ENS to help identify people
		IBAN/ICAP
			Have an ICAP reference for each user
		Ether Gas 
			Most gas costs should be paid at the time of transaction by the initiating party. There will be significant costs involved in paying out credibility after each round. 

