# KAFCA (KAIST summarization system using FCA)


**Improving Entity Summarization via Conceptual Analysis**<br/>
*Eun-kyung Kim, Key-Sun Choi*<br/>
*Proceedings of the 1st International Workshop on EntitY REtrieval (EYRE '18) co-located with CIKM 2018, Shared Tasks @ EYRE '18*<br/>

## Abstract
This paper presents a novel approach to automatic entity summarization, which provides a smaller representative subset from a lengthy description. As a solution to this problem, we propose an entity summarization system based on Formal Concept Analysis (FCA). The effectiveness of our proposed system is illustrated by an experimental study using the Entity Summarization BenchMark, where we compare our system with six other systems. It shows that our system is superior to others with respect to F-measure performance measurements.

## Evaluation Results
We list the result of various methods in <a href='http://ws.nju.edu.cn/summarization/esbm/'>Entity Summarization BenchMark (ESBM)</a>.


<table>
	<thead>
	<tr>
	<th rowspan="2" data-sorter="false"></th>
	<th colspan="2" class="nosort">DBpedia</th>
	<th colspan="2" class="nosort">LinkedMDB</th>
	<th colspan="2" class="nosort">All</th>
	</tr>
	<tr>
	<th id="dbp1">k=5</th>
	<th id="dbp2">k=10</th>
	<th id="lmdb1">k=5</th>
	<th id="lmdb1">k=10</th>
	<th id="all1">k=5</th>
	<th id="all1">k=10</th>
	</tr>
	</thead>
	<tr>
	<td>RELIN [1]</td>
	<td name="td1">0.250</td>
	<td name="td2">0.468</td>
	<td name="td3">0.210</td>
	<td name="td4">0.260</td>
	<td name="td5">0.239</td>
	<td name="td6">0.409</td>
	<tr>
	<td>DIVERSUM [2]</td>
	<td name="td1">0.260</td>
	<td name="td2">0.522</td>
	<td name="td3">0.222</td>
	<td name="td4"><b>0.365</b></td>
	<td name="td5">0.249</td>
	<td name="td6"><b>0.477</b></td>
	</tr>
	<tr>
	<td>CD [3]<br></td>
	<td name="td1"><b>0.299</b><br><span>(&gamma;=0.47)</span></td>
	<td name="td2"><b>0.531</b><br><span>(&gamma;=0.23)</span></td>
	<td name="td3">0.215<br><span>(&gamma;=1.00)</span></td>
	<td name="td4">0.326<br><span>(&gamma;=1.00)</span></td>
	<td name="td5">0.267<br><span>(&gamma;=0.52)</span></td>
	<td name="td6">0.467<br><span>(&gamma;=0.16)</span></td>
	</tr>
	<tr>
	<td>FACES-E [4]</td>
	<td name="td1">0.285</td>
	<td name="td2">0.527</td>
	<td name="td3"><b>0.252</b></td>
	<td name="td4">0.348</td>
	<td name="td5"><b>0.276</b></td>
	<td name="td6">0.476</td>
	</tr>
	</tr>
	<tr>
	<td>FACES [5]</td>
	<td name="td1">0.272</td>
	<td name="td2">0.439</td>
	<td name="td3">0.160</td>
	<td name="td4">0.259</td>
	<td name="td5">0.240</td>
	<td name="td6">0.388</td>
	</tr>
	<tr>
	<td>LinkSUM [6]</td>
	<td name="td1">0.290<br><span>(&alpha;=0.01)</span></td>
	<td name="td2">0.498<br><span>(&alpha;=0.04)</span></td>
	<td name="td3">0.117<br><span>(&alpha;=1.00)</span></td>
	<td name="td4">0.255<br><span>(&alpha;=1.00)</span></td>
	<td name="td5">0.240<br><span>(&alpha;=0.01)</span></td>
	<td name="td6">0.428<br><span>(&alpha;=0.04)</span></td>
	</tr>
</table>

## Code
The codes are in the folder src/.


## Change Log
Aug. 30, 2018 : Initial upload. version 1.0

