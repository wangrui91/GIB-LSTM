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
  lang=EN-US style='font-family:"Times New Roman",serif'>Dictionary selection [1]<o:p></o:p></span></p>
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
  lang=EN-US style='font-family:"Times New Roman",serif'>Online space coding [4]<o:p></o:p></span></p>
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
  lang=EN-US style='font-family:"Times New Roman",serif'>Co-archetypal [5]<o:p></o:p></span></p>
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
  lang=EN-US style='font-family:"Times New Roman",serif'> [6]<o:p></o:p></span></p>
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
  lang=EN-US style='font-family:"Times New Roman",serif'>DR-DSN [7]<o:p></o:p></span></p>
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
  lang=EN-US style='font-family:"Times New Roman",serif'>Cycle-SUM [8]<o:p></o:p></span></p>
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
  lang=EN-US style='font-family:"Times New Roman",serif'> [9]<o:p></o:p></span></p>
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
  lang=EN-US style='font-family:"Times New Roman",serif'>GAT-LSTM [10]<o:p></o:p></span></p>
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
  lang=EN-US style='font-family:"Times New Roman",serif'>DSAVS [11]<o:p></o:p></span></p>
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
  lang=EN-US style='font-family:"Times New Roman",serif'>Interestingness [12]<o:p></o:p></span></p>
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
  lang=EN-US style='font-family:"Times New Roman",serif'> [13]<o:p></o:p></span></p>
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
  lang=EN-US style='font-family:"Times New Roman",serif'>Summary transfer [14]<o:p></o:p></span></p>
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
  lang=EN-US style='font-family:"Times New Roman",serif'>Bi-LSTM [15]<o:p></o:p></span></p>
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
  lang=EN-US style='font-family:"Times New Roman",serif'>-LSTM [15]<o:p></o:p></span></p>
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
  lang=EN-US style='font-family:"Times New Roman",serif'> [6]<o:p></o:p></span></p>
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
  [7]<o:p></o:p></span></p>
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
  class=SpellE>SUMsup</span> [8]<o:p></o:p></span></p>
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
  lang=EN-US style='font-family:"Times New Roman",serif'> [9]<o:p></o:p></span></p>
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
  lang=EN-US style='font-family:"Times New Roman",serif'> [16]<o:p></o:p></span></p>
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
  class=SpellE>LSTMsup</span> [10]<o:p></o:p></span></p>
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
  lang=EN-US style='font-family:"Times New Roman",serif'>HMT [17]<o:p></o:p></span></p>
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
  lang=EN-US style='font-family:"Times New Roman",serif'> [11]<o:p></o:p></span></p>
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
  lang=EN-US style='font-family:"Times New Roman",serif'> [18]<o:p></o:p></span></p>
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
  lang=EN-US style='font-family:"Times New Roman",serif'>LMHA [19]<o:p></o:p></span></p>
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
  lang=EN-US style='font-family:"Times New Roman",serif'>LMHA-two [19]<o:p></o:p></span></p>
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
  lang=EN-US style='font-family:"Times New Roman",serif'>RR-STG [20]<o:p></o:p></span></p>
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

## references
[1] E. Elhamifar, G. Sapiro, and R. Vidal, “See all by looking at a few: Sparse modeling for fifinding representative objects,” in CVPR, 2012, pp. 1600–1607.<br>
[2] De Avila, S. E. F., Lopes, A. P. B., da Luz Jr, A., & de Albuquerque Araújo, A. (2011). VSUMM: A mechanism designed to produce static video summaries and a novel evaluation method. Pattern recognition letters, 32(1), 56-68.<br>
[3] Khosla, A., Hamid, R., Lin, C. J., & Sundaresan, N. (2013). Large-scale video summarization using web-image priors. In Proceedings of the IEEE conference on computer vision and pattern recognition (pp. 2698-2705).<br>
[4] Zhao, B., & Xing, E. P. (2014). Quasi real-time summarization for consumer videos. In Proceedings of the IEEE conference on computer vision and pattern recognition (pp. 2513-2520).<br>
[5] Song, Y., Vallmitjana, J., Stent, A., & Jaimes, A. (2015). Tvsum: Summarizing web videos using titles. In Proceedings of the IEEE conference on computer vision and pattern recognition (pp. 5179-5187).<br>
[6] Mahasseni, B., Lam, M., & Todorovic, S. (2017). Unsupervised video summarization with adversarial lstm networks. In Proceedings of the IEEE conference on Computer Vision and Pattern Recognition (pp. 202-211).<br>
[7] Zhou, K., Qiao, Y., & Xiang, T. (2018, April). Deep reinforcement learning for unsupervised video summarization with diversity-representativeness reward. In Proceedings of the AAAI Conference on Artificial Intelligence (Vol. 32, No. 1).<br>
[8] Yuan, L., Tay, F. E. H., Li, P., & Feng, J. (2019). Unsupervised video summarization with cycle-consistent adversarial LSTM networks. IEEE Transactions on Multimedia, 22(10), 2711-2722.<br>
[9] Jung, Y., Cho, D., Kim, D., Woo, S., & Kweon, I. S. (2019, July). Discriminative feature learning for unsupervised video summarization. In Proceedings of the AAAI Conference on artificial intelligence (Vol. 33, No. 01, pp. 8537-8544).<br>
[10] Zhong, R., Wang, R., Zou, Y., Hong, Z., & Hu, M. (2021). Graph attention networks adjusted bi-LSTM for video summarization. IEEE Signal Processing Letters, 28, 663-667.<br>
[11] Zhong, S. H., Lin, J., Lu, J., Fares, A., & Ren, T. (2022). Deep semantic and attentive network for unsupervised video summarization. ACM Transactions on Multimedia Computing, Communications, and Applications (TOMM), 18(2), 1-21.<br>
[12] Gygli, M., Grabner, H., Riemenschneider, H., & Van Gool, L. (2014). Creating summaries from user videos. In Computer Vision–ECCV 2014: 13th European Conference, Zurich, Switzerland, September 6-12, 2014, Proceedings, Part VII 13 (pp. 505-520). Springer International Publishing.<br>
[13] Gygli, M., Grabner, H., & Van Gool, L. (2015). Video summarization by learning submodular mixtures of objectives. In Proceedings of the IEEE conference on computer vision and pattern recognition (pp. 3090-3098).<br>
[14] Zhang, K., Chao, W. L., Sha, F., & Grauman, K. (2016). Summary transfer: Exemplar-based subset selection for video summarization. In Proceedings of the IEEE conference on computer vision and pattern recognition (pp. 1059-1067).<br>
[15] Zhang, K., Chao, W. L., Sha, F., & Grauman, K. (2016). Video summarization with long short-term memory. In Computer Vision–ECCV 2016: 14th European Conference, Amsterdam, The Netherlands, October 11–14, 2016, Proceedings, Part VII 14 (pp. 766-782). Springer International Publishing.<br>
[16] Yuan, Y., Li, H., & Wang, Q. (2019). Spatiotemporal modeling for video summarization using convolutional recurrent neural network. IEEE Access, 7, 64676-64685.<br>
[17] Sanabria, M., Precioso, F., & Menguy, T. (2021, January). Hierarchical multimodal attention for deep video summarization. In 2020 25th International Conference on Pattern Recognition (ICPR) (pp. 7977-7984). IEEE.<br>
[18] Zhu, W., Lu, J., Li, J., & Zhou, J. (2020). Dsnet: A flexible detect-to-summarize network for video summarization. IEEE Transactions on Image Processing, 30, 948-962.<br>
[19] Zhu, W., Lu, J., Han, Y., & Zhou, J. (2022). Learning multiscale hierarchical attention for video summarization. Pattern Recognition, 122, 108312.<br>
[20] Zhu, W., Han, Y., Lu, J., & Zhou, J. (2022). Relational reasoning over spatial-temporal graphs for video summarization. IEEE Transactions on Image Processing, 31, 3017-3031.<br>
