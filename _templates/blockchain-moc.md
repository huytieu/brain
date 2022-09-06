This is a [[Map of Content]] related to the blockchain.


## Foundational Topics
---
<%*
const query = `LIST FROM #blockchain AND #foundational-topics`
const dv = this.app.plugins.plugins["dataview"].api ;
const te = await dv.queryMarkdown(query);
tR += te.value;
%>

## Decentralized Finance (DeFI)
---
<%*
const query1 = `LIST FROM #blockchain AND (#defi AND -#dex AND -#nft AND -#smart-contract) AND -"Blockchain/DeFi 1"`
const te1 = await dv.queryMarkdown(query1);
tR += te1.value;
%>
### Decentralized Exchange (DEX)
<%*
const query2 = `LIST FROM #blockchain AND #dex AND -"Blockchain/DeFi 1"`
const te2 = await dv.queryMarkdown(query2);
tR += te2.value;
%>
## Non-Fungible Tokens (NFT)
---
<%*
const query3 = `LIST FROM #blockchain AND #nft`
const te3 = await dv.queryMarkdown(query3);
tR += te3.value;
%>
## Solana
---
<%*
const query4 = `LIST FROM #blockchain AND #solana`
const te4 = await dv.queryMarkdown(query4);
tR += te4.value;
%>
## Bitcoin
---
<%*
const query5 = `LIST FROM #blockchain AND #bitcoin`
const te5 = await dv.queryMarkdown(query5);
tR += te5.value;
%>

*This page was last modified at <%* tR += new Date().toISOString();%>*.
