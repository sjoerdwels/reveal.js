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