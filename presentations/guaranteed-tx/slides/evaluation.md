<!-- .slide: data-background="#146287" -->
## Evaluation


<div style="text-align:left;">
<h3>Performance</h3>

<ul>
<li>Dependencies
<ul>
  <li>Fork rate</li>
  <li>Required additional confirmations</li>
  <li>Epoch length</li>
  <li>Slashing conditions</li>
</ul></li>
<li class = "fragment">Average transaction rate</li>
</div>


<h3>Latencies</h3>
<table>
  <thead>
  <tr>
    <th>    </th>
    <th>Ethereum 2.0</th>
    <th>Guaranteed-TX</th>
  </tr>
  </thead>
  <tr>
    <th>TX <sub>cross</sub> latency</th>
    <td>3.2 min</td>
    <td>M x slottime </td>
  </tr>
  <tr>
    <th>TX <sub>cross</sub> jitter</th>
    <td> 3.5 min</td>
    <td> n.a.</td>
  </tr>
    <tr>
      <th>TX <sub>app</sub> latency</th>
      <td>N x epochtime </td>
      <td><i>N x TX <sub>cross</sub> latency</i></td>
    </tr>
</table>


<h3>Overhead</h3>
<table style="width: 130%; margin-left:-15%;">
  <thead>
  <tr>
    <th>Use case</th>
    <th style="text-align:right">A</th>
    <th style="text-align:right">B</th>
    <th style="text-align:right">C</th>
    <th style="text-align:right">D</th>
  </tr>
  </thead>
    <tr>
      <th>Number of TX<sub>app</sub> per block</th>
      <td style="text-align:right">150</td>
      <td style="text-align:right">115</td>
      <td style="text-align:right">100</td>
      <td style="text-align:right">83</td>
    </tr>
     <tr>
         <th>Number of TX<sub>cross</sub> per block</th>
          <td style="text-align:right">0</td>
          <td style="text-align:right">35</td>
          <td style="text-align:right">83</td>
          <td style="text-align:right">67</td>
        </tr>
   <tr>
           <th>No Guaranteed-TX</th>
            <td style="text-align:right">31.72 MiB</td>
            <td style="text-align:right">32.27 MiB</td>
            <td style="text-align:right">32.50 MiB</td>
            <td style="text-align:right">32.77 MiB</td>
          </tr>
            <tr>
         <th>Guaranteed-TX</th>
          <td style="text-align:right">5.00 MiB</td>
          <td style="text-align:right">214.79 MiB</td>
          <td style="text-align:right">304.71 MiB</td>
          <td style="text-align:right">406.41 MiB</td>
        </tr>  
           <tr>
        <th>Optimised Guaranteed-TX</th>
         <td style="text-align:right" >24.98 MiB</td>
         <td style="text-align:right">25.40 MiB</td>
         <td style="text-align:right">25.78 MiB</td>
         <td style="text-align:right">26.05 MiB</td>
       </tr> 
</table>
<p><small>Transferred cross-shard transaction data per epoch per node</small></p>


<div style="text-align:left;">
<h3>Overhead</h3>
Similar overhead with or without optimised Guaranteed-TX

<p class="fragment"><br>
<b>but... </b> overhead is 30x more than the am ount of data shared within a single shard
</p>
</div>


<h3>Known limitation</h3>
<ul>
      <li> No upper bound  cross-shard transaction latency
<ul>
      <li>Epoch length</li>
      <li>Maximum stake penalisation</li>
</ul>
</li>
</ul>