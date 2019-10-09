# XMLScripts-Project-AWGStepTesting
XMLScript project that allows measuring the steps between all input values and it’s successor of a SAG1021.

To get this repository with all its submodules the following command might be of use 

git clone --recurse-submodules https://github.com/HendriXML/XMLScripts-Project-AWGStepTesting.git C:\AWGStepTesting

What's needed to use this script?
* SAG1021
* NI VISA setup (It uses a COM interface that comes with it)
* Ethernet/Wifi connection on Scope (Using the above with USB fails)
* Interpreter executable (64 bit Windows, developed by me)
* Script + Script libraries
* XML editor to alter some values (for example an offset to get the first batch in view, scopes ip-adress). I really like the free Visual Studio Community for that.
* about 2 hours of executing time

The first run of the script will probably not have the waveform in view, because of the 5mV/div it needs an accurate DSO offset. Using the pause checkbox the script will pause the execution, making manual adjustments possible. Unchecking pause and pushing resume will continue without further pausing. (But it can be checked at anytime, to request a pause. The script has a script element for that to check this.)

## Automatically test AWG output.xml
Main script to find extreme transitions steps

## Dual AWG value test.xml
Script to generate a waveform with only 2 values in it, usefull to zoom in on the transition between them
