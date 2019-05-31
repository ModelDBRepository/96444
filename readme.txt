This is the readme for the model for the paper:

Hines ML, Carnevale NT.
Translating network models to parallel hardware in NEURON.
J Neurosci Methods. 2008 Apr 30;169(2):425-55.

=====
USAGE
=====

You may either autolaunch from your browser, or download 
the zip file and run the simulations manually.


1.  Autolaunching from ModelDB
------------------------------

A "Launch" panel will appear that offers four buttons labeled
  Ring (Serial)
  Ring (Parallel)
  Random (Serial)
  Random (Parallel)
Click on one of these to run a simulation.  Results will be 
printed in the terminal window.  At the end of a run, you may 
run another simulation, or exit.


2.  Download zip file
---------------------

Expand the zip file in an empty directory.
The ring and random network files are in 
  HinesCarnevaleJNM2007/ring
and
  HinesCarnevaleJNM2007/random
respectively.

Before running the random network simulations, you must first 
compile the mod files in HinesCarnevaleJNM2007/random with mknrndll 
(MSWin, OS X) or nrnivmodl (UNIX/Linux).
If you're not sure how, see
http://www.neuron.yale.edu/neuron/docs/faq.html#compilemod

To run a simulation manually:

UNIX/Linux--
cd into the ring or random subdirectory
At the system prompt, type
  nrngui filename
where filename is one of the following:
  ringser.hoc
  ringpar.hoc
  ran3ser.hoc
  ran3par.hoc

MSWin--
Double click on ringser.hoc, ringpar.hoc, ran3ser.hoc, or 
ran3par.hoc
If the simulation finishes and exits too quickly, open the 
hoc file with a plain text editor and change the last 
statement from 
  quit()
to
// quit()
Save the hoc file and try again.  It will now be necessary 
to type ^D (control-D) or quit() at the oc> prompt to exit 
NEURON.

OS X--
Double click on ringser.hoc, ringpar.hoc, ran3ser.hoc, or 
ran3par.hoc
  or
drag and drop the hoc file on the nrngui icon in the NEURON 
application folder.
If the simulation finishes and exits too quickly, edit the 
hoc file as suggested for MSWin.
