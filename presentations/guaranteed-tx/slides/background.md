<!-- .slide: data-background="#146287" -->
## Background

<small> Ethereum 2.0 </small>


<div class="container">
    <div class="col">
    <h3>Blockchain: </h2>
    </div>
    <div class="col">
        <ul>
            <li>Cryptography</li>
            <li>Consensus</li>
            <li>Cryptoeconomics</li>    
        </ul>
    </div>
</div>

Note:
- Cryptography:
    - chained blocks
    - identification transactions
    - identification of user and accounts
- Consensus
    - Leader based: inefficient
    - Finalisation once in a while
    - Malicious nodes
- Crypto economics
    - Rewardings low
    - Punishments high
    - Deposits


<h4>Shard design</h4>
<img src="img/shard-design.svg" alt="Design" style="margin-bottom:10%; height: 6em; margin-left:1em" />

<p style="margin-top:-1em;">
<b>Epoch</b> = 64 slots = 6.4 minutes <br> 
<b>Slot</b> = 6 seconds
</p>

Note:
- Block generation periods:
    - Epoch
    - Slots
- Validator is assigned
- Not necessarily a block
    - network delay
    - malicious behaviour


<h4>Cross-linking shards</h4>
<img src="img/ethereum-design.svg" alt="Design" style="margin-bottom:10%; height: 12em; margin-left:1em" />

Note:
- Crosslinking
    - A cross-link is an attestation for a particular block
    - 6.4 minutes
- Process of cross-shard transaction: 
    - could be 6 seconds
    - could be 6.4 minutes