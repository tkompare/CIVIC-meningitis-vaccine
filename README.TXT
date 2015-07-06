I have again partnered with the Chicago Department of Public Health (CDPH) to create a meningitis vaccine clinic event finder web application. Currently it has all the CDPH free locations and events. You will notice it is a slightly altered version of the 'flushots2013' code. Well, I had to make this thing work in two days. So that's what you get. Public health emergencies are like that sometimes.

I created this as a volunteer effort. The code that runs it is open, completely free, and reusable by anyone.

Special thanks to Smart Chicago for hosting this thing. Also thanks to Raed Mansour and  Commissioner Dr. Julie Morita (both with CDPH) for being great to work with. Chicago, you don't know how lucky you are to have these two working for you.

Launch Instructions:
1) If you look at /webapp/index.html toward the bottom of the file, you will see a note about minimizing & concatenating Javascript files. I use a software product called Codekit to mash all of the commented out JS files into one main-min.js file. If you do not have access to such a tool, uncomment all of the JS files, and comment out the main-min.js file reference.
2) Look inside the 'main.js' file's 'Default' array to alter most things to your own locale.
3) Make sure to change to your own Google API keys in main.js in 'Default' array, and index.html towards the bottom of the file.
4) Make sure to change the Google Analytics ID towards the bottom of index.html, or remove it completely if you are not using it.
5) Launch all the files and directories within /webapp into the root directory of wherever you are hosting you version of this web application.
6) A note about the '/server-php/ical.php' file: This is the file that reflects back an .ical appointment to the persons using this application. Place it on a PHP enabled web server. Its function could easily be rewritten into a variety of other server-side programming languages by a competent programmer. Please point to this PHP file's URL by altering 'echoUrl' property found inside the 'setIcal' function in the 'flushots.js' file.
7) Yes, you'll see a lot references to "flu shots" in the code. I started this web app from a copy of my Flu Shots finder web application. Like I said, I made this in a hurry. Corners needed to be cut. This was one of them. At some point, these two applications will become one. That's my lofty goal, anyway.