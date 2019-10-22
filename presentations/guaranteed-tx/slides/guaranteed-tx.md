<!-- .slide: data-background="#146287" -->
## Solution

<small>Guaranteed-TX design</small>


### The idea:
- Record every created and processed cross-shard transaction
- Punish validators for not processing transactions

Note:
- Optimistic execution:
    - shard that processed needs to keep track of creation
- Guaranteed execution
    - shard that craeted needs to keep track of processed 
   
- A block that created a TX cross, shares this
- A block that processed a TX cross, shares this
- Punish validators

<div class="container">
    <div class="col">
    <h3>Design: </h2>
    </div>
    <div class="col">
        <ul>
            <li>Layered architecture</li>
            <li>Heartbeat mechanism</li>
            <li>Slashing conditions</li>
            <li>Block filtering</li>    
        </ul>
    </div>
</div>


<h4>Layered architecture</h4>

<div style="margin-top:2em;" class="container">
    <div class="col">
    <img src="img/ledger-old.svg" alt="Design" style="margin-bottom:10%; height: 2.2em; margin-left:1em" />
    <p><small>Ethereum 2.0</small></p>
    </div>
    <div class="col">
    <img src="img/ledger-new.svg" alt="Design" style="margin-bottom:10%; height: 2.2em; margin-left:1em" />
    <p><small>Guaranteed-TX</small></p>
    </div>
</div>

 <img src="img/ledger-legend.svg" alt="Design" style="margin-bottom:10%; height: 1.5em; margin-left:1em" />


<h4>Layered architecture</h4>
<img src="img/overal.svg" alt="Design" style="height: 8em; margin-left:1em" />
<img src="img/overal-legend.svg" alt="Design" style="margin-bottom:10%; height: 1.5em; margin-left:1em" />


<h4>Heartbeat mechanism         </h4>
<img src="img/heartbeat.svg" alt="Design" style="margin-top:2em; margin-bottom:10%; height: 6em; margin-left:1em" />
<p style="margin-top:-1em;">
<b>Cross-link</b> = heartbeat  (every 6.4 minutes) <br> 
<p>


<div style="text-align:left"> 
<h4>Slashing conditions</h4>
   <ul>
            <li>Malicious message part production</li>
            <li>Not processing cross-shard transactions
        </ul>

<p class="fragment"><br>
<b>but... </b> punishment can not be severe
</p>
</div>


<h4>Filtering blocks</h4>
<img src="img/filtering.svg" alt="Filtering" style="margin-top:1em; margin-bottom:10%; height: 4em; margin-left:1em" />
<img src="img/filtering-legend.svg" alt="Filtering" style="margin-bottom:10%; height: 2em; margin-left:1em" />


<div style="text-align:left"> 
<h4>Optimisations</h4>
<ul>
    <li>Batching cross-shard transactions</li>
    <li>Shard action lists
      <ul><li>Reduced overhead costs 10x</li></lu>
                </li>
                </li>
</ul>