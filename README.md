SeminarAlgorithms
=================

Course TU Delft considering replanning algorithms

### Todo still

- Determine goal
- Change titel to fit goal
- Find second paper to focus on
- Contact authors of the paper
- Determine hypotheses for the paper
- Identify different ways of solving problems
- Identify weak point in state of the art
- Describe experiment / create roadmap
- Develop a domain and argument why this is better than current domains (has to be scalable)
- Write domain in PDDL
- Stimulate fails either online vs offline
- Experiment by tweeking the current algorithms
- Describe foundings of the experiment
- Try to adjust
- Conclude
- Future works


### RDDLSim & Glutton

#### RDDLSim

Installation of RDDLSim: https://code.google.com/p/rddlsim/source/browse/trunk/INSTALL.txt

Basically download with SVN:

	svn checkout http://rddlsim.googlecode.com/svn/trunk/ rddlsim

Then to start the server:

	cd rddlsim
	./run rddl.competition.Server files/final_comp/rddl


#### Glutton / G-pack

Download the [G-pack](http://www.cs.washington.edu/ai/planning/glutton.html).

	cd G-pack-2.0
	make

Run the planner

	./planner localhost:2323 ../rddlsim-read-only/files/final_comp/ppddl/navigation_inst_mdp__1.ppddl navigation_inst_mdp__1

To write it to a file, append `> log`.

To see the content of the log file 'in real time', in another terminal window

	tail -F log


#### RDDL Files

The files that are tested so far are the final_comp files, which are from the 2011 competition.
Glutton uses the ppddl files as problem files. The server does use the rddl files as domain files.

rddl files can be translated to ppddl files (see INSTALL.txt of rddlsim).
