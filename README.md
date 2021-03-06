# KAFCA (KAIST summarization system using FCA)


**Improving Entity Summarization via Conceptual Analysis**<br/>
*Eun-kyung Kim, Key-Sun Choi*<br/>
*Proceedings of the 1st International Workshop on EntitY REtrieval (EYRE '18) co-located with CIKM 2018, Shared Tasks @ EYRE '18*<br/>

## Abstract
This paper presents a novel approach to automatic entity summarization, which provides a smaller representative subset from a lengthy description. As a solution to this problem, we propose an entity summarization system based on Formal Concept Analysis (FCA). The effectiveness of our proposed system is illustrated by an experimental study using the Entity Summarization BenchMark, where we compare our system with six other systems. It shows that our system is superior to others with respect to F-measure performance measurements.

## Evaluation Results
We list the result of various methods in <a href='http://ws.nju.edu.cn/summarization/esbm/'>Entity Summarization BenchMark (ESBM)</a>.

**Table 1. F-measure of selected entity summarizers under their best parameter settings**<br/>
<table>
	<thead>
		<tr>
			<th rowspan="2"></th>
			<th colspan="2">DBpedia</th>
			<th colspan="2">LinkedMDB</th>
			<th colspan="2">All</th>
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
	</tr>
	<tr>
		<td>DIVERSUM [2]</td>
		<td name="td1">0.260</td>
		<td name="td2">0.522</td>
		<td name="td3">0.222</td>
		<td name="td4">0.365</td>
		<td name="td5">0.249</td>
		<td name="td6">0.477</td>
	</tr>
	<tr>
		<td>CD [3]<br></td>
		<td name="td1">0.299</td>
		<td name="td2">0.531</td>
		<td name="td3">0.215</td>
		<td name="td4">0.326</td>
		<td name="td5">0.267</td>
		<td name="td6">0.467</td>
	</tr>
	<tr>
		<td>FACES-E [4]</td>
		<td name="td1">0.285</td>
		<td name="td2">0.527</td>
		<td name="td3"><b>0.252</b></td>
		<td name="td4">0.348</td>
		<td name="td5">0.276</td>
		<td name="td6">0.476</td>
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
		<td name="td1">0.290</td>
		<td name="td2">0.498</td>
		<td name="td3">0.117</td>
		<td name="td4">0.255</td>
		<td name="td5">0.240</td>
		<td name="td6">0.428</td>
	</tr>
	<tr>
		<td><strong>KAFCA</strong></td>
		<td name="td1"><b>0.332</td>
		<td name="td2"><b>0.531</td>
		<td name="td3">0.249</td>
		<td name="td4"><b>0.399</td>
		<td name="td5"><b>0.308</td>
		<td name="td6"><b>0.493</td>
	</tr>
</table>

**Table 2. MAP of selected entity summarizers under their best parameter settings**<br/>
<table class="tablesorter" id="tb_map">
	<thead>
		<tr>
		<th rowspan="2"></th>
		<th colspan="2">DBpedia</th>
		<th colspan="2">LinkedMDB</th>
		<th colspan="2">All</th>
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
		<td name="td1">0.348</td>
		<td name="td2">0.532</td>
		<td name="td3">0.243</td>
		<td name="td4">0.337</td>
		<td name="td5">0.318</td>
		<td name="td6">0.476</td>
	</tr>
	<tr>
		<td>DIVERSUM [2]</td>
		<td name="td1">0.316</td>
		<td name="td2">0.511</td>
		<td name="td3">0.269</td>
		<td name="td4">0.388</td>
		<td name="td5">0.302</td>
		<td name="td6">0.476</td>
	</tr>
	<tr>
		<td>CD [3]<br></td>
		<td name="td1">-</td>
		<td name="td2">-</td>
		<td name="td3">-</td>
		<td name="td4">-</td>
		<td name="td5">-</td>
		<td name="td6">-</td>
	</tr>
	<tr>
	<td>FACES-E [4]</td>
		<td name="td1">0.354</td>
		<td name="td2">0.529</td>
		<td name="td3">0.258</td>
		<td name="td4">0.361</td>
		<td name="td5">0.326</td>
		<td name="td6">0.481</td>
	</tr>
	<tr>
		<td>FACES [5]</td>
		<td name="td1">0.247</td>
		<td name="td2">0.386</td>
		<td name="td3">0.140</td>
		<td name="td4">0.261</td>
		<td name="td5">0.216</td>
		<td name="td6">0.351</td>
	</tr>
	<tr>
		<td>LinkSUM [6]</td>
		<td name="td1">0.246</td>
		<td name="td2">0.386</td>
		<td name="td3">0.120</td>
		<td name="td4">0.254</td>
		<td name="td5">0.210</td>
		<td name="td6">0.348</td>
	</tr>
	<tr>
		<td><strong>KAFCA</strong></td>
		<td name="td1"><b>0.402</td>
		<td name="td2"><b>0.597</td>
		<td name="td3"><b>0.319</td>
		<td name="td4"><b>0.428</td>
		<td name="td5"><b>0.378</td>
		<td name="td6"><b>0.549</td>
	</tr>
</table>


## References
[1] Gong Cheng, Thanh Tran, Yuzhong Qu: RELIN: Relatedness and Informativeness-Based Centrality for Entity Summarization. International Semantic Web Conference (1) 2011: 114-129. <br/>
[2] Marcin Sydow, Mariusz Pikula, Ralf Schenkel: The notion of diversity in graphical entity summarisation on semantic knowledge graphs. J. Intell. Inf. Syst. 41(2): 109-149 (2013).<br/>
[3] Danyun Xu, Liang Zheng, Yuzhong Qu: CD at ENSEC 2016: Generating Characteristic and Diverse Entity Summaries. SumPre@ESWC 2016.<br/>
[4] Kalpa Gunaratna, Krishnaprasad Thirunarayan, Amit P. Sheth, Gong Cheng: Gleaning Types for Literals in RDF Triples with Application to Entity Summarization. ESWC 2016: 85-100.<br/>
[5] Kalpa Gunaratna, Krishnaprasad Thirunarayan, Amit P. Sheth: FACES: Diversity-Aware Entity Summarization Using Incremental Hierarchical Conceptual Clustering. AAAI 2015: 116-122.<br/>
[6] Andreas Thalhammer, Nelia Lasierra, Achim Rettinger: LinkSUM: Using Link Analysis to Summarize Entity Data. ICWE 2016: 244-261.<br/>

## Change Log
Aug. 30, 2018 : Initial upload. version 1.0

