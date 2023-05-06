Download Link: https://assignmentchef.com/product/solved-economics7103-hw7
<br>
You have access to imaginary vehicle sales data from 2017 (<em>instrumentalvehicles.csv</em>). You are interested in estimating the hedonic price of an additional mile per gallon as part of a larger analysis of willingness to pay for fuel efficiency. In your data, you have the following variables:

<table width="526">

 <tbody>

  <tr>

   <td width="64">Variable</td>

   <td width="462">Description</td>

  </tr>

  <tr>

   <td width="64"><em>price</em></td>

   <td width="462">Sales price of the vehicle in USD</td>

  </tr>

  <tr>

   <td width="64"><em>car</em></td>

   <td width="462">Class of the vehicle. =1 if the vehicle is a sedan, =0 if the vehicle is an SUV</td>

  </tr>

  <tr>

   <td width="64"><em>mpg</em></td>

   <td width="462">Fuel efficiency in miles per gallon</td>

  </tr>

  <tr>

   <td width="64"><em>weight</em></td>

   <td width="462">Weight of the vehicle in pounds</td>

  </tr>

  <tr>

   <td width="64"><em>height</em></td>

   <td width="462">Height of the vehicle in inches</td>

  </tr>

  <tr>

   <td width="64"><em>length</em></td>

   <td width="462">Length of the vehicle in inches</td>

  </tr>

 </tbody>

</table>

Table 1: Variable descriptions for homework 6.

<ol>

 <li>Run the ordinary-least-squares regression of price on <em>mpg</em>, the <em>car </em>indicator variable, and a constant. Report and interpret the coefficient on miles per gallon (do not construct a table).</li>

 <li>What forms of endogeneity are you concerned about when estimating the coefficient on <em>mpg</em>?</li>

 <li>To correct for this endogeneity, you would like to use instrumental variables. Specifically, you areinterested in the system of equations:</li>

</ol>

<table width="401">

 <tbody>

  <tr>

   <td width="384"><em>price<sub>v </sub></em>= <em>β</em><sub>0 </sub>+ <em>β</em><sub>1</sub><em>mpg<sub>v </sub></em>+ <em>β</em><sub>2</sub><em>car<sub>v </sub></em>+ <em>e<sub>v</sub></em></td>

   <td width="17">(1)</td>

  </tr>

  <tr>

   <td width="384"><em>mpg<sub>v </sub></em>= <em>γ</em><sub>0 </sub>+ <em>γ</em><sub>1</sub><em>z<sub>v </sub></em>+ <em>γ</em><sub>2</sub><em>car<sub>v </sub></em>+ <em>u<sub>v</sub>,</em></td>

   <td width="17">(2)</td>

  </tr>

 </tbody>

</table>

where <em>z<sub>v </sub></em>is the value of the instrument for vehicle <em>v </em>and <em>e<sub>v </sub></em>and <em>u<sub>v </sub></em>are error terms. Report the estimated second-stage coefficients, standard errors or confidence intervals, and the first-stage <em>F</em>-statistic for the excluded instrument in the same table for the following procedures (just us a regular F-statistic for this exercise rather than the robust Montiel-Olea-Pflueger F-statistic):

(a) Perform two-stage-least-squares estimation by hand using <em>weight </em>as the excluded instrument. (First regress <em>mpg </em>on all of the instruments. Save the fitted values from the first stage <em>mpg</em>ˆ and use the fitted values in place of the endogenous variable in the second stage price regression.) (b) Perform two-stage-least-squares estimation by hand using <em>weight</em><sup>2 </sup>as the excluded instrument.

<ul>

 <li>Perform two-stage-least-squares estimation by hand using <em>height </em>as the excluded instrument.</li>

 <li>In words, what are the different exclusion restrictions required for parts (a)-(c)? Does this seemreasonable for these instruments?</li>

 <li>Compare and contrast the estimated coefficient on <em>mpg </em>from parts (a)-(c). What explains the discrepancies?</li>

</ul>

<ol start="4">

 <li>Calculate the IV estimate using GMM with <em>weight </em>as the excluded instrument. (Look for the Linearmodels function IVGMM). Report the estimated second-stage coefficient and standard error or confidence interval for <em>mpg </em>What factors account for the differences in the standard errors?</li>

</ol>