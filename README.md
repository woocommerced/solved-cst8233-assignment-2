Download Link: https://assignmentchef.com/product/solved-cst8233-assignment-2
<br>
<strong>Linear Regression Fit to Data  </strong>

<strong><em> </em></strong><strong>Purpose:</strong> Fit data using linear regression least squares method for both a Linear function and a Power Law function.

<strong>Algorithm. </strong>Write a program named that will enable the user to fit data to both a linear and a power law function.




Here is a data set for CO<sub>2</sub> levels in the World over a range of years.

<table width="639">

 <tbody>

  <tr>

   <td width="103">year</td>

   <td width="53">1960</td>

   <td width="54">1965</td>

   <td width="53">1970</td>

   <td width="54">1975</td>

   <td width="54">1980</td>

   <td width="53">1985</td>

   <td width="53">1990</td>

   <td width="54">1995</td>

   <td width="53">2000</td>

   <td width="54">2005</td>

  </tr>

  <tr>

   <td width="103">CO2 level ppm</td>

   <td width="53">316.5</td>

   <td width="54">320</td>

   <td width="53">325</td>

   <td width="54">331</td>

   <td width="54">338</td>

   <td width="53">346</td>

   <td width="53">353</td>

   <td width="54">360</td>

   <td width="53">368.5</td>

   <td width="54">378</td>

  </tr>

 </tbody>

</table>




The supplied data file you will use for the fits, CO2.txt shown below, is the same data as above but 1960 has been subtracted from each of the years and 316.5 has been subtracted from each CO2 level. In other words, 1960 is the start year and levels are measured relative to what it was in that year. This is done to reduce the size of products and sums that occur in the least-squares formulas and increase to accuracy of the results. <strong><em>CO2.txt </em></strong>

<table width="585">

 <tbody>

  <tr>

   <td width="103">year</td>

   <td width="54">5</td>

   <td width="53">10</td>

   <td width="54">15</td>

   <td width="53">20</td>

   <td width="54">25</td>

   <td width="53">30</td>

   <td width="54">35</td>

   <td width="53">40</td>

   <td width="54">45</td>

  </tr>

  <tr>

   <td width="103">CO2 level ppm</td>

   <td width="54">3.5</td>

   <td width="53">8.5</td>

   <td width="54">14.5</td>

   <td width="53">21.5</td>

   <td width="54">29.5</td>

   <td width="53">36.5</td>

   <td width="54">43.5</td>

   <td width="53">52</td>

   <td width="54">61.5</td>

  </tr>

 </tbody>

</table>




<ol>

 <li><strong>Fit to a Linear function y = mx + c </strong></li>

</ol>

In the linear case you are fitting the CO2.txt data to the straight line y = mx + c, where y represents the CO2 level and x represents the year in the file CO2.txt and m and c are constants. Solve these equations using the least-squares linear regression formulas in the lecture notes to get to get solutions for m and c. Using the fit, offer the user the option of interpolating/extrapolating the data by including the (1960, 316.5) offsets to the formula you calculate.

<strong> </strong>

<ol start="2">

 <li><strong>Fit to a power law y = ax<sup>b</sup>. </strong></li>

</ol>

In this case you are fitting the data to the power law y = ax<sup>b</sup> where y represents the CO2 level and x represents the year in the file CO2.txt and a and b are constants. To do a linear regression the data need to be transformed as dicussed in class notes. With the transformed data solve the least-squares linear regression formulas in the lecture notes to get solutions for a and b. Then using the power law formula, offer the user the option of interpolating/ extrapolating the data by including the (1960, 316.5) offsets to the formula you calculate.

<strong> </strong>

Set up a Win32 console project in Visual Studio 2015 with the name ass1. In a file named ass1.cpp using the C (or/C++) programming language, write the code to implement the application, as described above,. Example output is given at the end. Yours should be the same. Note than your assignment might be

tested with a different data file with a different number of entries and with different interpolation/extrapolation parameters than those shown.




See the Marking Sheet for how you can lose marks, but you definitely lose 60% or more if:

<ul>

 <li>your application won’t build in Visual Studio 2015</li>

 <li>your application crashes in normal operation or with a different data file</li>

 <li>I can’t build it because you submitted the wrong files or the files are missing, even if it’s an honest mistake – 100% deduction.</li>

</ul>




1




CST 8233 – F18 – Assignment #2                                                           A.Tyler




<strong> </strong>

<strong>What to Submit : </strong>Use Brightspace to submit this assignment as a zip file (<strong>not </strong>RAR, not 9zip, not 7 zip) containing only the source code file (ass2.cpp). The name of the zipped folder <strong><u>must </u></strong>contain your name as a prefix so that I can identify it, for example using my name the file would be tyleraAss2CST8233.zip. It is also vital that you include the Cover Information (as specified in the Submission Standard) as a file header (you don’t need to include an additional separate file header) in your source file so the file can be identified as yours. Use comment lines in the file to include the information.

There is a late penalty of 25% per day – even one minute is counted late. Don’t send me the file as an email attachment – it will get 0.




<strong><em>Example Output </em></strong>

LEAST_SQUARES LINEAR REGRESSION

MENU

<ol>

 <li>Linear Fit</li>

 <li>Power Law Fit</li>

 <li>Quit</li>

</ol>

2

Please enter the name of the file to open: CO2.txt

There are 9 records.

y = 0.43x^1.31

MENU

<ol>

 <li>Interpolate/Extrapolate</li>

 <li>Main Menu</li>

</ol>

1

Please enter the year to interpolate/extrapolate to: 2020 The power law interpolated/extrapolated CO2 level in the year 2020.0 is 405.99 MENU

<ol>

 <li>Interpolate/Extrapolate</li>

 <li>Main Menu</li>

</ol>

1

Please enter the year to interpolate/extrapolate to: 1968 The power law interpolated/extrapolated CO2 level in the year 1968.0 is 322.94 MENU

<ol>

 <li>Interpolate/Extrapolate</li>

 <li>Main Menu</li>

</ol>

2




LEAST_SQUARES LINEAR REGRESSION

MENU

<ol>

 <li>Linear Fit</li>

 <li>Power Law Fit</li>

 <li>Quit</li>

</ol>

1

Please enter the name of the file to open: CO2.txt

There are 9 records. y = 1.45*x + -6.18

MENU

<ol>

 <li>Interpolate/Extrapolate</li>

 <li>Main Menu</li>

</ol>

1

Please enter the year to interpolate/extrapolate to: 2020 The linear interpolated/extrapolated CO2 level in the year 2020.0 is 397.42

MENU

<ol>

 <li>Interpolate/Extrapolate</li>

 <li>Main Menu</li>

</ol>

1

Please enter the year to interpolate/extrapolate to: 1968 The linear interpolated/extrapolated CO2 level in the year 1968.0 is 321.93

MENU

<ol>

 <li>Interpolate/Extrapolate 2. Main Menu</li>

</ol>




2


