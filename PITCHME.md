<style type='text/css'>
figcaption {
  font-size: 50%;
}
.paragraph1 {
  font-size: 18px;
}
.paragraph2 {
  font-size: 13px;
}
.paragraph3 {
  font-size: 10px;
}
.tg  {border-collapse:collapse;border-spacing:0;border-color:#ccc;}
.tg td{font-family:Arial, sans-serif;font-size:18px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:#ccc;color:#333;background-color:#fff;}
.tg th{font-family:Arial, sans-serif;font-size:18px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:#ccc;color:#333;background-color:#f0f0f0;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-yw4l{vertical-align:top}

/*
table {font-family:Arial, sans-serif; font-size:18px;}
table td {padding:10px 5px;}
*/
li {
  font-size: 26px !important;
}
.tg tr:last-child {border-bottom: 1px solid #ccc;}

</style>

## Towards DTN Adaptive routing

26.06.2018 - José Irigon, Manuel Weißbach

---

### Store & Forward x Connection oriented 

<video width="640" height="480" controls>
  <source src="https://raw.githubusercontent.com/irigon/ASiCS_presentation/master/videos/dtn.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

<span style="font-size: 19px;">[1] Credits: NASA</span>

---

### DTN - Use Cases examples

- Wild life [Juang2002]
- Disaster response and Humanitarian Aid [Kannan2008]
- DakNet, TrainNet [Pentland2004,Zarafshan-Araki2010]
- Vehicular DTN [Sharef2014]
- Unmanned Air/Underwater Systems [Johansen2014]
- Ring Road [Burleigh2011]

Note:
  - ZebraNet - Kenia
  - Terrestrial cost effective connectivity
  - Ring Road: Satellite cost effective connectivity
  - If 

---

### Challenges in DTN adoption

 - Routing is context bound
 - Use-case depends on context available resources
 - Different contexts &#8594; abstracts &#8594; same problem 
 - Less done towards internetworking

Note: 
p2: reutilization might needs the same combination
p3: deep space x ad-hoc mobile networks: latency, routing different -- disruption the same
However, a group of scientists usually works on similar problems
Next: In order to improve DTN adoption we urge to 

---

### Context in DTN

- Stochastic
- Probabilistic
- Deterministic

---

### Stochastic 

<figure>
<img src="https://raw.githubusercontent.com/irigon/ASiCS_presentation/master/figures/3-shows.gif" alt= "3 room party" width="464" height="403">
</figure>

---

### Probabilistic 

<figure>
<img src="https://raw.githubusercontent.com/irigon/ASiCS_presentation/master/figures/shortestpath.gif" alt= "cars" width="624" height="415">
</figure>


---

### Deterministic 

<figure>
<img src="https://raw.githubusercontent.com/irigon/ASiCS_presentation/master/figures/worldMap-deterministicMove.gif" alt= "satelites" width="504" height="259">
</figure>

---


### Abstracting a DTN network

<figure>
<img src="https://raw.githubusercontent.com/irigon/ASiCS_presentation/master/figures/Scenario-simple.png" alt= "simple" width="281" height="323">
</figure>

---

<div id="image-table">
<table>
<tr>
<td style="padding:15px">
<img src="https://raw.githubusercontent.com/irigon/ASiCS_presentation/master/figures/Stochastic.gif" alt= "Stochastic" width="190" height="354">
<figcaption style="font-size: medium; text-align: center;">Stochastic</figcaption>
</td>
<td style="padding:15px">
<img src="https://raw.githubusercontent.com/irigon/ASiCS_presentation/master/figures/Probabilistic.gif" alt= "Probabilistic" width="190" height="354">

<figcaption style="font-size: medium; text-align: center;">Probabilistic</figcaption>
</td>
<td style="padding:15px">
<img src="https://raw.githubusercontent.com/irigon/ASiCS_presentation/master/figures/Deterministic.gif" alt= "Deterministic" width="190" height="354">
<figcaption style="font-size: medium; text-align: center;">Deterministic</figcaption>
</td>
</tr>
</table>
</div>

---

Routing algorithm performance

<table class="tg">
<tr>
<th class="tg-yw4l"></th>
<th class="tg-yw4l">Epidemic</th>
<th class="tg-yw4l">Prophet</th>
<th class="tg-yw4l">CGR</th>
<th class="tg-yw4l">RBAR</th>
</tr>
<tr>
<td class="tg-yw4l">Stochastic</td>
<td class="tg-baqh">&#9724;</td>
<td class="tg-baqh">&#9633;</td>
<td class="tg-baqh">&#9633;</td>
<td class="tg-baqh">&#9724;</td>
</tr>
<tr>
<td class="tg-yw4l">Probabilistic</td>
<td class="tg-baqh">&#9633;</td>
<td class="tg-baqh">&#8862;</td>
<td class="tg-baqh">&#9633;</td>
<td class="tg-baqh">&#8862;</td>
</tr>
<td class="tg-yw4l">Deterministic</td>
<td class="tg-baqh">&#9633;</td>
<td class="tg-baqh">&#9633;</td>
<td class="tg-baqh">&#9724;</td>
<td class="tg-baqh">&#9724;</td>
</tr>
</table>
<p style="font-size: 16px">&#9724;</span>: Good, &#8862;: Average, &#9633;: Bad </p>
---

Still to be done

<table class="tg">
<tr>
<th class="tg-yw4l"></th>
<th class="tg-yw4l">DTN2</th>
<th class="tg-yw4l">uPCN</th>
<th class="tg-yw4l">IBR-DTN</th>
<th class="tg-yw4l">uION</th>
<th class="tg-yw4l">uDTN</th>
<th class="tg-yw4l">JavaDTN</th>
</tr>
<tr>
<td class="tg-yw4l">RR Adaptation</td>
<td class="tg-baqh">&#9633;</td>
<td class="tg-baqh">&#9724;</td>
<td class="tg-baqh">&#9724;</td>
<td class="tg-baqh">&#9724;</td>
<td class="tg-baqh">&#9724;</td>
<td class="tg-baqh">&#9724;</td>
</tr>
<tr>
<td class="tg-yw4l">RR Parameterization</td>
<td class="tg-baqh">&#9633;</td>
<td class="tg-baqh">&#9724;</td>
<td class="tg-baqh">&#9724;</td>
<td class="tg-baqh">&#9724;</td>
<td class="tg-baqh">&#9724;</td>
<td class="tg-baqh">&#9724;</td>
</tr>
<tr>
<td class="tg-yw4l">RR Extension</td>
<td class="tg-baqh">&#9724;</td>
<td class="tg-baqh">&#9724;</td>
<td class="tg-baqh">&#9724;</td>
<td class="tg-baqh">&#9724;</td>
<td class="tg-baqh">&#9724;</td>
<td class="tg-baqh">&#9724;</td>
</tr>
<tr>
<td class="tg-yw4l">Stochastic Routing</td>
<td class="tg-baqh">&#9633;</td>
<td class="tg-baqh">&#8862;</td>
<td class="tg-baqh">&#9633;</td>
<td class="tg-baqh">&#9724;</td>
<td class="tg-baqh">&#9633;</td>
<td class="tg-baqh">&#9633;</td>
</tr>
<tr>
<td class="tg-yw4l">Probabilistic Routing</td>
<td class="tg-baqh">&#9633;</td>
<td class="tg-baqh">&#8862;</td>
<td class="tg-baqh">&#9633;</td>
<td class="tg-baqh">&#9724;</td>
<td class="tg-baqh">&#8862;</td>
<td class="tg-baqh">&#8862;</td>
</tr>
<tr>
<td class="tg-yw4l">Deterministic Routing</td>
<td class="tg-baqh">&#8862;</td>
<td class="tg-baqh">&#9633;</td>
<td class="tg-baqh">&#8862;</td>
<td class="tg-baqh">&#9633;</td>
<td class="tg-baqh">&#8862;</td>
<td class="tg-baqh">&#8862;</td>
</tr>
</table>
<p style="font-size: 16px">&#9724;</span>: Implemented, &#8862;: Doable, &#9633;: Structural changes needed</p>
---
## References

<table class="tg">
<tr>
<td>[Pentland2004]</td><td>Pentland, Alex and Fletcher, Richard and Hasson, Amir, DakNet: Rethinking Connectivity in Developing Nations, Computer, 2004</td>
</tr>
<tr>
<td>[Kannan2008]</td><td>Kannan, Kfgij and Silveira, Fernando and Taft, Nina, A Disruption-Tolerant Architecture for Secure and Efficient Disaster Response Communications, Kfall.Com, 2008</td>
</tr>
<tr>
<td>[Seth2006]</td><td>Seth, A. and Kroeker, D. and Zaharia, M. and Guo, S. and Keshav, S., Low-cost communication for rural internet kiosks using mechanical backhaul, MobiCom '06, 2006</td>
</tr>
<tr>
<td>[Zarafshan-Araki2010]</td><td>Zarafshan-Araki, Mohammad and Chin, Kwan Wu, TrainNet: A transport system for delivering non real-time data, Computer Communications, 2010</td>
</tr>
<tr>
<td>[Juang2002]</td><td>Juang, Philo and Oki, Hidekazu and Wang, Yong and Martonosi, Margaret and {Peh Li-Shiuan}, Peh and Rubenstein, Daniel, Energy-Efficient Computing for Wildlife Tracking: Design Tradeoffs and Early Experiences with ZebraNet, ASPLOS 2002</td>
</tr>
<tr>
<td>[Johansen2014]</td><td>Johansen, Tor A. and Zolich, Artur and Hansen, Torkel and Sorensen, Asgeir J., Unmanned aerial vehicle as communication relay for autonomous underwater vehicle — Field tests, IEEE Globecom Workshops, 2014</td>
</tr>
<tr>
<td>[Sharef2014]</td><td>Sharef, Baraa T. and Alsaqour, Raed A. and Ismail, Mahamod, Vehicular communication ad hoc routing protocols: A survey, Journal of Network and Computer Applications, 2014</td>
</tr>
<tr>
<td>[Burleigh2011]</td><td>Burleigh, Scott C and Birrane, Edward J., Toward a communications satellite network for humanitarian relief, ACWR '11, 2011</td>
</tr>
</table>

