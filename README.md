![Figure2_Formula3](https://github.com/nurdannkuru/PHACE/assets/68369488/1cb5d26c-01f0-4ee7-b055-d2006b615e29)# PHACE
PHACE - Phylogeny-Aware Co-Evolution Algorithm


The co-evolution trends of amino acids within or between genes offer valuable insights into protein structure and function. Existing tools for uncovering
co-evolutionary signals primarily rely on multiple sequence alignments (MSAs), often neglecting considerations of phylogenetic relatedness and shared 
evolutionary history. Here, we present a novel approach based on the substitution mapping of amino acid changes onto the phylogenetic tree. We categorize 
amino acids into two groups: 'tolerable' and 'intolerable,' assigned to each position based on the position dynamics concerning the observed amino acids. 
Amino acids deemed 'tolerable' are those observed phylogenetically independently and multiple times at a specific position, signifying the position's 
tolerance to that alteration. Gaps are regarded as a third character type, and we only take phylogenetically independent altered gap characters into 
consideration. Our algorithm is based on a tree traversal process through the nodes and computes the total amount of substitution per branch based on 
the probability differences of two groups of amino acids and gaps between neighboring nodes. To mitigate false co-evolution signals from unaligned regions, 
we employ an MSA-masking approach. When compared to tools utilizing phylogeny (e.g., CAPS and CoMap) and state-of-the-art MSA-based approaches (DCA, GaussDCA, 
PSICOV, and MIp), our method exhibits significantly superior accuracy in identifying co-evolving position pairs, as measured by statistical metrics including 
MCC, AUC, and F1 score. The success of PHACE stems from our capacity to account for the often-overlooked phylogenetic dependency.


![Uploading Figure2_Formula3.<?xml version="1.0" encoding="utf-8"?>
<!-- Generator: Adobe Illustrator 28.3.0, SVG Export Plug-In . SVG Version: 6.00 Build 0)  -->
<svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
	 viewBox="0 0 595.28 841.89" style="enable-background:new 0 0 595.28 841.89;" xml:space="preserve">
<style type="text/css">
	.st0{fill-rule:evenodd;clip-rule:evenodd;fill:url(#SVGID_1_);stroke:#180B0B;stroke-width:0.3042;stroke-miterlimit:10;}
	.st1{fill:#FDDCB4;}
	.st2{fill:#EAD1DC;stroke:#FFFFFF;stroke-width:1.4031;stroke-miterlimit:10;}
	.st3{fill:none;stroke:#010101;stroke-width:0.3181;stroke-linecap:round;stroke-linejoin:round;stroke-miterlimit:10;}
	.st4{fill:#97D3BB;}
	.st5{fill:#A285B5;}
	.st6{fill:#C2E4D8;}
	.st7{fill:#FFFFFF;}
	.st8{fill:#A8C3E0;}
	.st9{fill:#EA818B;}
	.st10{fill:#FABAA6;}
	.st11{fill:#C9A4B6;}
	.st12{fill:#9CB0B9;}
	.st13{fill:#FCDCB4;stroke:#000000;stroke-width:0.1299;stroke-miterlimit:10;}
	.st14{fill:#B3AAB8;}
	.st15{fill:none;stroke:#030202;stroke-width:0.0351;stroke-miterlimit:10;}
	.st16{fill:none;}
	.st17{font-family:'ArialMT';}
	.st18{font-size:10.9009px;}
	.st19{font-size:4.7568px;}
	.st20{fill:none;stroke:#414042;stroke-width:0.2973;stroke-miterlimit:10;}
	.st21{fill:#414042;}
	.st22{fill:#EDB47B;}
	.st23{fill:none;stroke:#000000;stroke-width:0.2729;stroke-miterlimit:10;}
	.st24{fill:#80A9B6;}
	.st25{fill:none;stroke:#443C3E;stroke-width:0.9178;stroke-miterlimit:10;}
	.st26{fill:#443C3E;}
	.st27{font-family:'MyriadPro-Regular';}
	.st28{font-size:5.9459px;}
	.st29{fill:#FFFFFF;stroke:#000000;stroke-width:0.1213;stroke-miterlimit:10;}
	.st30{fill:none;stroke:#030202;stroke-width:0.0991;stroke-miterlimit:10;}
	.st31{font-size:8.085px;}
	.st32{fill:none;stroke:#D6DADC;stroke-width:0.3032;stroke-linejoin:round;stroke-miterlimit:10;}
	.st33{fill:none;stroke:#D6DADC;stroke-width:0.4042;stroke-linejoin:round;stroke-miterlimit:10;}
	.st34{fill:#010101;}
	.st35{font-family:'Helvetica-Bold';}
	.st36{font-size:4.851px;}
	.st37{font-size:3.2634px;}
	.st38{font-family:'Helvetica';}
	.st39{filter:url(#Adobe_OpacityMaskFilter);}
	.st40{fill-rule:evenodd;clip-rule:evenodd;fill:url(#SVGID_00000148660801159511220010000001161676344780883886_);}
	
		.st41{mask:url(#SVGID_00000005261798009430258290000000696558158157094826_);fill-rule:evenodd;clip-rule:evenodd;fill:url(#SVGID_00000145768802079953563490000002546457043533066150_);}
	.st42{fill:none;stroke:#000000;stroke-width:0.2887;stroke-miterlimit:10;}
	.st43{fill:none;stroke:#030202;stroke-width:0.0497;stroke-miterlimit:10;}
</style>
<linearGradient id="SVGID_1_" gradientUnits="userSpaceOnUse" x1="670.4641" y1="154.8103" x2="487.6844" y2="154.8103">
	<stop  offset="0" style="stop-color:#FFFFFF"/>
	<stop  offset="0.025" style="stop-color:#FFFFFF"/>
	<stop  offset="0.06" style="stop-color:#FFFFFF"/>
	<stop  offset="0.095" style="stop-color:#FFFFFF"/>
	<stop  offset="0.13" style="stop-color:#FFFFFF"/>
	<stop  offset="0.2533" style="stop-color:#FFFFFF"/>
	<stop  offset="0.3767" style="stop-color:#FFFFFF"/>
	<stop  offset="0.5" style="stop-color:#FFFFFF"/>
	<stop  offset="0.6233" style="stop-color:#FFFFFF"/>
	<stop  offset="0.7467" style="stop-color:#FFFFFF"/>
	<stop  offset="0.87" style="stop-color:#FFFFFF"/>
	<stop  offset="0.905" style="stop-color:#FFFFFF"/>
	<stop  offset="0.94" style="stop-color:#FFFFFF"/>
	<stop  offset="0.975" style="stop-color:#FFFFFF"/>
	<stop  offset="1" style="stop-color:#FFFFFF"/>
</linearGradient>
<polyline class="st0" points="487.68,215.01 487.68,94.61 579.07,94.61 578.86,215.01 "/>
<rect x="263.17" y="324.24" class="st1" width="14.98" height="3.96"/>
<rect x="261.19" y="275.3" class="st1" width="33.92" height="3.96"/>
<rect x="256.24" y="106.01" class="st2" width="9.91" height="3.96"/>
<rect x="296.8" y="57.58" class="st2" width="9.91" height="3.96"/>
<rect x="291.53" y="73.73" class="st2" width="9.91" height="3.96"/>
<rect x="291.82" y="65.65" class="st2" width="9.91" height="3.96"/>
<rect x="296.8" y="49.3" class="st2" width="9.91" height="3.96"/>
<rect x="292.57" y="41.44" class="st2" width="9.91" height="3.96"/>
<rect x="293.32" y="33.37" class="st2" width="9.91" height="3.96"/>
<rect x="292.8" y="25.3" class="st2" width="9.91" height="3.96"/>
<g>
	<line class="st3" x1="17.19" y1="307.21" x2="20.64" y2="307.21"/>
	<line class="st3" x1="18.45" y1="291.07" x2="19.69" y2="291.07"/>
	<line class="st3" x1="18.45" y1="283" x2="19.69" y2="283"/>
	<line class="st3" x1="18.07" y1="299.14" x2="18.49" y2="299.14"/>
	<line class="st3" x1="53.92" y1="210.35" x2="71.67" y2="210.35"/>
	<line class="st3" x1="53.92" y1="202.28" x2="53.92" y2="202.28"/>
	<line class="st3" x1="50.79" y1="218.42" x2="56.5" y2="218.42"/>
	<line class="st3" x1="42.14" y1="226.5" x2="50.37" y2="226.5"/>
	<line class="st3" x1="82.81" y1="178.07" x2="82.81" y2="178.07"/>
	<line class="st3" x1="82.81" y1="169.99" x2="82.81" y2="169.99"/>
	<line class="st3" x1="78.67" y1="153.85" x2="81.59" y2="153.85"/>
	<line class="st3" x1="78.67" y1="145.78" x2="79.82" y2="145.78"/>
	<line class="st3" x1="78.13" y1="161.92" x2="79.91" y2="161.92"/>
	<line class="st3" x1="77.35" y1="194.21" x2="81.83" y2="194.21"/>
	<line class="st3" x1="77.35" y1="186.14" x2="85.72" y2="186.14"/>
	<line class="st3" x1="22.6" y1="258.78" x2="23.06" y2="258.78"/>
	<line class="st3" x1="22.6" y1="250.71" x2="22.6" y2="250.71"/>
	<line class="st3" x1="22.16" y1="242.64" x2="22.16" y2="242.64"/>
	<line class="st3" x1="22.16" y1="234.57" x2="22.61" y2="234.57"/>
	<line class="st3" x1="21.71" y1="266.85" x2="22.16" y2="266.85"/>
	<line class="st3" x1="20.26" y1="274.92" x2="21.11" y2="274.92"/>
	<line class="st3" x1="17.19" y1="277.49" x2="17.19" y2="277.49"/>
	<line class="st3" x1="17.19" y1="293.09" x2="18.07" y2="293.09"/>
	<line class="st3" x1="18.07" y1="287.03" x2="18.45" y2="287.03"/>
	<line class="st3" x1="17.19" y1="232.17" x2="18.82" y2="232.17"/>
	<line class="st3" x1="18.82" y1="198.5" x2="39.89" y2="198.5"/>
	<line class="st3" x1="39.89" y1="219.43" x2="42.14" y2="219.43"/>
	<line class="st3" x1="42.14" y1="212.37" x2="50.79" y2="212.37"/>
	<line class="st3" x1="50.79" y1="206.31" x2="53.92" y2="206.31"/>
	<line class="st3" x1="39.89" y1="177.56" x2="73.03" y2="177.56"/>
	<line class="st3" x1="73.03" y1="164.95" x2="76.1" y2="164.95"/>
	<line class="st3" x1="76.1" y1="174.03" x2="82.81" y2="174.03"/>
	<line class="st3" x1="76.1" y1="155.87" x2="78.13" y2="155.87"/>
	<line class="st3" x1="78.13" y1="149.81" x2="78.67" y2="149.81"/>
	<line class="st3" x1="73.03" y1="190.17" x2="77.35" y2="190.17"/>
	<line class="st3" x1="18.82" y1="265.85" x2="20.26" y2="265.85"/>
	<line class="st3" x1="20.26" y1="256.76" x2="21.71" y2="256.76"/>
	<line class="st3" x1="21.71" y1="246.68" x2="22.16" y2="246.68"/>
	<line class="st3" x1="22.16" y1="254.75" x2="22.6" y2="254.75"/>
	<line class="st3" x1="22.16" y1="238.6" x2="22.16" y2="238.6"/>
	<line class="st3" x1="17.19" y1="277.49" x2="17.19" y2="307.21"/>
	<line class="st3" x1="18.45" y1="287.03" x2="18.45" y2="291.07"/>
	<line class="st3" x1="18.45" y1="287.03" x2="18.45" y2="283"/>
	<line class="st3" x1="18.07" y1="293.09" x2="18.07" y2="299.14"/>
	<line class="st3" x1="53.92" y1="206.31" x2="53.92" y2="210.35"/>
	<line class="st3" x1="53.92" y1="206.31" x2="53.92" y2="202.28"/>
	<line class="st3" x1="50.79" y1="212.37" x2="50.79" y2="218.42"/>
	<line class="st3" x1="42.14" y1="219.43" x2="42.14" y2="226.5"/>
	<line class="st3" x1="82.81" y1="174.03" x2="82.81" y2="178.07"/>
	<line class="st3" x1="82.81" y1="174.03" x2="82.81" y2="169.99"/>
	<line class="st3" x1="78.67" y1="149.81" x2="78.67" y2="153.85"/>
	<line class="st3" x1="78.67" y1="149.81" x2="78.67" y2="145.78"/>
	<line class="st3" x1="78.13" y1="155.87" x2="78.13" y2="161.92"/>
	<line class="st3" x1="77.35" y1="190.17" x2="77.35" y2="194.21"/>
	<line class="st3" x1="77.35" y1="190.17" x2="77.35" y2="186.14"/>
	<line class="st3" x1="22.6" y1="254.75" x2="22.6" y2="258.78"/>
	<line class="st3" x1="22.6" y1="254.75" x2="22.6" y2="250.71"/>
	<line class="st3" x1="22.16" y1="238.6" x2="22.16" y2="242.64"/>
	<line class="st3" x1="22.16" y1="238.6" x2="22.16" y2="234.57"/>
	<line class="st3" x1="21.71" y1="256.76" x2="21.71" y2="266.85"/>
	<line class="st3" x1="20.26" y1="265.85" x2="20.26" y2="274.92"/>
	<line class="st3" x1="17.19" y1="277.49" x2="17.19" y2="277.49"/>
	<line class="st3" x1="17.19" y1="277.49" x2="17.19" y2="293.09"/>
	<line class="st3" x1="18.07" y1="293.09" x2="18.07" y2="287.03"/>
	<line class="st3" x1="17.19" y1="277.49" x2="17.19" y2="232.17"/>
	<line class="st3" x1="18.82" y1="232.17" x2="18.82" y2="198.5"/>
	<line class="st3" x1="39.89" y1="198.5" x2="39.89" y2="219.43"/>
	<line class="st3" x1="42.14" y1="219.43" x2="42.14" y2="212.37"/>
	<line class="st3" x1="50.79" y1="212.37" x2="50.79" y2="206.31"/>
	<line class="st3" x1="39.89" y1="198.5" x2="39.89" y2="177.56"/>
	<line class="st3" x1="73.03" y1="177.56" x2="73.03" y2="164.95"/>
	<line class="st3" x1="76.1" y1="164.95" x2="76.1" y2="174.03"/>
	<line class="st3" x1="76.1" y1="164.95" x2="76.1" y2="155.87"/>
	<line class="st3" x1="78.13" y1="155.87" x2="78.13" y2="149.81"/>
	<line class="st3" x1="73.03" y1="177.56" x2="73.03" y2="190.17"/>
	<line class="st3" x1="18.82" y1="232.17" x2="18.82" y2="265.85"/>
	<line class="st3" x1="20.26" y1="265.85" x2="20.26" y2="256.76"/>
	<line class="st3" x1="21.71" y1="256.76" x2="21.71" y2="246.68"/>
	<line class="st3" x1="22.16" y1="246.68" x2="22.16" y2="254.75"/>
	<line class="st3" x1="22.16" y1="246.68" x2="22.16" y2="238.6"/>
	<rect x="88.99" y="303.98" class="st4" width="6.93" height="6.46"/>
	<rect x="102.61" y="303.98" class="st5" width="6.93" height="6.46"/>
	<rect x="88.99" y="295.91" class="st6" width="6.93" height="6.46"/>
	<rect x="102.61" y="295.91" class="st5" width="6.93" height="6.46"/>
	<rect x="88.99" y="287.84" class="st4" width="6.93" height="6.46"/>
	<rect x="102.61" y="287.84" class="st5" width="6.93" height="6.46"/>
	<rect x="88.99" y="279.77" class="st4" width="6.93" height="6.46"/>
	<rect x="102.61" y="279.77" class="st5" width="6.93" height="6.46"/>
	<rect x="88.99" y="271.7" class="st4" width="6.93" height="6.46"/>
	<rect x="102.61" y="271.7" class="st5" width="6.93" height="6.46"/>
	<rect x="88.99" y="263.62" class="st4" width="6.93" height="6.46"/>
	<rect x="102.61" y="263.62" class="st5" width="6.93" height="6.46"/>
	<rect x="88.99" y="255.55" class="st4" width="6.93" height="6.46"/>
	<rect x="102.61" y="255.55" class="st5" width="6.93" height="6.46"/>
	<rect x="88.99" y="247.48" class="st4" width="6.93" height="6.46"/>
	<rect x="102.61" y="247.48" class="st5" width="6.93" height="6.46"/>
	<rect x="88.99" y="239.41" class="st4" width="6.93" height="6.46"/>
	<rect x="102.61" y="239.41" class="st5" width="6.93" height="6.46"/>
	<rect x="88.99" y="231.34" class="st4" width="6.93" height="6.46"/>
	<rect x="102.61" y="231.34" class="st5" width="6.93" height="6.46"/>
	<rect x="88.99" y="223.27" class="st7" width="6.93" height="6.46"/>
	<rect x="102.61" y="223.27" class="st7" width="6.93" height="6.46"/>
	<rect x="88.99" y="215.19" class="st8" width="6.93" height="6.46"/>
	<rect x="102.61" y="215.19" class="st9" width="6.93" height="6.46"/>
	<rect x="88.99" y="207.12" class="st8" width="6.93" height="6.46"/>
	<rect x="102.61" y="207.12" class="st10" width="6.93" height="6.46"/>
	<rect x="88.99" y="199.05" class="st8" width="6.93" height="6.46"/>
	<rect x="102.61" y="199.05" class="st9" width="6.93" height="6.46"/>
	<rect x="88.99" y="190.98" class="st7" width="6.93" height="6.46"/>
	<rect x="102.61" y="190.98" class="st7" width="6.93" height="6.46"/>
	<rect x="88.99" y="182.91" class="st7" width="6.93" height="6.46"/>
	<rect x="102.61" y="182.91" class="st7" width="6.93" height="6.46"/>
	<rect x="88.99" y="174.84" class="st7" width="6.93" height="6.46"/>
	<rect x="102.61" y="174.84" class="st7" width="6.93" height="6.46"/>
	<rect x="88.99" y="166.77" class="st7" width="6.93" height="6.46"/>
	<rect x="102.61" y="166.77" class="st7" width="6.93" height="6.46"/>
	<rect x="88.99" y="158.69" class="st7" width="6.93" height="6.46"/>
	<rect x="102.61" y="158.69" class="st7" width="6.93" height="6.46"/>
	<rect x="88.99" y="150.62" class="st7" width="6.93" height="6.46"/>
	<rect x="88.99" y="142.55" class="st7" width="6.93" height="6.46"/>
</g>
<g>
	<rect x="180.72" y="183.41" class="st11" width="6.92" height="6.46"/>
	<rect x="180.72" y="175.34" class="st12" width="6.92" height="6.46"/>
	<rect x="180.72" y="167.27" class="st11" width="6.92" height="6.46"/>
	<rect x="180.72" y="159.19" class="st11" width="6.92" height="6.46"/>
	<rect x="180.72" y="151.12" class="st11" width="6.92" height="6.46"/>
	<rect x="180.72" y="143.05" class="st11" width="6.92" height="6.46"/>
	<rect x="180.72" y="134.98" class="st11" width="6.92" height="6.46"/>
	<rect x="180.72" y="126.91" class="st11" width="6.92" height="6.46"/>
	<rect x="180.72" y="118.84" class="st11" width="6.92" height="6.46"/>
	<rect x="180.72" y="110.76" class="st11" width="6.92" height="6.46"/>
	<rect x="180.72" y="102.69" class="st7" width="6.92" height="6.46"/>
	<rect x="180.72" y="94.62" class="st12" width="6.92" height="6.46"/>
	<rect x="180.72" y="86.55" class="st12" width="6.92" height="6.46"/>
	<rect x="180.72" y="78.48" class="st12" width="6.92" height="6.46"/>
	<rect x="180.72" y="70.41" class="st7" width="6.92" height="6.46"/>
	<rect x="180.72" y="62.33" class="st7" width="6.92" height="6.46"/>
	<rect x="180.72" y="54.26" class="st7" width="6.92" height="6.46"/>
	<rect x="180.72" y="46.19" class="st7" width="6.92" height="6.46"/>
</g>
<rect x="210.67" y="21.95" class="st7" width="5.14" height="5.14"/>
<rect x="209.73" y="21.95" class="st13" width="6.08" height="6.28"/>
<rect x="209.73" y="29.85" class="st12" width="6.08" height="5.76"/>
<rect x="215.29" y="51.57" class="st7" width="5.14" height="5.14"/>
<rect x="209.85" y="37.22" class="st11" width="5.96" height="5.99"/>
<g>
	<rect x="180.71" y="402.47" class="st14" width="6.93" height="6.46"/>
	<rect x="193.59" y="402.47" class="st14" width="6.93" height="6.46"/>
	<rect x="180.71" y="394.4" class="st14" width="6.93" height="6.46"/>
	<rect x="193.59" y="394.4" class="st14" width="6.93" height="6.46"/>
	<rect x="180.71" y="386.33" class="st14" width="6.93" height="6.46"/>
	<rect x="193.59" y="386.33" class="st14" width="6.93" height="6.46"/>
	<rect x="180.71" y="378.26" class="st14" width="6.93" height="6.46"/>
	<rect x="193.59" y="378.26" class="st14" width="6.93" height="6.46"/>
	<rect x="180.71" y="370.19" class="st14" width="6.93" height="6.46"/>
	<rect x="193.59" y="370.19" class="st14" width="6.93" height="6.46"/>
	<rect x="180.71" y="362.12" class="st14" width="6.93" height="6.46"/>
	<rect x="193.59" y="362.12" class="st14" width="6.93" height="6.46"/>
	<rect x="180.71" y="354.04" class="st14" width="6.93" height="6.46"/>
	<rect x="193.59" y="354.04" class="st14" width="6.93" height="6.46"/>
	<rect x="180.71" y="345.97" class="st14" width="6.93" height="6.46"/>
	<rect x="193.59" y="345.97" class="st14" width="6.93" height="6.46"/>
	<rect x="180.71" y="337.9" class="st14" width="6.93" height="6.46"/>
	<rect x="193.59" y="337.9" class="st14" width="6.93" height="6.46"/>
	<rect x="180.71" y="329.83" class="st14" width="6.93" height="6.46"/>
	<rect x="193.59" y="329.83" class="st14" width="6.93" height="6.46"/>
	<rect x="180.71" y="321.76" class="st1" width="6.93" height="6.46"/>
	<rect x="193.59" y="321.76" class="st1" width="6.93" height="6.46"/>
	<rect x="180.71" y="313.69" class="st14" width="6.93" height="6.46"/>
	<rect x="193.59" y="313.69" class="st14" width="6.93" height="6.46"/>
	<rect x="180.71" y="305.61" class="st14" width="6.93" height="6.46"/>
	<rect x="193.59" y="305.61" class="st14" width="6.93" height="6.46"/>
	<rect x="180.71" y="297.54" class="st14" width="6.93" height="6.46"/>
	<rect x="193.59" y="297.54" class="st14" width="6.93" height="6.46"/>
	<rect x="180.71" y="289.47" class="st1" width="6.93" height="6.46"/>
	<rect x="193.59" y="289.47" class="st1" width="6.93" height="6.46"/>
	<rect x="180.71" y="281.4" class="st1" width="6.93" height="6.46"/>
	<rect x="193.59" y="281.4" class="st1" width="6.93" height="6.46"/>
	<rect x="180.71" y="273.33" class="st1" width="6.93" height="6.46"/>
	<rect x="193.59" y="273.33" class="st1" width="6.93" height="6.46"/>
	<rect x="180.71" y="265.26" class="st1" width="6.93" height="6.46"/>
	<rect x="193.59" y="265.26" class="st1" width="6.93" height="6.46"/>
	<rect x="180.71" y="257.18" class="st1" width="6.93" height="6.46"/>
	<rect x="193.59" y="257.18" class="st1" width="6.93" height="6.46"/>
	<rect x="180.71" y="249.21" class="st1" width="6.93" height="6.46"/>
	<rect x="193.59" y="249.11" class="st1" width="6.93" height="6.46"/>
	<rect x="180.71" y="241.22" class="st1" width="6.93" height="6.46"/>
	<rect x="193.59" y="241.04" class="st1" width="6.93" height="6.46"/>
</g>
<rect x="88.99" y="142.55" class="st15" width="6.93" height="167.89"/>
<rect x="223.56" y="222.16" class="st16" width="37.7" height="10.93"/>
<text transform="matrix(1 0 0 1 223.559 229.9683)" class="st17 st18">MSA 2</text>
<rect x="227.57" y="3.71" class="st16" width="37.7" height="10.93"/>
<text transform="matrix(1 0 0 1 227.5639 11.5118)" class="st17 st18">MSA 1</text>
<line class="st3" x1="232.14" y1="188.71" x2="235.58" y2="188.71"/>
<line class="st3" x1="233.4" y1="172.57" x2="234.63" y2="172.57"/>
<line class="st3" x1="233.4" y1="164.5" x2="234.64" y2="164.5"/>
<line class="st3" x1="233.01" y1="180.64" x2="233.43" y2="180.64"/>
<line class="st3" x1="268.87" y1="91.85" x2="286.62" y2="91.85"/>
<line class="st3" x1="268.87" y1="83.78" x2="268.87" y2="83.78"/>
<line class="st3" x1="265.73" y1="99.92" x2="271.44" y2="99.92"/>
<line class="st3" x1="257.09" y1="107.99" x2="265.31" y2="107.99"/>
<line class="st3" x1="297.75" y1="59.57" x2="297.75" y2="59.57"/>
<line class="st3" x1="297.75" y1="51.49" x2="297.75" y2="51.49"/>
<line class="st3" x1="293.62" y1="35.35" x2="296.54" y2="35.35"/>
<line class="st3" x1="293.62" y1="27.28" x2="294.77" y2="27.28"/>
<line class="st3" x1="293.08" y1="43.42" x2="294.86" y2="43.42"/>
<line class="st3" x1="292.3" y1="75.71" x2="296.77" y2="75.71"/>
<line class="st3" x1="292.3" y1="67.64" x2="300.67" y2="67.64"/>
<line class="st3" x1="237.55" y1="140.28" x2="238" y2="140.28"/>
<line class="st3" x1="237.55" y1="132.21" x2="237.55" y2="132.21"/>
<line class="st3" x1="237.1" y1="124.14" x2="237.1" y2="124.14"/>
<line class="st3" x1="237.1" y1="116.07" x2="237.56" y2="116.07"/>
<line class="st3" x1="236.65" y1="148.35" x2="237.11" y2="148.35"/>
<line class="st3" x1="235.2" y1="156.42" x2="236.05" y2="156.42"/>
<line class="st3" x1="232.14" y1="158.99" x2="232.14" y2="158.99"/>
<line class="st3" x1="232.14" y1="174.59" x2="233.01" y2="174.59"/>
<line class="st3" x1="233.01" y1="168.53" x2="233.4" y2="168.53"/>
<line class="st3" x1="232.14" y1="113.67" x2="233.76" y2="113.67"/>
<line class="st3" x1="233.76" y1="80" x2="254.83" y2="80"/>
<line class="st3" x1="254.83" y1="100.93" x2="257.09" y2="100.93"/>
<line class="st3" x1="257.09" y1="93.87" x2="265.73" y2="93.87"/>
<line class="st3" x1="265.73" y1="87.81" x2="268.87" y2="87.81"/>
<line class="st3" x1="254.83" y1="59.06" x2="287.97" y2="59.06"/>
<line class="st3" x1="287.97" y1="46.45" x2="291.04" y2="46.45"/>
<line class="st3" x1="291.04" y1="55.53" x2="297.75" y2="55.53"/>
<line class="st3" x1="291.04" y1="37.37" x2="293.08" y2="37.37"/>
<line class="st3" x1="293.08" y1="31.31" x2="293.62" y2="31.31"/>
<line class="st3" x1="287.97" y1="71.67" x2="292.3" y2="71.67"/>
<line class="st3" x1="233.76" y1="147.35" x2="235.2" y2="147.35"/>
<line class="st3" x1="235.2" y1="138.26" x2="236.65" y2="138.26"/>
<line class="st3" x1="236.65" y1="128.18" x2="237.1" y2="128.18"/>
<line class="st3" x1="237.1" y1="136.25" x2="237.55" y2="136.25"/>
<line class="st3" x1="237.1" y1="120.1" x2="237.1" y2="120.1"/>
<line class="st3" x1="232.14" y1="158.99" x2="232.14" y2="188.71"/>
<line class="st3" x1="233.4" y1="168.53" x2="233.4" y2="172.57"/>
<line class="st3" x1="233.4" y1="168.53" x2="233.4" y2="164.5"/>
<line class="st3" x1="233.01" y1="174.59" x2="233.01" y2="180.64"/>
<line class="st3" x1="268.87" y1="87.81" x2="268.87" y2="91.85"/>
<line class="st3" x1="268.87" y1="87.81" x2="268.87" y2="83.78"/>
<line class="st3" x1="265.73" y1="93.87" x2="265.73" y2="99.92"/>
<line class="st3" x1="257.09" y1="100.93" x2="257.09" y2="107.99"/>
<line class="st3" x1="297.75" y1="55.53" x2="297.75" y2="59.57"/>
<line class="st3" x1="297.75" y1="55.53" x2="297.75" y2="51.49"/>
<line class="st3" x1="293.62" y1="31.31" x2="293.62" y2="35.35"/>
<line class="st3" x1="293.62" y1="31.31" x2="293.62" y2="27.28"/>
<line class="st3" x1="293.08" y1="37.37" x2="293.08" y2="43.42"/>
<line class="st3" x1="292.3" y1="71.67" x2="292.3" y2="75.71"/>
<line class="st3" x1="292.3" y1="71.67" x2="292.3" y2="67.64"/>
<line class="st3" x1="237.55" y1="136.25" x2="237.55" y2="140.28"/>
<line class="st3" x1="237.55" y1="136.25" x2="237.55" y2="132.21"/>
<line class="st3" x1="237.1" y1="120.1" x2="237.1" y2="124.14"/>
<line class="st3" x1="237.1" y1="120.1" x2="237.1" y2="116.07"/>
<line class="st3" x1="236.65" y1="138.26" x2="236.65" y2="148.35"/>
<line class="st3" x1="235.2" y1="147.35" x2="235.2" y2="156.42"/>
<line class="st3" x1="232.14" y1="158.99" x2="232.14" y2="158.99"/>
<line class="st3" x1="232.14" y1="158.99" x2="232.14" y2="174.59"/>
<line class="st3" x1="233.01" y1="174.59" x2="233.01" y2="168.53"/>
<line class="st3" x1="232.14" y1="158.99" x2="232.14" y2="113.67"/>
<line class="st3" x1="233.76" y1="113.67" x2="233.76" y2="80"/>
<line class="st3" x1="254.83" y1="80" x2="254.83" y2="100.93"/>
<line class="st3" x1="257.09" y1="100.93" x2="257.09" y2="93.87"/>
<line class="st3" x1="265.73" y1="93.87" x2="265.73" y2="87.81"/>
<line class="st3" x1="254.83" y1="80" x2="254.83" y2="59.06"/>
<line class="st3" x1="287.97" y1="59.06" x2="287.97" y2="46.45"/>
<line class="st3" x1="291.04" y1="46.45" x2="291.04" y2="55.53"/>
<line class="st3" x1="291.04" y1="46.45" x2="291.04" y2="37.37"/>
<line class="st3" x1="293.08" y1="37.37" x2="293.08" y2="31.31"/>
<line class="st3" x1="287.97" y1="59.06" x2="287.97" y2="71.67"/>
<line class="st3" x1="233.76" y1="113.67" x2="233.76" y2="147.35"/>
<line class="st3" x1="235.2" y1="147.35" x2="235.2" y2="138.26"/>
<line class="st3" x1="236.65" y1="138.26" x2="236.65" y2="128.18"/>
<line class="st3" x1="237.1" y1="128.18" x2="237.1" y2="136.25"/>
<line class="st3" x1="237.1" y1="128.18" x2="237.1" y2="120.1"/>
<line class="st3" x1="238.49" y1="406.94" x2="241.94" y2="406.94"/>
<line class="st3" x1="239.75" y1="390.79" x2="240.99" y2="390.79"/>
<line class="st3" x1="239.75" y1="382.72" x2="240.99" y2="382.72"/>
<line class="st3" x1="239.37" y1="398.86" x2="239.78" y2="398.86"/>
<line class="st3" x1="275.22" y1="310.08" x2="292.97" y2="310.08"/>
<line class="st3" x1="275.22" y1="302.01" x2="275.22" y2="302.01"/>
<line class="st3" x1="272.09" y1="318.15" x2="277.8" y2="318.15"/>
<line class="st3" x1="263.44" y1="326.22" x2="271.66" y2="326.22"/>
<line class="st3" x1="304.11" y1="277.79" x2="304.11" y2="277.79"/>
<line class="st3" x1="304.11" y1="269.72" x2="304.11" y2="269.72"/>
<line class="st3" x1="299.97" y1="253.58" x2="302.89" y2="253.58"/>
<line class="st3" x1="299.97" y1="245.5" x2="301.12" y2="245.5"/>
<line class="st3" x1="299.43" y1="261.65" x2="301.21" y2="261.65"/>
<line class="st3" x1="298.65" y1="293.93" x2="303.12" y2="293.93"/>
<line class="st3" x1="298.65" y1="285.86" x2="307.02" y2="285.86"/>
<line class="st3" x1="243.9" y1="358.51" x2="244.35" y2="358.51"/>
<line class="st3" x1="243.9" y1="350.44" x2="243.9" y2="350.44"/>
<line class="st3" x1="243.45" y1="342.36" x2="243.45" y2="342.36"/>
<line class="st3" x1="243.45" y1="334.29" x2="243.91" y2="334.29"/>
<line class="st3" x1="243.01" y1="366.58" x2="243.46" y2="366.58"/>
<line class="st3" x1="241.56" y1="374.65" x2="242.41" y2="374.65"/>
<line class="st3" x1="238.49" y1="377.22" x2="238.49" y2="377.22"/>
<line class="st3" x1="238.49" y1="392.81" x2="239.37" y2="392.81"/>
<line class="st3" x1="239.37" y1="386.76" x2="239.75" y2="386.76"/>
<line class="st3" x1="238.49" y1="331.9" x2="240.12" y2="331.9"/>
<line class="st3" x1="240.12" y1="298.22" x2="261.19" y2="298.22"/>
<line class="st3" x1="261.19" y1="319.16" x2="263.44" y2="319.16"/>
<line class="st3" x1="263.44" y1="312.1" x2="272.09" y2="312.1"/>
<line class="st3" x1="272.09" y1="306.04" x2="275.22" y2="306.04"/>
<line class="st3" x1="261.19" y1="277.29" x2="294.32" y2="277.29"/>
<line class="st3" x1="294.32" y1="264.67" x2="297.4" y2="264.67"/>
<line class="st3" x1="297.4" y1="273.75" x2="304.11" y2="273.75"/>
<line class="st3" x1="297.4" y1="255.59" x2="299.43" y2="255.59"/>
<line class="st3" x1="299.43" y1="249.54" x2="299.97" y2="249.54"/>
<line class="st3" x1="294.32" y1="289.9" x2="298.65" y2="289.9"/>
<line class="st3" x1="240.12" y1="365.57" x2="241.56" y2="365.57"/>
<line class="st3" x1="241.56" y1="356.49" x2="243.01" y2="356.49"/>
<line class="st3" x1="243.01" y1="346.4" x2="243.45" y2="346.4"/>
<line class="st3" x1="243.45" y1="354.47" x2="243.9" y2="354.47"/>
<line class="st3" x1="243.45" y1="338.33" x2="243.45" y2="338.33"/>
<line class="st3" x1="238.49" y1="377.22" x2="238.49" y2="406.94"/>
<line class="st3" x1="239.75" y1="386.76" x2="239.75" y2="390.79"/>
<line class="st3" x1="239.75" y1="386.76" x2="239.75" y2="382.72"/>
<line class="st3" x1="239.37" y1="392.81" x2="239.37" y2="398.86"/>
<line class="st3" x1="275.22" y1="306.04" x2="275.22" y2="310.08"/>
<line class="st3" x1="275.22" y1="306.04" x2="275.22" y2="302.01"/>
<line class="st3" x1="272.09" y1="312.1" x2="272.09" y2="318.15"/>
<line class="st3" x1="263.44" y1="319.16" x2="263.44" y2="326.22"/>
<line class="st3" x1="304.11" y1="273.75" x2="304.11" y2="277.79"/>
<line class="st3" x1="304.11" y1="273.75" x2="304.11" y2="269.72"/>
<line class="st3" x1="299.97" y1="249.54" x2="299.97" y2="253.58"/>
<line class="st3" x1="299.97" y1="249.54" x2="299.97" y2="245.5"/>
<line class="st3" x1="299.43" y1="255.59" x2="299.43" y2="261.65"/>
<line class="st3" x1="298.65" y1="289.9" x2="298.65" y2="293.93"/>
<line class="st3" x1="298.65" y1="289.9" x2="298.65" y2="285.86"/>
<line class="st3" x1="243.9" y1="354.47" x2="243.9" y2="358.51"/>
<line class="st3" x1="243.9" y1="354.47" x2="243.9" y2="350.44"/>
<line class="st3" x1="243.45" y1="338.33" x2="243.45" y2="342.36"/>
<line class="st3" x1="243.45" y1="338.33" x2="243.45" y2="334.29"/>
<line class="st3" x1="243.01" y1="356.49" x2="243.01" y2="366.58"/>
<line class="st3" x1="241.56" y1="365.57" x2="241.56" y2="374.65"/>
<line class="st3" x1="238.49" y1="377.22" x2="238.49" y2="377.22"/>
<line class="st3" x1="238.49" y1="377.22" x2="238.49" y2="392.81"/>
<line class="st3" x1="239.37" y1="392.81" x2="239.37" y2="386.76"/>
<line class="st3" x1="238.49" y1="377.22" x2="238.49" y2="331.9"/>
<line class="st3" x1="240.12" y1="331.9" x2="240.12" y2="298.22"/>
<line class="st3" x1="261.19" y1="298.22" x2="261.19" y2="319.16"/>
<line class="st3" x1="263.44" y1="319.16" x2="263.44" y2="312.1"/>
<line class="st3" x1="272.09" y1="312.1" x2="272.09" y2="306.04"/>
<line class="st3" x1="261.19" y1="298.22" x2="261.19" y2="277.29"/>
<line class="st3" x1="294.32" y1="277.29" x2="294.32" y2="264.67"/>
<line class="st3" x1="297.4" y1="264.67" x2="297.4" y2="273.75"/>
<line class="st3" x1="297.4" y1="264.67" x2="297.4" y2="255.59"/>
<line class="st3" x1="299.43" y1="255.59" x2="299.43" y2="249.54"/>
<line class="st3" x1="294.32" y1="277.29" x2="294.32" y2="289.9"/>
<line class="st3" x1="240.12" y1="331.9" x2="240.12" y2="365.57"/>
<line class="st3" x1="241.56" y1="365.57" x2="241.56" y2="356.49"/>
<line class="st3" x1="243.01" y1="356.49" x2="243.01" y2="346.4"/>
<line class="st3" x1="243.45" y1="346.4" x2="243.45" y2="354.47"/>
<line class="st3" x1="243.45" y1="346.4" x2="243.45" y2="338.33"/>
<g>
	<path class="st12" d="M262.9,93.87c0,0.82-0.67,1.49-1.49,1.49c-0.82,0-1.49-0.67-1.49-1.49c0-0.82,0.67-1.49,1.49-1.49
		C262.23,92.38,262.9,93.05,262.9,93.87"/>
</g>
<path class="st12" d="M271.73,169.2c0,0.83-0.67,1.5-1.5,1.5c-0.83,0-1.5-0.67-1.5-1.5c0-0.83,0.67-1.5,1.5-1.5
	C271.06,167.7,271.73,168.37,271.73,169.2"/>
<text transform="matrix(1 0 0 1 273.8627 170.7847)" class="st17 st19">C     A</text>
<g>
	<g>
		<line class="st20" x1="278.31" y1="169.2" x2="281.34" y2="169.2"/>
		<g>
			<polygon class="st21" points="281.04,170.24 282.84,169.2 281.04,168.16 			"/>
		</g>
	</g>
</g>
<g>
	<g>
		<line class="st20" x1="282.56" y1="176.37" x2="285.59" y2="176.37"/>
		<g>
			<polygon class="st21" points="285.29,177.4 287.09,176.37 285.29,175.33 			"/>
		</g>
	</g>
</g>
<rect x="263.78" y="173.87" class="st2" width="9.91" height="3.96"/>
<text transform="matrix(1 0 0 1 273.8627 177.9517)" class="st17 st19">C/A     -</text>
<text transform="matrix(1 0 0 1 289.6313 399.1021)" class="st17 st19">C     G</text>
<rect x="274.06" y="395.65" class="st1" width="14.98" height="3.96"/>
<g>
	<g>
		<line class="st20" x1="293.92" y1="397.63" x2="296.95" y2="397.63"/>
		<g>
			<polygon class="st21" points="296.65,398.67 298.45,397.63 296.65,396.59 			"/>
		</g>
	</g>
</g>
<rect x="209.75" y="241.63" class="st7" width="5.14" height="5.14"/>
<rect x="209.96" y="241.84" class="st14" width="6.08" height="6.48"/>
<rect x="209.96" y="249.98" class="st1" width="6.08" height="5.59"/>
<text transform="matrix(1 0 0 1 217.7895 254.8433)" class="st17 st19">G</text>
<text transform="matrix(1 0 0 1 217.3188 246.7701)" class="st17 st19">C</text>
<text transform="matrix(1 0 0 1 216.7299 42.2179)" class="st17 st19">C</text>
<text transform="matrix(1 0 0 1 216.9682 34.1471)" class="st17 st19">A</text>
<text transform="matrix(1 0 0 1 217.4438 26.4444)" class="st17 st19">-</text>
<line class="st3" x1="351.87" y1="227.68" x2="355.32" y2="227.68"/>
<line class="st3" x1="353.13" y1="211.54" x2="354.36" y2="211.54"/>
<line class="st3" x1="353.13" y1="203.47" x2="354.37" y2="203.47"/>
<line class="st3" x1="352.74" y1="219.61" x2="353.16" y2="219.61"/>
<line class="st3" x1="388.6" y1="130.82" x2="406.35" y2="130.82"/>
<line class="st3" x1="388.6" y1="122.75" x2="388.6" y2="122.75"/>
<line class="st3" x1="385.46" y1="138.9" x2="391.18" y2="138.9"/>
<line class="st3" x1="376.82" y1="146.97" x2="385.04" y2="146.97"/>
<line class="st3" x1="417.49" y1="98.54" x2="417.49" y2="98.54"/>
<line class="st3" x1="417.49" y1="90.47" x2="417.49" y2="90.47"/>
<line class="st3" x1="413.35" y1="74.32" x2="416.27" y2="74.32"/>
<line class="st3" x1="413.35" y1="66.25" x2="414.5" y2="66.25"/>
<line class="st3" x1="412.81" y1="82.39" x2="414.59" y2="82.39"/>
<line class="st3" x1="412.03" y1="114.68" x2="416.5" y2="114.68"/>
<line class="st3" x1="412.03" y1="106.61" x2="420.4" y2="106.61"/>
<line class="st3" x1="357.28" y1="179.25" x2="357.73" y2="179.25"/>
<line class="st3" x1="357.28" y1="171.18" x2="357.28" y2="171.18"/>
<line class="st3" x1="356.83" y1="163.11" x2="356.83" y2="163.11"/>
<line class="st3" x1="356.83" y1="155.04" x2="357.29" y2="155.04"/>
<line class="st3" x1="356.39" y1="187.33" x2="356.84" y2="187.33"/>
<line class="st3" x1="354.94" y1="195.4" x2="355.79" y2="195.4"/>
<line class="st3" x1="351.87" y1="197.96" x2="351.87" y2="197.96"/>
<line class="st3" x1="351.87" y1="213.56" x2="352.74" y2="213.56"/>
<line class="st3" x1="352.74" y1="207.51" x2="353.13" y2="207.51"/>
<line class="st3" x1="351.87" y1="152.64" x2="353.5" y2="152.64"/>
<line class="st3" x1="353.5" y1="118.97" x2="374.57" y2="118.97"/>
<line class="st3" x1="374.57" y1="139.9" x2="376.82" y2="139.9"/>
<line class="st3" x1="376.82" y1="132.84" x2="385.46" y2="132.84"/>
<line class="st3" x1="385.46" y1="126.79" x2="388.6" y2="126.79"/>
<line class="st3" x1="374.57" y1="98.03" x2="407.7" y2="98.03"/>
<line class="st3" x1="407.7" y1="85.42" x2="410.78" y2="85.42"/>
<line class="st3" x1="410.78" y1="94.5" x2="417.49" y2="94.5"/>
<line class="st3" x1="410.78" y1="76.34" x2="412.81" y2="76.34"/>
<line class="st3" x1="412.81" y1="70.29" x2="413.35" y2="70.29"/>
<line class="st3" x1="407.7" y1="110.64" x2="412.03" y2="110.64"/>
<line class="st3" x1="353.5" y1="186.32" x2="354.94" y2="186.32"/>
<line class="st3" x1="354.94" y1="177.24" x2="356.39" y2="177.24"/>
<line class="st3" x1="356.39" y1="167.15" x2="356.83" y2="167.15"/>
<line class="st3" x1="356.83" y1="175.22" x2="357.28" y2="175.22"/>
<line class="st3" x1="356.83" y1="159.08" x2="356.83" y2="159.08"/>
<line class="st3" x1="351.87" y1="197.96" x2="351.87" y2="227.68"/>
<line class="st3" x1="353.13" y1="207.51" x2="353.13" y2="211.54"/>
<line class="st3" x1="353.13" y1="207.51" x2="353.13" y2="203.47"/>
<line class="st3" x1="352.74" y1="213.56" x2="352.74" y2="219.61"/>
<line class="st3" x1="388.6" y1="126.79" x2="388.6" y2="130.82"/>
<line class="st3" x1="388.6" y1="126.79" x2="388.6" y2="122.75"/>
<line class="st3" x1="385.46" y1="132.84" x2="385.46" y2="138.9"/>
<line class="st3" x1="376.82" y1="139.9" x2="376.82" y2="146.97"/>
<line class="st3" x1="417.49" y1="94.5" x2="417.49" y2="98.54"/>
<line class="st3" x1="417.49" y1="94.5" x2="417.49" y2="90.47"/>
<line class="st3" x1="413.35" y1="70.29" x2="413.35" y2="74.32"/>
<line class="st3" x1="413.35" y1="70.29" x2="413.35" y2="66.25"/>
<line class="st3" x1="412.81" y1="76.34" x2="412.81" y2="82.39"/>
<line class="st3" x1="412.03" y1="110.64" x2="412.03" y2="114.68"/>
<line class="st3" x1="412.03" y1="110.64" x2="412.03" y2="106.61"/>
<line class="st3" x1="357.28" y1="175.22" x2="357.28" y2="179.25"/>
<line class="st3" x1="357.28" y1="175.22" x2="357.28" y2="171.18"/>
<line class="st3" x1="356.83" y1="159.08" x2="356.83" y2="163.11"/>
<line class="st3" x1="356.83" y1="159.08" x2="356.83" y2="155.04"/>
<line class="st3" x1="356.39" y1="177.24" x2="356.39" y2="187.33"/>
<line class="st3" x1="354.94" y1="186.32" x2="354.94" y2="195.4"/>
<line class="st3" x1="351.87" y1="197.96" x2="351.87" y2="197.96"/>
<line class="st3" x1="351.87" y1="197.96" x2="351.87" y2="213.56"/>
<line class="st3" x1="352.74" y1="213.56" x2="352.74" y2="207.51"/>
<line class="st3" x1="351.87" y1="197.96" x2="351.87" y2="152.64"/>
<line class="st3" x1="353.5" y1="152.64" x2="353.5" y2="118.97"/>
<line class="st3" x1="374.57" y1="118.97" x2="374.57" y2="139.9"/>
<line class="st3" x1="376.82" y1="139.9" x2="376.82" y2="132.84"/>
<line class="st3" x1="385.46" y1="132.84" x2="385.46" y2="126.79"/>
<line class="st3" x1="374.57" y1="118.97" x2="374.57" y2="98.03"/>
<line class="st3" x1="407.7" y1="98.03" x2="407.7" y2="85.42"/>
<line class="st3" x1="410.78" y1="85.42" x2="410.78" y2="94.5"/>
<line class="st3" x1="410.78" y1="85.42" x2="410.78" y2="76.34"/>
<line class="st3" x1="412.81" y1="76.34" x2="412.81" y2="70.29"/>
<line class="st3" x1="407.7" y1="98.03" x2="407.7" y2="110.64"/>
<line class="st3" x1="353.5" y1="152.64" x2="353.5" y2="186.32"/>
<line class="st3" x1="354.94" y1="186.32" x2="354.94" y2="177.24"/>
<line class="st3" x1="356.39" y1="177.24" x2="356.39" y2="167.15"/>
<line class="st3" x1="356.83" y1="167.15" x2="356.83" y2="175.22"/>
<line class="st3" x1="356.83" y1="167.15" x2="356.83" y2="159.08"/>
<g>
	<path class="st22" d="M388.66,98.03c0-1.37,1.11-2.48,2.48-2.48c1.37,0,2.48,1.11,2.48,2.48c0,1.37-1.11,2.48-2.48,2.48
		C389.77,100.51,388.66,99.4,388.66,98.03"/>
</g>
<path class="st23" d="M139.64,323.34H12.11c-5.75,0-10.42-4.66-10.42-10.42V135.73c0-5.75,4.66-10.42,10.42-10.42h127.53
	c5.75,0,10.42,4.66,10.42,10.42v177.19C150.06,318.68,145.39,323.34,139.64,323.34z"/>
<g>
	<path class="st24" d="M378.66,132.84c0-1.37,1.11-2.48,2.48-2.48c1.37,0,2.48,1.11,2.48,2.48c0,1.37-1.11,2.48-2.48,2.48
		C379.77,135.32,378.66,134.21,378.66,132.84"/>
</g>
<g>
	<path class="st22" d="M378.66,146.97c0-1.37,1.11-2.48,2.48-2.48c1.37,0,2.48,1.11,2.48,2.48c0,1.37-1.11,2.48-2.48,2.48
		C379.77,149.44,378.66,148.34,378.66,146.97"/>
</g>
<g>
	<g>
		<line class="st25" x1="152.67" y1="166.45" x2="167.15" y2="166.51"/>
		<g>
			<polygon class="st26" points="166.61,168.33 169.79,166.51 166.63,164.67 			"/>
		</g>
	</g>
</g>
<text transform="matrix(1 0 0 1 370.5907 75.8521)"><tspan x="0" y="0" class="st22 st27 st28">Dif1: 0.572</tspan><tspan x="0" y="7.14" class="st22 st27 st28">Dif2: 0.572</tspan><tspan x="-3.77" y="14.27" class="st22 st27 st28">Length: 0.594</tspan></text>
<text transform="matrix(1 0 0 1 372.0126 157.4)"><tspan x="0" y="0" class="st22 st27 st28">Dif1: 0.569</tspan><tspan x="0" y="7.14" class="st22 st27 st28">Dif2: 0.569</tspan><tspan x="-3.77" y="14.27" class="st22 st27 st28">Length: 0.147</tspan></text>
<text transform="matrix(1 0 0 1 398.7626 128.8053)"><tspan x="0" y="0" class="st24 st27 st28">Dif1: 0.642</tspan><tspan x="0" y="7.14" class="st24 st27 st28">Dif2: 0.644</tspan><tspan x="-3.77" y="14.27" class="st24 st27 st28">Length: 0.377</tspan></text>
<rect x="460.93" y="61.32" class="st7" width="5.14" height="5.14"/>
<rect x="459.99" y="61.32" class="st13" width="6.08" height="6.28"/>
<rect x="459.99" y="69.21" class="st12" width="6.08" height="5.76"/>
<rect x="460.11" y="76.58" class="st11" width="5.96" height="5.99"/>
<rect x="118.36" y="143.27" class="st7" width="5.14" height="5.14"/>
<rect x="117.88" y="143.67" class="st29" width="6.08" height="5.48"/>
<text transform="matrix(1 0 0 1 125.9125 147.3746)" class="st17 st19">-</text>
<rect x="117.88" y="157.32" class="st4" width="6.08" height="5.62"/>
<rect x="117.88" y="150.42" class="st5" width="6.08" height="5.62"/>
<rect x="117.88" y="164.09" class="st6" width="6.08" height="5.74"/>
<rect x="117.88" y="171.03" class="st10" width="6.08" height="5.7"/>
<rect x="117.88" y="177.63" class="st9" width="6.08" height="5.81"/>
<rect x="117.88" y="184.45" class="st8" width="6.08" height="5.81"/>
<text transform="matrix(0.8933 0 0 1 125.9779 155.2681)" class="st17 st19">I</text>
<text transform="matrix(0.8933 0 0 1 125.5941 169.5308)" class="st17 st19">M</text>
<text transform="matrix(1 0 0 1 125.6127 175.6959)" class="st17 st19">P</text>
<text transform="matrix(0.8933 0 0 1 125.5941 182.7125)" class="st17 st19">R</text>
<text transform="matrix(0.8933 0 0 1 125.5941 189.4478)" class="st17 st19">V</text>
<text transform="matrix(0.8933 0 0 1 125.6127 162.1959)" class="st17 st19">L</text>
<g>
	<path class="st24" d="M372.73,229.44c0-1.37,1.11-2.48,2.48-2.48c1.37,0,2.48,1.11,2.48,2.48c0,1.37-1.11,2.48-2.48,2.48
		C373.84,231.91,372.73,230.8,372.73,229.44"/>
</g>
<text transform="matrix(1 0 0 1 379.6288 231.3648)" class="st17 st19">C     A</text>
<g>
	<g>
		<line class="st20" x1="384.08" y1="229.78" x2="387.11" y2="229.78"/>
		<g>
			<polygon class="st21" points="386.81,230.82 388.6,229.78 386.81,228.74 			"/>
		</g>
	</g>
</g>
<g>
	<path class="st22" d="M372.73,239.5c0-1.37,1.11-2.48,2.48-2.48c1.37,0,2.48,1.11,2.48,2.48c0,1.37-1.11,2.48-2.48,2.48
		C373.84,241.98,372.73,240.87,372.73,239.5"/>
</g>
<g>
	<g>
		<line class="st20" x1="388.8" y1="239.5" x2="391.83" y2="239.5"/>
		<g>
			<polygon class="st21" points="391.52,240.54 393.32,239.5 391.52,238.47 			"/>
		</g>
	</g>
</g>
<text transform="matrix(1 0 0 1 380.0946 241.0875)" class="st17 st19">C/A     -</text>
<path class="st30" d="M404.64,106.37"/>
<path class="st30" d="M400.37,162.65"/>
<rect x="180.72" y="70.21" class="st7" width="6.92" height="6.46"/>
<rect x="180.72" y="62.14" class="st7" width="6.92" height="6.46"/>
<rect x="180.72" y="54.07" class="st7" width="6.92" height="6.46"/>
<rect x="180.72" y="46" class="st7" width="6.92" height="6.46"/>
<polyline class="st1" points="187.64,76.82 187.64,70.37 180.71,70.37 180.71,76.82 "/>
<rect x="180.71" y="62.3" class="st1" width="6.93" height="6.46"/>
<polyline class="st1" points="187.64,60.68 187.64,54.22 180.71,54.22 180.71,60.68 "/>
<rect x="180.71" y="46.15" class="st1" width="6.93" height="6.46"/>
<polyline class="st1" points="187.64,44.64 187.64,38.18 180.71,38.18 180.71,44.64 "/>
<rect x="180.71" y="30.11" class="st1" width="6.93" height="6.46"/>
<polyline class="st1" points="187.64,28.47 187.64,22.02 180.71,22.02 180.71,28.47 "/>
<polyline class="st7" points="187.64,109.25 187.64,102.79 180.72,102.79 180.72,109.25 "/>
<path class="st30" d="M358.42,85.59"/>
<path class="st30" d="M343.96,143.36"/>
<path class="st30" d="M371.04,136.24"/>
<path class="st30" d="M375.31,79.97"/>
<polyline class="st7" points="187.64,109.05 187.64,102.6 180.72,102.6 180.72,109.05 "/>
<polyline class="st1" points="187.64,109.21 187.64,102.75 180.71,102.75 180.71,109.21 "/>
<text transform="matrix(1 0 0 1 468.2128 81.0084)" class="st17 st19">C</text>
<text transform="matrix(1 0 0 1 468.4511 72.9351)" class="st17 st19">A</text>
<text transform="matrix(1 0 0 1 468.9276 65.233)" class="st17 st19">-</text>
<rect x="346.79" y="282.27" class="st16" width="216.92" height="15.05"/>
<text transform="matrix(1 0 0 1 348.5204 288.0587)" class="st17 st31">where WCC is weighted concordance correlation coefficient</text>
<rect x="20.81" y="112.31" class="st16" width="108.75" height="10.93"/>
<text transform="matrix(1 0 0 1 20.8129 120.1187)" class="st17 st18">Original MSA &amp; Tree</text>
<line class="st32" x1="511.65" y1="94.54" x2="511.65" y2="222.71"/>
<line class="st32" x1="535.62" y1="94.54" x2="535.62" y2="223.01"/>
<line class="st33" x1="487.53" y1="107.25" x2="578.86" y2="107.25"/>
<line class="st32" x1="487.53" y1="114.95" x2="578.86" y2="114.95"/>
<line class="st32" x1="487.53" y1="122.65" x2="578.86" y2="122.65"/>
<line class="st32" x1="487.53" y1="130.34" x2="578.86" y2="130.34"/>
<line class="st32" x1="487.53" y1="138.04" x2="578.86" y2="138.04"/>
<line class="st32" x1="487.53" y1="145.74" x2="578.86" y2="145.74"/>
<line class="st32" x1="487.53" y1="153.44" x2="578.86" y2="153.44"/>
<line class="st32" x1="487.53" y1="161.13" x2="578.86" y2="161.13"/>
<line class="st32" x1="487.53" y1="168.83" x2="578.86" y2="168.83"/>
<line class="st32" x1="487.53" y1="176.53" x2="578.86" y2="176.53"/>
<line class="st32" x1="487.53" y1="184.22" x2="578.86" y2="184.22"/>
<line class="st32" x1="487.53" y1="191.92" x2="578.86" y2="191.92"/>
<line class="st32" x1="487.53" y1="199.62" x2="578.86" y2="199.62"/>
<line class="st32" x1="487.53" y1="207.32" x2="578.86" y2="207.32"/>
<line class="st32" x1="487.53" y1="215.01" x2="578.86" y2="215.01"/>
<line class="st32" x1="487.53" y1="222.71" x2="578.86" y2="222.71"/>
<path class="st32" d="M578.86,230.41"/>
<path class="st32" d="M487.53,230.41"/>
<text transform="matrix(1 0 0 1 549.6102 99.6099)"><tspan x="0" y="0" class="st34 st35 st36">Bra</tspan><tspan x="8.04" y="0" class="st34 st35 st36">n</tspan><tspan x="11.02" y="0" class="st34 st35 st36">c</tspan><tspan x="13.71" y="0" class="st34 st35 st36">h</tspan></text>
<text transform="matrix(1 0 0 1 547.993 105.4303)"><tspan x="0" y="0" class="st34 st35 st36">di</tspan><tspan x="4.34" y="0" class="st34 st35 st36">vers</tspan><tspan x="14.24" y="0" class="st34 st35 st36">i</tspan><tspan x="15.61" y="0" class="st34 st35 st36">ty</tspan></text>
<text transform="matrix(1 0 0 1 519.4891 102.5191)"><tspan x="0" y="0" class="st34 st35 st36">D</tspan><tspan x="3.49" y="0" class="st34 st35 st36">i</tspan><tspan x="4.85" y="0" class="st34 st35 st36">f</tspan></text>
<text transform="matrix(1 0 0 1 525.9569 103.6656)" class="st34 st35 st37">2</text>
<text transform="matrix(1 0 0 1 495.5233 102.5191)"><tspan x="0" y="0" class="st34 st35 st36">D</tspan><tspan x="3.49" y="0" class="st34 st35 st36">i</tspan><tspan x="4.85" y="0" class="st34 st35 st36">f</tspan></text>
<text transform="matrix(1 0 0 1 501.9911 103.6656)" class="st34 st35 st37">1</text>
<text transform="matrix(1 0 0 1 551.9091 112.6627)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">37</tspan><tspan x="9.4" y="0" class="st34 st38 st36">7</tspan></text>
<text transform="matrix(1 0 0 1 518.9335 112.6627)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">6</tspan><tspan x="6.72" y="0" class="st34 st38 st36">4</tspan></text>
<text transform="matrix(1 0 0 1 494.9677 112.6627)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">6</tspan><tspan x="6.72" y="0" class="st34 st38 st36">4</tspan></text>
<text transform="matrix(1 0 0 1 551.9091 120.4254)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">59</tspan><tspan x="9.4" y="0" class="st34 st38 st36">4</tspan></text>
<text transform="matrix(1 0 0 1 518.9335 120.4254)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">5</tspan><tspan x="6.72" y="0" class="st34 st38 st36">7</tspan></text>
<text transform="matrix(1 0 0 1 494.9677 120.4254)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">5</tspan><tspan x="6.72" y="0" class="st34 st38 st36">7</tspan></text>
<text transform="matrix(1 0 0 1 551.9091 128.0982)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">14</tspan><tspan x="9.4" y="0" class="st34 st38 st36">7</tspan></text>
<text transform="matrix(1 0 0 1 518.9335 128.0982)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">5</tspan><tspan x="6.72" y="0" class="st34 st38 st36">7</tspan></text>
<text transform="matrix(1 0 0 1 494.9677 128.0982)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">5</tspan><tspan x="6.72" y="0" class="st34 st38 st36">7</tspan></text>
<text transform="matrix(1 0 0 1 551.9091 135.7711)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">15</tspan><tspan x="9.4" y="0" class="st34 st38 st36">5</tspan></text>
<text transform="matrix(1 0 0 1 518.9335 135.7711)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">2</tspan><tspan x="6.72" y="0" class="st34 st38 st36">8</tspan></text>
<text transform="matrix(1 0 0 1 494.9677 135.7711)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">2</tspan><tspan x="6.72" y="0" class="st34 st38 st36">8</tspan></text>
<text transform="matrix(1 0 0 1 551.9091 143.4449)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">04</tspan><tspan x="9.4" y="0" class="st34 st38 st36">0</tspan></text>
<text transform="matrix(1 0 0 1 518.9335 143.4449)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">0</tspan><tspan x="6.72" y="0" class="st34 st38 st36">7</tspan></text>
<text transform="matrix(1 0 0 1 494.9677 143.4449)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">0</tspan><tspan x="6.72" y="0" class="st34 st38 st36">7</tspan></text>
<text transform="matrix(1 0 0 1 551.9091 151.2066)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">10</tspan><tspan x="9.4" y="0" class="st34 st38 st36">2</tspan></text>
<text transform="matrix(1 0 0 1 518.9335 151.2066)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">0</tspan><tspan x="6.72" y="0" class="st34 st38 st36">1</tspan></text>
<text transform="matrix(1 0 0 1 494.9677 151.2066)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">0</tspan><tspan x="6.72" y="0" class="st34 st38 st36">1</tspan></text>
<text transform="matrix(1 0 0 1 551.9091 158.8795)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">05</tspan><tspan x="9.4" y="0" class="st34 st38 st36">6</tspan></text>
<text transform="matrix(1 0 0 1 518.9335 158.8795)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">0</tspan><tspan x="6.72" y="0" class="st34 st38 st36">1</tspan></text>
<text transform="matrix(1 0 0 1 494.9677 158.8795)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">0</tspan><tspan x="6.72" y="0" class="st34 st38 st36">1</tspan></text>
<text transform="matrix(1 0 0 1 551.9091 166.5533)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">12</tspan><tspan x="9.4" y="0" class="st34 st38 st36">0</tspan></text>
<text transform="matrix(1 0 0 1 518.9335 166.5533)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">0</tspan><tspan x="6.72" y="0" class="st34 st38 st36">1</tspan></text>
<text transform="matrix(1 0 0 1 494.9677 166.5533)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">0</tspan><tspan x="6.72" y="0" class="st34 st38 st36">1</tspan></text>
<text transform="matrix(1 0 0 1 551.9091 174.2262)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">07</tspan><tspan x="9.4" y="0" class="st34 st38 st36">8</tspan></text>
<text transform="matrix(1 0 0 1 518.9335 174.2262)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">0</tspan><tspan x="6.72" y="0" class="st34 st38 st36">1</tspan></text>
<text transform="matrix(1 0 0 1 494.9677 174.2262)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">0</tspan><tspan x="6.72" y="0" class="st34 st38 st36">1</tspan></text>
<text transform="matrix(1 0 0 1 551.9091 181.9888)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">05</tspan><tspan x="9.4" y="0" class="st34 st38 st36">5</tspan></text>
<text transform="matrix(1 0 0 1 518.9335 181.9888)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">0</tspan><tspan x="6.72" y="0" class="st34 st38 st36">1</tspan></text>
<text transform="matrix(1 0 0 1 494.9677 181.9888)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">0</tspan><tspan x="6.72" y="0" class="st34 st38 st36">1</tspan></text>
<text transform="matrix(1 0 0 1 551.9091 189.6607)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">06</tspan><tspan x="9.4" y="0" class="st34 st38 st36">2</tspan></text>
<text transform="matrix(1 0 0 1 518.9335 189.6607)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">0</tspan><tspan x="6.72" y="0" class="st34 st38 st36">0</tspan></text>
<text transform="matrix(1 0 0 1 494.9677 189.6607)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">0</tspan><tspan x="6.72" y="0" class="st34 st38 st36">1</tspan></text>
<text transform="matrix(1 0 0 1 551.9091 197.3345)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">01</tspan><tspan x="9.4" y="0" class="st34 st38 st36">6</tspan></text>
<text transform="matrix(1 0 0 1 518.9335 197.3345)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">0</tspan><tspan x="6.72" y="0" class="st34 st38 st36">0</tspan></text>
<text transform="matrix(1 0 0 1 494.9677 197.3345)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">0</tspan><tspan x="6.72" y="0" class="st34 st38 st36">1</tspan></text>
<text transform="matrix(1 0 0 1 551.9091 205.0963)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">00</tspan><tspan x="9.4" y="0" class="st34 st38 st36">7</tspan></text>
<text transform="matrix(1 0 0 1 518.9335 205.0963)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">0</tspan><tspan x="6.72" y="0" class="st34 st38 st36">0</tspan></text>
<text transform="matrix(1 0 0 1 494.9677 205.0963)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">0</tspan><tspan x="6.72" y="0" class="st34 st38 st36">2</tspan></text>
<text transform="matrix(1 0 0 1 551.9091 212.7691)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">02</tspan><tspan x="9.4" y="0" class="st34 st38 st36">6</tspan></text>
<text transform="matrix(1 0 0 1 518.9335 212.7691)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">0</tspan><tspan x="6.72" y="0" class="st34 st38 st36">0</tspan></text>
<text transform="matrix(1 0 0 1 494.9677 212.7691)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">0</tspan><tspan x="6.72" y="0" class="st34 st38 st36">0</tspan></text>
<text transform="matrix(1 0 0 1 551.9091 220.4439)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">00</tspan><tspan x="9.4" y="0" class="st34 st38 st36">8</tspan></text>
<text transform="matrix(1 0 0 1 518.9335 220.4439)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">0</tspan><tspan x="6.72" y="0" class="st34 st38 st36">0</tspan></text>
<text transform="matrix(1 0 0 1 494.9677 220.4439)"><tspan x="0" y="0" class="st34 st38 st36">0</tspan><tspan x="2.68" y="0" class="st34 st38 st36">.</tspan><tspan x="4.04" y="0" class="st34 st38 st36">0</tspan><tspan x="6.72" y="0" class="st34 st38 st36">0</tspan></text>
<defs>
	<filter id="Adobe_OpacityMaskFilter" filterUnits="userSpaceOnUse" x="480.74" y="205.06" width="98.34" height="35.29">
		<feColorMatrix  type="matrix" values="1 0 0 0 0  0 1 0 0 0  0 0 1 0 0  0 0 0 1 0"/>
	</filter>
</defs>
<mask maskUnits="userSpaceOnUse" x="480.74" y="205.06" width="98.34" height="35.29" id="SVGID_00000153696681527952498250000009782666863973765310_">
	<g class="st39">
		
			<linearGradient id="SVGID_00000020371036692739102150000002692104580830245039_" gradientUnits="userSpaceOnUse" x1="450.2113" y1="276.8755" x2="381.1187" y2="276.8755" gradientTransform="matrix(-3.464102e-07 1 -1 -3.464102e-07 806.8574 -176.0721)">
			<stop  offset="0" style="stop-color:#010101"/>
			<stop  offset="0.025" style="stop-color:#010101"/>
			<stop  offset="0.06" style="stop-color:#535454"/>
			<stop  offset="0.095" style="stop-color:#A7A6A6"/>
			<stop  offset="0.13" style="stop-color:#FAFBFC"/>
			<stop  offset="0.2533" style="stop-color:#FAFBFC"/>
			<stop  offset="0.3767" style="stop-color:#F9F9FA"/>
			<stop  offset="0.5" style="stop-color:#FAFBFC"/>
			<stop  offset="0.6233" style="stop-color:#F9F9FA"/>
			<stop  offset="0.7467" style="stop-color:#FAFBFC"/>
			<stop  offset="0.87" style="stop-color:#FAFBFC"/>
			<stop  offset="0.905" style="stop-color:#A7A6A6"/>
			<stop  offset="0.94" style="stop-color:#535454"/>
			<stop  offset="0.975" style="stop-color:#010101"/>
			<stop  offset="1" style="stop-color:#010101"/>
		</linearGradient>
		
			<rect x="480.8" y="205.05" style="fill-rule:evenodd;clip-rule:evenodd;fill:url(#SVGID_00000020371036692739102150000002692104580830245039_);" width="98.36" height="34.55"/>
	</g>
</mask>
<linearGradient id="SVGID_00000142172341558156578570000015587286139977955724_" gradientUnits="userSpaceOnUse" x1="451.723" y1="276.9515" x2="381.1353" y2="276.9515" gradientTransform="matrix(-3.464102e-07 1 -1 -3.464102e-07 806.8574 -176.0721)">
	<stop  offset="0" style="stop-color:#FFFFFF"/>
	<stop  offset="0.025" style="stop-color:#FFFFFF"/>
	<stop  offset="0.06" style="stop-color:#FFFFFF"/>
	<stop  offset="0.095" style="stop-color:#FFFFFF"/>
	<stop  offset="0.13" style="stop-color:#FFFFFF"/>
	<stop  offset="0.2533" style="stop-color:#FFFFFF"/>
	<stop  offset="0.3767" style="stop-color:#FFFFFF"/>
	<stop  offset="0.5" style="stop-color:#FFFFFF"/>
	<stop  offset="0.6233" style="stop-color:#FFFFFF"/>
	<stop  offset="0.7467" style="stop-color:#FFFFFF"/>
	<stop  offset="0.87" style="stop-color:#FFFFFF"/>
	<stop  offset="0.905" style="stop-color:#FFFFFF"/>
	<stop  offset="0.94" style="stop-color:#FFFFFF"/>
	<stop  offset="0.975" style="stop-color:#FFFFFF"/>
	<stop  offset="1" style="stop-color:#FFFFFF"/>
</linearGradient>
<polygon style="mask:url(#SVGID_00000153696681527952498250000009782666863973765310_);fill-rule:evenodd;clip-rule:evenodd;fill:url(#SVGID_00000142172341558156578570000015587286139977955724_);" points="
	480.74,205.06 480.74,239.65 579.07,240.36 579.07,205.77 "/>
<rect x="474.36" y="84.96" class="st16" width="116.34" height="15.05"/>
<text transform="matrix(1 0 0 1 487.3661 90.7462)" class="st17 st31">Total Change per Branch</text>
<rect x="102.85" y="142.55" class="st15" width="6.93" height="167.89"/>
<polyline class="st11" points="193.6,189.94 200.52,189.94 200.52,183.49 193.6,183.49 "/>
<polyline class="st11" points="193.6,181.87 200.52,181.87 200.52,175.41 193.6,175.41 "/>
<polyline class="st11" points="193.6,173.8 200.52,173.8 200.52,167.34 193.6,167.34 "/>
<polyline class="st11" points="193.6,165.73 200.52,165.73 200.52,159.27 193.6,159.27 "/>
<polyline class="st11" points="193.6,157.66 200.52,157.66 200.52,151.2 193.6,151.2 "/>
<polyline class="st11" points="193.6,149.58 200.52,149.58 200.52,143.13 193.6,143.13 "/>
<polyline class="st11" points="193.6,141.51 200.52,141.51 200.52,135.06 193.6,135.06 "/>
<polyline class="st11" points="193.6,133.44 200.52,133.44 200.52,126.98 193.6,126.98 "/>
<polyline class="st11" points="193.6,125.37 200.52,125.37 200.52,118.91 193.6,118.91 "/>
<polyline class="st11" points="193.6,117.3 200.52,117.3 200.52,110.84 193.6,110.84 "/>
<polyline class="st7" points="193.6,109.23 200.52,109.23 200.52,102.77 193.6,102.77 "/>
<polyline class="st12" points="193.6,101.15 200.52,101.15 200.52,94.7 193.6,94.7 "/>
<polyline class="st12" points="193.6,93.08 200.52,93.08 200.52,86.63 193.6,86.63 "/>
<polyline class="st12" points="193.6,85.01 200.52,85.01 200.52,78.55 193.6,78.55 "/>
<polyline class="st7" points="193.6,76.94 200.52,76.94 200.52,70.48 193.6,70.48 "/>
<polyline class="st7" points="193.6,68.87 200.52,68.87 200.52,62.41 193.6,62.41 "/>
<polyline class="st7" points="193.6,60.8 200.52,60.8 200.52,54.34 193.6,54.34 "/>
<polyline class="st7" points="193.6,52.72 200.52,52.72 200.52,46.27 193.6,46.27 "/>
<polyline class="st7" points="193.6,76.75 200.52,76.75 200.52,70.29 193.6,70.29 "/>
<polyline class="st7" points="193.6,68.68 200.52,68.68 200.52,62.22 193.6,62.22 "/>
<polyline class="st7" points="193.6,60.6 200.52,60.6 200.52,54.15 193.6,54.15 "/>
<polyline class="st7" points="193.6,52.53 200.52,52.53 200.52,46.08 193.6,46.08 "/>
<polyline class="st1" points="200.52,76.9 200.52,70.44 193.59,70.44 "/>
<polyline class="st1" points="193.59,68.83 200.52,68.83 200.52,62.37 193.59,62.37 "/>
<polyline class="st1" points="193.6,52.69 200.52,52.69 200.52,46.23 193.6,46.23 "/>
<polyline class="st1" points="193.6,36.64 200.52,36.64 200.52,30.18 193.6,30.18 "/>
<polyline class="st7" points="200.52,109.32 200.52,102.86 193.6,102.86 "/>
<polyline class="st7" points="200.52,109.13 200.52,102.67 193.59,102.67 "/>
<polyline class="st1" points="200.52,109.28 200.52,102.83 193.59,102.83 "/>
<polyline class="st1" points="193.59,44.64 200.52,44.64 200.52,38.18 193.59,38.18 "/>
<polyline class="st1" points="193.59,60.8 200.52,60.8 200.52,54.34 193.59,54.34 "/>
<polyline class="st1" points="193.59,28.47 200.52,28.47 200.52,22.02 193.59,22.02 "/>
<polyline class="st1" points="193.59,76.82 200.52,76.82 200.52,70.37 193.59,70.37 "/>
<polyline class="st1" points="193.59,109.32 200.52,109.32 200.52,102.86 193.59,102.86 "/>
<rect x="180.71" y="21.77" class="st15" width="6.93" height="167.89"/>
<rect x="193.59" y="21.67" class="st15" width="6.93" height="167.89"/>
<path class="st42" d="M309.81,196.61H181.7c-5.48,0-9.92-4.44-9.92-9.92V26.47c0-5.48,4.44-9.92,9.92-9.92h128.11
	c5.48,0,9.92,4.44,9.92,9.92v160.22C319.73,192.17,315.29,196.61,309.81,196.61z"/>
<rect x="180.71" y="241.22" class="st15" width="6.93" height="167.89"/>
<rect x="193.59" y="241.22" class="st15" width="6.93" height="167.89"/>
<g>
	<g>
		<line class="st25" x1="151.55" y1="260.1" x2="166.03" y2="260.16"/>
		<g>
			<polygon class="st26" points="165.49,261.98 168.66,260.17 165.5,258.32 			"/>
		</g>
	</g>
</g>
<path class="st42" d="M309.81,415.02H181.7c-5.48,0-9.92-4.44-9.92-9.92V244.88c0-5.48,4.44-9.92,9.92-9.92h128.11
	c5.48,0,9.92,4.44,9.92,9.92V405.1C319.73,410.58,315.29,415.02,309.81,415.02z"/>
<rect x="433.41" y="222.28" class="st11" width="6.92" height="6.46"/>
<rect x="433.41" y="214.21" class="st12" width="6.92" height="6.46"/>
<rect x="433.41" y="206.14" class="st11" width="6.92" height="6.46"/>
<rect x="433.41" y="198.07" class="st11" width="6.92" height="6.46"/>
<rect x="433.41" y="190" class="st11" width="6.92" height="6.46"/>
<rect x="433.41" y="181.93" class="st11" width="6.92" height="6.46"/>
<rect x="433.41" y="173.85" class="st11" width="6.92" height="6.46"/>
<rect x="433.41" y="165.78" class="st11" width="6.92" height="6.46"/>
<rect x="433.41" y="157.71" class="st11" width="6.92" height="6.46"/>
<rect x="433.41" y="149.64" class="st11" width="6.92" height="6.46"/>
<rect x="433.41" y="141.57" class="st7" width="6.92" height="6.46"/>
<rect x="433.41" y="133.5" class="st12" width="6.92" height="6.46"/>
<rect x="433.41" y="125.42" class="st12" width="6.92" height="6.46"/>
<rect x="433.41" y="117.35" class="st12" width="6.92" height="6.46"/>
<rect x="433.41" y="109.28" class="st7" width="6.92" height="6.46"/>
<rect x="433.41" y="101.21" class="st7" width="6.92" height="6.46"/>
<rect x="433.41" y="93.14" class="st7" width="6.92" height="6.46"/>
<rect x="433.41" y="85.07" class="st7" width="6.92" height="6.46"/>
<polyline class="st1" points="440.33,115.89 440.33,109.43 433.4,109.43 433.4,115.89 "/>
<rect x="433.4" y="101.36" class="st1" width="6.93" height="6.46"/>
<path class="st43" d="M438.06,162.65"/>
<path class="st30" d="M445.89,106.37"/>
<polyline class="st1" points="440.33,99.75 440.33,93.29 433.4,93.29 433.4,99.75 "/>
<rect x="433.4" y="85.22" class="st1" width="6.93" height="6.46"/>
<polyline class="st1" points="440.33,83.7 440.33,77.25 433.4,77.25 433.4,83.7 "/>
<rect x="433.4" y="69.17" class="st1" width="6.93" height="6.46"/>
<polyline class="st1" points="440.33,67.54 440.33,61.08 433.4,61.08 433.4,67.54 "/>
<rect x="433.4" y="141.62" class="st1" width="6.93" height="6.46"/>
<g>
	<rect x="447.1" y="222.28" class="st11" width="6.92" height="6.46"/>
	<rect x="447.1" y="214.21" class="st11" width="6.92" height="6.46"/>
	<rect x="447.1" y="206.14" class="st11" width="6.92" height="6.46"/>
	<rect x="447.1" y="198.07" class="st11" width="6.92" height="6.46"/>
	<rect x="447.1" y="190" class="st11" width="6.92" height="6.46"/>
	<rect x="447.1" y="181.93" class="st11" width="6.92" height="6.46"/>
	<rect x="447.1" y="173.85" class="st11" width="6.92" height="6.46"/>
	<rect x="447.1" y="165.78" class="st11" width="6.92" height="6.46"/>
	<rect x="447.1" y="157.71" class="st11" width="6.92" height="6.46"/>
	<rect x="447.1" y="149.64" class="st11" width="6.92" height="6.46"/>
	<rect x="447.1" y="141.57" class="st7" width="6.92" height="6.46"/>
	<rect x="447.1" y="133.5" class="st12" width="6.92" height="6.46"/>
	<rect x="447.1" y="125.42" class="st12" width="6.92" height="6.46"/>
	<rect x="447.1" y="117.35" class="st12" width="6.92" height="6.46"/>
	<rect x="447.1" y="109.28" class="st7" width="6.92" height="6.46"/>
	<rect x="447.1" y="101.21" class="st7" width="6.92" height="6.46"/>
	<rect x="447.1" y="93.14" class="st7" width="6.92" height="6.46"/>
	<rect x="447.1" y="85.07" class="st7" width="6.92" height="6.46"/>
</g>
<polyline class="st1" points="454.02,115.89 454.02,109.43 447.09,109.43 447.09,115.89 "/>
<rect x="447.09" y="101.36" class="st1" width="6.93" height="6.46"/>
<polyline class="st1" points="454.02,99.75 454.02,93.29 447.1,93.29 447.1,99.75 "/>
<rect x="447.1" y="85.22" class="st1" width="6.93" height="6.46"/>
<polyline class="st1" points="454.02,83.7 454.02,77.25 447.1,77.25 447.1,83.7 "/>
<rect x="447.1" y="69.17" class="st1" width="6.93" height="6.46"/>
<polyline class="st1" points="454.02,67.54 454.02,61.08 447.09,61.08 447.09,67.54 "/>
<rect x="447.1" y="141.62" class="st1" width="6.93" height="6.46"/>
<g>
	<g>
		<line class="st25" x1="325.12" y1="122.56" x2="342.21" y2="122.63"/>
		<g>
			<polygon class="st26" points="341.66,124.45 344.84,122.64 341.68,120.79 			"/>
		</g>
	</g>
</g>
<g>
	<g>
		<line class="st25" x1="324.42" y1="243.24" x2="342.68" y2="235.59"/>
		<g>
			<polygon class="st26" points="342.9,237.48 345.11,234.57 341.48,234.1 			"/>
		</g>
	</g>
</g>
</svg>
svg…]()
