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