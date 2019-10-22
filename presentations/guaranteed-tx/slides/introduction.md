<!-- .slide: data-background="#146287" -->
## Introduction


<div class="container">
    <div class="col">
         <img src="img/visa.svg" alt="Visa" style="margin-bottom:10%; height: 1.5em; " />    
         <p>Centralised</p>    
         <p>1700 TPS</p>   
                  <p>&nbsp;</p>   
    </div>
    <div class="col">
        <img src="img/bitcoin.svg" alt="Bitcoin" style="margin-bottom:10%; height: 1.5em;" />
         <p>Decentralised</p>    
         <p>4.8 TPS</p>  
         <p>&nbsp;</p>  
    </div>
</div>

Note:
- Today, banks are at the heart of our financial system:
- A bank is an intermediary. They are between two parties who are making transactions. 
- In 2009 Bitcoin, cryptocurrency
- Compare Bitcoin and VISA
- No scalability
- Unable to process transactions at the speed of centralised systems 


<div class="container">
    <div class="col">
         <img src="img/centralised.svg" alt="Centralised" style="margin-bottom:10%; height: 4em; " />    
         <p>Centralised</p>     
    </div>
    <div class="col">
        <img src="img/distributed.svg" alt="Distributed" style="margin-bottom:10%; height: 4em;" />
         <p>Decentralised</p>    
    </div>
</div>

Note:
- Centralised: one company VISA, maintain all our accounts, storage of data, processing our request.
- Decentralised: 
    - Digital ledger which stores changes
    - Initial state - accumulated changes - end state
    - Set of predefined rules 
- Everyone has a copy
    - Everyone validate them self
    - Need to agree on the same set of change
    - Consensus problem


<div class="container">
    <div class="col">
        <img src="img/ethereum.svg" alt="Ethereum" style="margin-bottom:10%; height: 10em;" /> 
    </div>
    <div class="col">
<p>
<ul>
    <li>Digital money</li>
    <li>Smart contracts</li>    
</ul>
</p>
<p style="margin-top:1em;" class="fragment"><b>BUT...</b> 15 TPS<p>
</div>
</div>

<p class="fragment" >
<b> Version 2.0: </b> Scalability through <i>sharding</i> <br> Phase 0: January 2020
</p>

Note:
- Late 2013 Ethereum
- Payment transactions - Ether
- The novelty is extenson of these rules.
- By publishing code, a small application defining some new rules.
- but 15 TPS
- New verson technique sharding

- Rollout in phases


### Sharding

<div class="container">
    <div class="col">
    Split the computational work among multiple groups of participants 
 </div>
        <div class="col fragment">
         Full sharding:
         <ul>
             <li>Storage</li>
             <li>Processing</li>   
             <li>Communication </li>
         </ul>
         </div>
    </div>

Note:
- Transaction china and netherlands
- Split validators and accounts states
- Shards

- Partition transaction processing not enough
- Reduce per node - Validator


<div class="container">
    <div class="col">
         <img src="img/non-sharded-ledger-crop.svg" alt="Non-sharded ledger" style="margin-bottom:10%; height: 6em;" />    
         <p>Non-sharded ledger <Br> <small>15 TPS</small></p>     
    </div>
    <div class="col">
        <img src="img/sharded-ledger-intro.svg" alt="Sharded ledger" style="margin-bottom:10%; height: 6em; margin-left:1em" />
         <p>Sharded ledger  <br> <small>N x 15 TPS</small></p>    
    </div>
</div>

Note:
- What does this mean for a distributed ledger
    - Non-sharded: validators, TPS
    - Sharded: N times, n = 1000
- Problems:
    - Security (1 shard takeover)
    - Cross-sharding: Transaction changes multiple shards
    - TX_app and TX_cross
    - Receipts
- ING to RABO transaction
    - trust in each other
    - time


### Problems:
<div class="container">
    <div class="col">
         <img src="img/stale-block.svg" alt="Stale block" style="margin-bottom:10%; height: 4em;" />    
         <p><small>Receipt from stale block.</small></p>     
    </div>
    <div class="col">
        <img src="img/not-processed.svg" alt="Not processed receipt" style="margin-bottom:10%; height: 4em; margin-left:1em" />
         <p><small>Receipt not processed by target shard</small></p>    
    </div>
</div>

Note:
- Shards currently have no obligation
- Create tokens
    - Block not directly final
    - Think about revered entry. (storneren)
- Delete tokens


### Research:
How can we facilitate guaranteed cross-shard transaction execution in a sharded distributed ledger?
<p></p>


<div class="container">
    <div class="col">
    <h2>Result: </h2>
    </div>
    <div class="col">
        <h3>Guaranteed-TX</h3>
        <ul>
            <li>Optimistic execution</li>
            <li>Guaranteed execution</li>    
        </ul>
    </div>
</div>

Note:
- Explain optimistic execution
- Explain Guaranteed execution
- Outline for the rest presentation
    - Background Ethereum 2.0
    - Solution
    - Evaluation
