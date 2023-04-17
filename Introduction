# GIB-LSTM
# Semantic representation and attention alignment for Graph Information Bottleneck in video summarization  

## Introduction

We adopted the Graph Information Bottle (GIB) to develop a Contextual Feature Transformation (CFT)  mechanism that refines the temporal two-stream feature, yielding a semantic representation with attention alignment. Furthermore, a novel Salient-Area-Size-based spatial attention model is presented to extract frame-wise visual features based on the observation that humans tend to focus on sizable and moving objects. Finally, semantic representation is embedded within attention alignment under the end-to-end LSTM framework to differentiate indistinguishable images.

![](https://github.com/wangrui91/GIB-LSTM/blob/main/images/GIB-LSTM.png)

##  Experiments
#### 主观实验结果
Comparison with the state-of-the-art unsupervised video summarization methods on the SUMME and TVSUM datasets under the canonical setting  (F-score%)

<table class=MsoTableGrid border=1 cellspacing=0 cellpadding=0
 style='border-collapse:collapse;border:none;mso-border-alt:solid windowtext .5pt;
 mso-yfti-tbllook:1184;mso-padding-alt:0cm 5.4pt 0cm 5.4pt'>
 <tr style='mso-yfti-irow:0;mso-yfti-firstrow:yes'>
  <td width=150 valign=top style='width:112.8pt;border-top:solid windowtext 1.0pt;
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;
  mso-border-top-alt:solid windowtext 1.0pt;mso-border-bottom-alt:solid windowtext .75pt;
  padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>Method<o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border-top:solid windowtext 1.0pt;
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;
  mso-border-top-alt:solid windowtext 1.0pt;mso-border-bottom-alt:solid windowtext .75pt;
  padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>SumMe</span></span><span lang=EN-US style='font-size:12.0pt;font-family:
  "Times New Roman",serif;mso-fareast-font-family:CMR8;color:black;mso-font-kerning:
  0pt;mso-bidi-language:AR'><o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border-top:solid windowtext 1.0pt;
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;
  mso-border-top-alt:solid windowtext 1.0pt;mso-border-bottom-alt:solid windowtext .75pt;
  padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>TVSum</span></span><span lang=EN-US style='font-size:12.0pt;font-family:
  "Times New Roman",serif;mso-fareast-font-family:CMR8;color:black;mso-font-kerning:
  0pt;mso-bidi-language:AR'><o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:1'>
  <td width=150 valign=top style='width:112.8pt;border:none;mso-border-top-alt:
  solid windowtext .75pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>K-<span class=SpellE>medoids</span> <o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;mso-border-top-alt:
  solid windowtext .75pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>33.4<o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;mso-border-top-alt:
  solid windowtext .75pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>28.8<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:2'>
  <td width=150 valign=top style='width:112.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>Vsumm</span></span><span lang=EN-US style='font-size:12.0pt;font-family:
  "Times New Roman",serif;mso-fareast-font-family:CMR8;color:black;mso-font-kerning:
  0pt;mso-bidi-language:AR'><o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>33.7<o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>-<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:3'>
  <td width=150 valign=top style='width:112.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>Web image<o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>-<o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>36.0<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:4'>
  <td width=150 valign=top style='width:112.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>Dictionary selection<o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>37.8<o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>42.0<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:5'>
  <td width=150 valign=top style='width:112.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>Online sparse coding<o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>-<o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>46.0<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:6'>
  <td width=150 valign=top style='width:112.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>Co-archetypal<o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>-<o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>50.0<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:7'>
  <td width=150 valign=top style='width:112.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>GANdpp</span></span><span lang=EN-US style='font-size:12.0pt;font-family:
  "Times New Roman",serif;mso-fareast-font-family:CMR8;color:black;mso-font-kerning:
  0pt;mso-bidi-language:AR'><o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>39.1<o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>51.7<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:8'>
  <td width=150 valign=top style='width:112.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>DR-DSN<o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>41.4<o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>57.6<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:9'>
  <td width=150 valign=top style='width:112.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>Cycle-SUM<o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>41.9<o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>57.6<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:10'>
  <td width=150 valign=top style='width:112.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>CSNet</span></span><span lang=EN-US style='font-size:12.0pt;font-family:
  "Times New Roman",serif;mso-fareast-font-family:CMR8;color:black;mso-font-kerning:
  0pt;mso-bidi-language:AR'><o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>51.3<o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>58.8<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:11'>
  <td width=150 valign=top style='width:112.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>GAT-LSTM<o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>51.5<o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>59.1<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:12'>
  <td width=150 valign=top style='width:112.8pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>DSAVS<o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>47.0<o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>59.4<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:13;mso-yfti-lastrow:yes'>
  <td width=150 valign=top style='width:112.8pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>Proposed<o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><b><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>55.0<o:p></o:p></span></b></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><b><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;color:black;mso-font-kerning:0pt;mso-bidi-language:
  AR'>62.5<o:p></o:p></span></b></p>
  </td>
 </tr>
</table>

Comparison with the state-of-the-art supervised video summarization methods on the SUMME and TVSUM datasets under the canonical setting  (F-score%)

<table class=MsoTableGrid border=1 cellspacing=0 cellpadding=0
 style='border-collapse:collapse;border:none;mso-border-alt:solid windowtext .5pt;
 mso-yfti-tbllook:1184;mso-padding-alt:0cm 5.4pt 0cm 5.4pt'>
 <tr style='mso-yfti-irow:0;mso-yfti-firstrow:yes'>
  <td width=150 valign=top style='width:112.8pt;border-top:solid windowtext 1.0pt;
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;
  mso-border-top-alt:solid windowtext 1.0pt;mso-border-bottom-alt:solid windowtext .75pt;
  padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>Method</span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border-top:solid windowtext 1.0pt;
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;
  mso-border-top-alt:solid windowtext 1.0pt;mso-border-bottom-alt:solid windowtext .75pt;
  padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>SumMe</span></span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border-top:solid windowtext 1.0pt;
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;
  mso-border-top-alt:solid windowtext 1.0pt;mso-border-bottom-alt:solid windowtext .75pt;
  padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>TVSum</span></span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:1'>
  <td width=150 valign=top style='width:112.8pt;border:none;mso-border-top-alt:
  solid windowtext .75pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>Interestingness</span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;mso-border-top-alt:
  solid windowtext .75pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>39.4</span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;mso-border-top-alt:
  solid windowtext .75pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>-</span><span lang=EN-US style='font-size:
  12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:CMR8;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:2'>
  <td width=150 valign=top style='width:112.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>Submodularity</span></span><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;mso-bidi-font-family:"Times New Roman";
  mso-bidi-theme-font:minor-bidi;color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>39.7</span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>-</span><span lang=EN-US style='font-size:
  12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:CMR8;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:3'>
  <td width=150 valign=top style='width:112.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>Summary transfer</span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>40.9</span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>-</span><span lang=EN-US style='font-size:
  12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:CMR8;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:4'>
  <td width=150 valign=top style='width:112.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>Bi-LSTM</span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>37.6</span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>54.2</span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:5'>
  <td width=150 valign=top style='width:112.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>Dpp</span></span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-bidi-font-family:
  "Times New Roman";mso-bidi-theme-font:minor-bidi;color:black;mso-font-kerning:
  0pt'>-LSTM</span><span lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;mso-bidi-font-family:"Times New Roman";
  mso-bidi-theme-font:minor-bidi;color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>38.6</span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>54.7</span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:6'>
  <td width=150 valign=top style='width:112.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>GANsup</span></span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>41.7</span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>56.3</span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:7'>
  <td width=150 valign=top style='width:112.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>DR-<span class=SpellE>DSNsup</span></span><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;mso-bidi-font-family:"Times New Roman";
  mso-bidi-theme-font:minor-bidi;color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>42.1</span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>58.1</span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:8'>
  <td width=150 valign=top style='width:112.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>Cycle-<span class=SpellE>SUMsup</span><o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>44.8<o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>58.1<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:9'>
  <td width=150 valign=top style='width:112.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>CSNetsup</span></span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>48.6</span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>58.5</span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:10'>
  <td width=150 valign=top style='width:112.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>CRSum</span></span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>47.3</span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>58.0</span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:11'>
  <td width=150 valign=top style='width:112.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>GAT-<span class=SpellE>LSTMsup</span></span><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;mso-bidi-font-family:"Times New Roman";
  mso-bidi-theme-font:minor-bidi;color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  mso-font-kerning:0pt;mso-bidi-font-weight:bold'>51.7</span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt;mso-bidi-font-weight:bold'><o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt;mso-bidi-font-weight:bold'>59.6</span><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;mso-bidi-font-family:"Times New Roman";
  mso-bidi-theme-font:minor-bidi;color:black;mso-font-kerning:0pt;mso-bidi-font-weight:
  bold'><o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:12'>
  <td width=150 valign=top style='width:112.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>DSAVSsup</span></span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-bidi-font-family:
  "Times New Roman";mso-bidi-theme-font:minor-bidi;color:black;mso-font-kerning:
  0pt'><o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  mso-font-kerning:0pt;mso-bidi-font-weight:bold'>48.9<o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt;mso-bidi-font-weight:bold'>59.8<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:13'>
  <td width=150 valign=top style='width:112.8pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  class=SpellE><span lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>DSNet</span></span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-bidi-font-family:
  "Times New Roman";mso-bidi-theme-font:minor-bidi;color:black;mso-font-kerning:
  0pt'><o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  mso-font-kerning:0pt;mso-bidi-font-weight:bold'>50.2<o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt;mso-bidi-font-weight:bold'>62.1<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:14'>
  <td width=150 valign=top style='width:112.8pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>RR-STG<o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  mso-font-kerning:0pt;mso-bidi-font-weight:bold'>53.4<o:p></o:p></span></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><b><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>63.0<o:p></o:p></span></b></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:15;mso-yfti-lastrow:yes'>
  <td width=150 valign=top style='width:112.8pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-top-alt:solid windowtext .5pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>Proposed</span><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width=122 valign=top style='width:91.5pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-top-alt:solid windowtext .5pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><b><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'>56.0</span></b><b><span lang=EN-US
  style='font-size:12.0pt;font-family:"Times New Roman",serif;mso-fareast-font-family:
  CMR8;mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt'><o:p></o:p></span></b></p>
  </td>
  <td width=135 valign=top style='width:101.5pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-top-alt:solid windowtext .5pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-bidi-font-family:"Times New Roman";mso-bidi-theme-font:minor-bidi;
  color:black;mso-font-kerning:0pt;mso-bidi-font-weight:bold'>62.7</span><span
  lang=EN-US style='font-size:12.0pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:CMR8;mso-bidi-font-family:"Times New Roman";
  mso-bidi-theme-font:minor-bidi;color:black;mso-font-kerning:0pt;mso-bidi-font-weight:
  bold'><o:p></o:p></span></p>
  </td>
 </tr>
</table>


#### 客观实验结果

![](https://github.com/wangrui91/GIB-LSTM/blob/main/images/Visualization.png)
