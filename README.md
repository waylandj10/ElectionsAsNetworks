# Elections_as_Networks
<<<<<<< HEAD
A class project for CS510 and CS520 in the CADS PhD program at Chapman University.

## Usage
Use Voting_Systems_in_R.ipynb: this is an interactive jupyter notebook, loaded with an R kernel. To run this notebook you'll need a way to host a jupyter notebook (e.g. via Anaconda. See https://docs.anaconda.com/anaconda/install/). You can add an R kernel by following this guide: https://irkernel.github.io/.
The project contains a playground for understanding randomly generated election scenarios, as well as a script to compute the outcome of the 2016 Presidential election. Data is pulled live from https://electionlab.mit.edu/ and could be used to compute the result of the 2020 election once data becomes available. The electoral votes per state are stored in electoral_votes_per_state.csv.

## Context
Systems that describe how inputs transition into outputs are ubiquitous in science and engineering. We draw networks and diagrams to capture these processes and solve complex problems. How do we reason about such systems? Mathematically, how do we represent a network with inputs and outputs? Is there a formalism to confirm our intuition for how these networks should combine and/or run in parallel? Probing these questions is an active field of research in network theory and applied category theory. Currently, two main formalisms exist: both were developed by Dr. John Baez and his cohort at the University of California, Riverside. The first goes by "structured cospans" and the second "decorated cospans".

Don't get hung up on these names; these are just abstract ways of looking at networks (much too abstract for this computational course) that help mathematicians understand them. This formalism helps answer questions of the following type: what does the entire class of networks look like? How do different types of specialized networks relate to each other? I think you can (but might not want to) imagine more questions of this type that really get a mathematicians gears turning. Anyway, the golden question is always: how is this useful? This formalism has been used to capture the action of markovian processes, chemical reaction networks, electrical circuits, and Petri Nets. The hope is to develop a better understanding of how these networks behave in theory, so that one day we can leverage this understanding to give a practical/computational advantage. Given the ubiquity and robustness of network diagrams, I think its a good bet to continue building out this theory.

One type of network that wasn't studied until recently was voting systems. Why is a voting system a network? Well, voters first cast a ballot (the input to the network), the governing body goes through some transition phase were they aggregate the votes and evenutally determine the winners (the output). Now you may ask, what can be gained from viewing an election as a network? In short, theres no guarunteed upshot but it could help shed light on some interesting conundrums. Developing the formalism for elections as networks was the subject of my undergraduate honors thesis, which I completed in December of 2019 (Wayland2019 in the repo). Why go on such an endeaouver? I ask that myself all the time...

The answer is there are many open questions in Social choice theory (the formal study of collective decision processes). Basically elections don't actually work the way we would expect. There seems to be corruption hard coded into the theory (see Arrow's or Gibbard–Satterthwaite's theorem for details). And one would think the corruption could be traced back to human indecency... In practice you often can, but not many people realize how suspect the theory itself is. I digress, but here's the point: there might be a yield to approaching voting systems from a different angle to try and get additional perspecitve on why these strage behaviors occur. With an abundance of formalism on networks at my disposal, which use category theory (a pure math interest of mine) as their main machinery, I figured it was worth a shot.

## Project description
As you can see this research is ambitous in scope. The portion alotted for this course is quite simple and concrete: check whether computing the result of an elections, when viewing it as a network, can be implemented in a reasonable way. One of the upshots provided by Wayland2019 is that elections (as networks) are composable; a large election is simply a composition of smaller ones which can be more easily specified in the formalism. As a token example of a multistage election, I chose to look into computing the result of a presidential election using this formalism.

## Next Steps
This project is a contribution to a larger research initiative: to package the formalism of structured cospans and the subsequent results on the theory of networks into a strongly typed language that can be leveraged by scientists using networks. The idea is to provide universal accessibility to the formalism via an open source interface, eliminating the need to parse through dozens of papers and advancing the use of category theory in modern applied sciences. This project is an experiment attempting to determine which parts of the formalism are important when looking at voting systems; this will hopefully give insight into the best implementation	for the general network formalism.


=======
A class project for CS510 and CS520 in the CADS PhD program at Chapman University that looks to extend my research as an undergrad. The goal will be to implement the action performed when computing the results of an election in a way that is consistent with category theory models of generalized open networks. Details on the goals and background of this project can be found in Wayland2019 and Project_Proposal. Initially this project will simulate a generalized voting system using R. Once a foundational understanding has been achieved from a programming perspective, the implementation can be translated into Haskell which has the potential to truly build a model consistent with the underlying category theory.


## Current Progress
All that has been developed thus far is a playground (programmed in R) for testing out and understanding the compuational aspects of computing an election when we view it formally as a specialized type of network. More than anything, this is a mental check that the formalism developed in Wayland2019 can indeed compute the outcome of a given election, for example a presidential election. 
* See Elections_as_Networks/R/Voting_Systems_in_R.ipynb to interact
* Note: this is a jupyter notebook run with an R kernel. To run this notebook you'll need a way to host a jupyter notebook (e.g. via Anaconda https://docs.anaconda.com/anaconda/install/). You can add an R kernel by following this guide: https://irkernel.github.io/
>>>>>>> 2a800a3b91729b923bce4c13d0de4c03cd34b5b5
