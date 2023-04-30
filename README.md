Download Link: https://assignmentchef.com/product/solved-geological-computing-homework-3-the-volume-of-water-in-crater-lake
<br>
Save your scripts to a directory named <em>Homework-3 </em>in your home account on the server computer in SCA 219 (131.247.211.166); do not email your answers. A short report should be typed and submitted in PDF format; drawings and/or flowcharts may be hand-drawn, just be legible! Multiple pages should be stapled together. Some additional explanation is helpful and often necessary for the person reading your assignment to understand exactly what you are doing and why. Assume that the person grading your assignment does not have a copy of the assignment. What is important here is that <em>(1) </em>you understand what you are doing, and <em>(2) </em>that you can communicate what you are doing to others. Introduction

The crater of Crater Lake is filled with water. The elevation of the surface of the water is approximately 1883m above sea level. Surveys to determine the depth of Crater Lake were made in 1886, 1938-40, 1959, and most recently in 2000. The 1959 survey used echo-sounding technology, and measured the time it takes for sound to bounce off the lake floor, collecting depth information at more than 6,000 locations every 30 meters.

<h2>Problem 1a</h2>

Your goal in this part of the assignment is to create a data file that encompasses the boundaries of Crater Lake and provides depth information for the areas under water. The format of the data file should be <em>X Y Z</em>, where <em>X </em>is the Easting, <em>Y </em>is the Northing, and <em>Z </em>is the elevation of the locations under water. The data for this task is located online at: <a href="http://oe.oregonexplorer.info/craterlake/bathymetry.html">http://oe.oregonexplorer.info/craterlake/bathymetry.html</a>

Proceed as follows:

<ul>

 <li>Download the 1959 bathymetry survey (30-m resolution, <em>.dem </em>format, 420 KB compressed, 3 MB uncompressed). Uncompress (unzip) this file.</li>

 <li>Download the Perl script, <em>dem2xyz </em>from this link: <a href="https://projects.eri.ucsb.edu/mapcat/bin">https://projects.eri.ucsb.edu/mapcat/bin</a></li>

</ul>

Right-click on this file, <em>dem2xyz </em>and save the Perl script as: <em>dem2xyz.pl</em>

<ul>

 <li>Execute this Perl script to convert the 1959 <em>.dem </em>format data file into an <em>X Y Z </em>format data file. The Perl script will create a data file having the <em>X Y Z </em>format; this <em>X Y Z </em>data file will be named <em>dem.xyz</em>.</li>

 <li>Develop a flowchart that shows the steps necessary to filter the lines of data in <em>dem.xyz </em>to only include data located between the following coordinates (<em>roughly </em>the area of the lake):</li>

</ul>

Easting: 568000 to 577500

Northing: 4750500 to 4758500

Your output should be saved to a new file; name this file <em>filtered crater lake data.xyz</em>. Your flowchart needs to show the inputs, the outputs, and your procedure. Be specific and use the flowchart tools described in homework 2!

<ul>

 <li>Write a Perl or Python script based on this flowchart. Be sure to add comment lines to your script so that the lines in your code can be related to your flow chart. Remember, each comment line begins with the character, #.</li>

</ul>

1

<ul>

 <li>Execute this script and save the filtered data to a file named <em>filtered crater lake data.xyz</em>. You will use this data file in the next part of this assignment.</li>

</ul>

<h2>Problem 1b</h2>

Now, your goal is to find (1) the surface area of Crater Lake, (2) the volume of water in Crater Lake, and (3) the maximum depth of Crater Lake.

Bathymetric data obtained from surveys of the lake is needed to complete this assignment. The text file you created previously, <em>filtered crater lake data.xyz</em>, contains this data. Each line of the file has three numerical values separated by white space. These data should be the Easting (m), the Northing (m), and the Elevation (m above sea level) of locations encompassing Crater Lake. Use the following procedure:

<ul>

 <li>Develop a flowchart that shows the steps necessary to calculate the surface area of the lake, the volume of water in the lake, and the maximum depth of the lake using the bathymetric data file <em>filtered crater lake data.xyz</em>. Your flowchart needs to show the inputs, the outputs, and the procedures you use. Be specific and use the flowchart tools described in Homework 2!</li>

 <li>Write a Perl or Python script based on this flowchart. Be sure to comment your script so that the lines in your code can be related to your flow chart. Your script should calculate (1) the surface area of the lake, (2) the volume of water in the lake, (3) the maximum depth of the lake, and (4) print out the results. Please show your units.</li>

 <li>Turn in a short report that includes (1) the problem statements from parts 1a and 1b, (2) your flowchart(s) for solving these problems, (3) the command lines you used to run your script(s), and (4) the final output from your last script, that is, include three sentences stating the values you calculated and their units:

  <ol>

   <li>I found the surface area of Crater Lake to be <em>&lt;your value</em><em>&gt;</em>.</li>

   <li>I found the volume of Crater Lake to be <em>&lt;your value</em><em>&gt;</em>.</li>

   <li>I found the greatest depth in Crater Lake to be <em>&lt;your value</em><em>&gt;</em>.</li>

  </ol></li>

</ul>

<em>Units are important! </em>Don’t forget to include them with your value. The scripts and data file you used to do your calculations should be saved to the Homework-3 directory you created (see above).

2