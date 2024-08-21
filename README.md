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

## 

