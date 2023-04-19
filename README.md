# GIB-LSTM
# Semantic representation and attention alignment for Graph Information Bottleneck in video summarization  

## Introduction

We adopted the Graph Information Bottle (GIB) to develop a Contextual Feature Transformation (CFT)  mechanism that refines the temporal two-stream feature, yielding a semantic representation with attention alignment. Furthermore, a novel Salient-Area-Size-based spatial attention model is presented to extract frame-wise visual features based on the observation that humans tend to focus on sizable and moving objects. Finally, semantic representation is embedded within attention alignment under the end-to-end LSTM framework to differentiate indistinguishable images.

![](https://github.com/wangrui91/GIB-LSTM/blob/main/images/GIB-LSTM.png)

##  Experiments
#### 主观实验结果
Comparison with other unsupervised video summarization methods under the canonical setting (F-score %)

<table class=MsoTableGrid border=1 cellspacing=0 cellpadding=0
 style='border-collapse:collapse;border:none;mso-border-alt:solid windowtext .5pt;
 mso-yfti-tbllook:1184;mso-padding-alt:0cm 5.4pt 0cm 5.4pt'>
 <tr style='mso-yfti-irow:0;mso-yfti-firstrow:yes'>
  <td width=165 valign=top style='width:123.7pt;border-top:solid windowtext 1.0pt;
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;
  mso-border-top-alt:solid windowtext .5pt;mso-border-bottom-alt:solid windowtext .5pt;
  padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>Method<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border-top:solid windowtext 1.0pt;
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;
  mso-border-top-alt:solid windowtext .5pt;mso-border-bottom-alt:solid windowtext .5pt;
  padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-family:"Times New Roman",serif'>SumMe</span></span><span
  lang=EN-US style='font-family:"Times New Roman",serif'><o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border-top:solid windowtext 1.0pt;
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;
  mso-border-top-alt:solid windowtext .5pt;mso-border-bottom-alt:solid windowtext .5pt;
  padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-family:"Times New Roman",serif'>TVSum</span></span><span
  lang=EN-US style='font-family:"Times New Roman",serif'><o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:1'>
  <td width=165 valign=top style='width:123.7pt;border:none;mso-border-top-alt:
  solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>K-<span class=SpellE>methoids</span>
  [1]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;mso-border-top-alt:
  solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>33.4<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;mso-border-top-alt:
  solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>28.8<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:2'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-family:"Times New Roman",serif'>Vsumm</span></span><span
  lang=EN-US style='font-family:"Times New Roman",serif'> [2]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>33.7<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>-<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:3'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>Web image [3]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>-<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>36.0<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:4'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>Dictionary selection [4]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>37.8<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>42.0<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:5'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>Online space coding [5]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>-<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>46.0<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:6'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>Co-archetypal [6]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>-<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>50.0<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:7'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-family:"Times New Roman",serif'>GANdpp</span></span><span
  lang=EN-US style='font-family:"Times New Roman",serif'> [7]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>39.1<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>51.7<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:8'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>DR-DSN [8]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>41.4<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>57.6<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:9'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>Cycle-SUM [9]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>41.9<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>57.6<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:10'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-family:"Times New Roman",serif'>CSNet</span></span><span
  lang=EN-US style='font-family:"Times New Roman",serif'> [10]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>51.3<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>58.8<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:11'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>GAT-LSTM [11]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>51.5<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>59.1<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:12'>
  <td width=165 valign=top style='width:123.7pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>DSAVS [12]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>47.0<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>59.4<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:13;mso-yfti-lastrow:yes'>
  <td width=165 valign=top style='width:123.7pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-top-alt:solid windowtext .5pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>Proposed<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-top-alt:solid windowtext .5pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><b><span
  lang=EN-US style='font-family:"Times New Roman",serif'>55.0<o:p></o:p></span></b></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-top-alt:solid windowtext .5pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><b><span
  lang=EN-US style='font-family:"Times New Roman",serif'>62.5<o:p></o:p></span></b></p>
  </td>
 </tr>
</table>

Comparison with other supervised video summarization methods under the canonical setting (F-score %)

<table class=MsoTableGrid border=1 cellspacing=0 cellpadding=0
 style='border-collapse:collapse;border:none;mso-border-alt:solid windowtext .5pt;
 mso-yfti-tbllook:1184;mso-padding-alt:0cm 5.4pt 0cm 5.4pt'>
 <tr style='mso-yfti-irow:0;mso-yfti-firstrow:yes'>
  <td width=165 valign=top style='width:123.7pt;border-top:solid windowtext 1.0pt;
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;
  mso-border-top-alt:solid windowtext .5pt;mso-border-bottom-alt:solid windowtext .5pt;
  padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>Method</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif'><o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border-top:solid windowtext 1.0pt;
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;
  mso-border-top-alt:solid windowtext .5pt;mso-border-bottom-alt:solid windowtext .5pt;
  padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-family:"Times New Roman",serif'>SumMe</span></span><span
  lang=EN-US style='font-family:"Times New Roman",serif'><o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border-top:solid windowtext 1.0pt;
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;
  mso-border-top-alt:solid windowtext .5pt;mso-border-bottom-alt:solid windowtext .5pt;
  padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-family:"Times New Roman",serif'>TVSum</span></span><span
  lang=EN-US style='font-family:"Times New Roman",serif'><o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:1'>
  <td width=165 valign=top style='width:123.7pt;border:none;mso-border-top-alt:
  solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>Interestingness [13]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;mso-border-top-alt:
  solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>39.4<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;mso-border-top-alt:
  solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>-<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:2;height:16.1pt'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt;
  height:16.1pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-family:"Times New Roman",serif'>Submodularity</span></span><span
  lang=EN-US style='font-family:"Times New Roman",serif'> [14]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt;
  height:16.1pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>39.7<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt;
  height:16.1pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>-<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:3'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>Summary transfer [15]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>40.9<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>-<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:4'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>Bi-LSTM [16]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>37.6<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>54.2<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:5'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-family:"Times New Roman",serif'>Dpp</span></span><span
  lang=EN-US style='font-family:"Times New Roman",serif'>-LSTM [16]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>38.6<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>54.7<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:6'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-family:"Times New Roman",serif'>GANsup</span></span><span
  lang=EN-US style='font-family:"Times New Roman",serif'> [7]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>41.7<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>56.3<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:7'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>DR-<span class=SpellE>DSNsup</span>
  [8]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>42.1<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>58.1<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:8'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>Cycle-<span
  class=SpellE>SUMsup</span> [9]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>44.8<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>58.1<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:9'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-family:"Times New Roman",serif'>CSNetsup</span></span><span
  lang=EN-US style='font-family:"Times New Roman",serif'> [10]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>48.6<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>58.5<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:10'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-family:"Times New Roman",serif'>CRSum</span></span><span
  lang=EN-US style='font-family:"Times New Roman",serif'> [17]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>47.3<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>58.0<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:11'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>GAT-<span
  class=SpellE>LSTMsup</span> [11]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>51.7<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>59.6<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:12'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>HMT [18]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>44.1<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>60.1<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:13'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-family:"Times New Roman",serif'>DSAVSsup</span></span><span
  lang=EN-US style='font-family:"Times New Roman",serif'> [12]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>48.9<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>59.8<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:14'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-family:"Times New Roman",serif'>DSNet</span></span><span
  lang=EN-US style='font-family:"Times New Roman",serif'> [19]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>50.2<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>62.1<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:15'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>LMHA [20]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>51.1<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>61.0<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:16'>
  <td width=165 valign=top style='width:123.7pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>LMHA-two [20]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>51.4<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>61.5<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:17'>
  <td width=165 valign=top style='width:123.7pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>RR-STG [21]<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>53.4<o:p></o:p></span></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><b><span
  lang=EN-US style='font-family:"Times New Roman",serif'>63.0</span></b><span
  lang=EN-US style='font-family:"Times New Roman",serif'><o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:18;mso-yfti-lastrow:yes'>
  <td width=165 valign=top style='width:123.7pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-top-alt:solid windowtext .5pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>Proposed-sup<o:p></o:p></span></p>
  </td>
  <td width=97 valign=top style='width:72.8pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-top-alt:solid windowtext .5pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><b><span
  lang=EN-US style='font-family:"Times New Roman",serif'>56.0<o:p></o:p></span></b></p>
  </td>
  <td width=88 valign=top style='width:66.0pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-top-alt:solid windowtext .5pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-family:"Times New Roman",serif'>62.7<b><o:p></o:p></b></span></p>
  </td>
 </tr>
</table>



#### 客观实验结果

![](https://github.com/wangrui91/GIB-LSTM/blob/main/images/Visualization.png)
