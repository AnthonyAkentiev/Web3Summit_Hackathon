# Web3Summit_Hackathon - Anytype Gate project

## Disclaimer
I was hacking solo. I work full time at Anytype as a Web3 engineer.

## Short Description
Anytype is “like Notion”, but:
* Open source
* Local-first (no need for internet)
* P2P (you can set up a network just between your friends, family, etc)
* Web3-friendly
  *   Ethereum private key address internally
  *   You can use the **SAME SEED PHRASE in your MetaMask** to control your assets like ANY name!
  *   Naming system is based on ENS
  *   We use AccountAbstraction (by Alchemy)
  *   ...

## Hackathon Idea
Anytype Space are currenly like Communities.
You can **Join** spaces, share links, etc.
You can **Collaborate** together - write docs, chat, etc.

Let's add more Web3 SOCIAL FEATURES: **add NFT token gating to the Anytype.**

<img width="1677" alt="anytype-screen" src="https://github.com/user-attachments/assets/b5d04d78-06af-4923-bf42-82627e8c16ad">

## Architecture
![AnytypeGatingArch](https://github.com/user-attachments/assets/d3960fc7-28b8-41ea-b301-ae688546f6cf)

## Full Presentation
[Here](https://docs.google.com/presentation/d/1_hwlBbFb36U9f-ePhIKG44maaBdKzqZ6rOF-BKar4k0/edit?usp=sharing).

## How to run
1. Clone **web3-summit-hack** branch of [anytype-heart](https://github.com/anyproto/anytype-heart/tree/web3-summit-hack)
2. Clone **web3-summit-hack** branch of [anytype-ts (desktop client)](https://github.com/anyproto/anytype-ts/tree/web3-summit-hack)
3. Run anytype-heart: `ANYTYPE_LOG_LEVEL=debug make run-server`
4. Run anytype-ts: `SERVER_PORT=8080 ANYTYPE_USE_SIDE_SERVER=http://127.0.0.1:31008 npm run start:dev`

## What to do
1. Create an Account1
2. Create Space1
3. Click on "Share space with NFT token gating"

<kbd>
<img width="498" alt="share_space" style="border: 2px solid grey;" src="https://github.com/user-attachments/assets/c77fa273-6281-4896-a6ea-a947358ee9b5">
</kbd>

5. Enter your NFT address. E.g.: 0x709981f628593c60182f77f15abc59bc47609d13
<kbd>
<img width="1661" alt="open_sea" style="border: 2px solid grey;" src="https://github.com/user-attachments/assets/a0f94e4b-57b3-4f8a-9cc6-4d5f7dfbdf43">
</kbd>

6. Generate a link. E.g.: `https://invite.any.coop/bafybeid6opln5wbtq6uhd6cc56r5zjcnxkydf5tcvltgcynuiwdvdejkwm#Dfdwp1qJqsepB4QD9Eut4fpbNKo7SAtotgnAQdtY1V12&nftTokenAddr=0x709981f628593c60182f77f15abc59bc47609d13`

7. Create an Account2
8. Paste the link into your browser
9. Click on "Join"
<kbd>
<img width="412" alt="join" style="border: 2px solid grey;" src="https://github.com/user-attachments/assets/fc34522a-8dc9-4275-b6c6-512cdece50ac">
</kbd>

10. It should fail, because you don't have a required NFT token:

<kbd>
<img width="406" alt="join_fail" style="border: 2px solid grey;" src="https://github.com/user-attachments/assets/c7fc29f0-3c85-4b83-bb34-c11bb084a2a0">
</kbd>

11. Now what is cool about Anytype is that we have an Ethereum address that is DERIVED from your Anytype seed phrase! This means that you can use the **SAME SEED PHRASE in your MetaMask** to control your tokens.

<kbd>
<img width="843" alt="settings" style="border: 2px solid grey;" src="https://github.com/user-attachments/assets/428707a6-96e9-4265-9b61-bfe9e17235d1">
</kbd>
 
12. Let's send a required NFT from your MetaMask to Account2! E.g.: 0x0840dC22150646bAd4e0d3cBeBeCCdbAB8e032a2
<kbd>
<img width="352" alt="metamask" style="border: 2px solid grey;" src="https://github.com/user-attachments/assets/198eddc3-f37b-41b0-9c3e-8f4d03d2fa1e">
</kbd>

13. Now try to join the space again (steps 5-8):

<kbd>
<img width="412" alt="join" style="border: 2px solid grey;" src="https://github.com/user-attachments/assets/fc34522a-8dc9-4275-b6c6-512cdece50ac">
</kbd>

14. SUCCESS!!! NFT check succeeded.
Now the final step is for Account1 to accept Account2!!!

<kbd>
  <img width="1671" alt="success" style="border: 2px solid grey;" src="https://github.com/user-attachments/assets/e6b95b97-0103-4dec-bb23-16f7675429d5">
</kbd>




