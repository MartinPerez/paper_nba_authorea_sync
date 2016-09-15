Once we have the neural dynamic segments of the compartment circuit, we need specification of the timing of parsing operations, the hypothesized tree structure to represent and the desired duration of WM activity. The number of compartment circuits necessary to make the simulation simply come from the tree structure. The timing of parsing operations is the time at which we expect each of the nodes of the tree structure to be translated into the WM activity of some compartment circuit. One can see in Figure \ref{sentence_example} how the hypothesized tree structure of a sentence and the timing of the activation of tree nodes is transformed into the neural activity of a blackboard.

We assume that WM activation is long enough to allow all bindings in the tree to happen as words are incorporated in blackboard. For example if words are presented every 600 ms, we assume WM is active for around 3 seconds to bind the first word to an awaited phrase node activated after a fifth word, if WM was active for say less than 2.4s then activation of the MA would cease before the other MA and Ctl populations come into play for that compartment circuit.

Control delay considered 50ms after target word for 100ms, very naive version of xxx parsing. important to have in mind that there are other parsing possibilities. Look into generalized left corner parsing of Hale.

We take activity minus baseline activity to look at differences in neural activity.

We normalize time series to look at relative and qualitative effects. Moreover to give equal weight to time series in a regression model and allow the betas to be determined then...

Example activation for a right branch tree the same as above but summing across all cells. Moreover introducing groupings of populations.

Explain patterns in phrases vs list of words for right branched trees for Simpcomp.

Preparation of data for Bold-fMRI. Example plot of hemodynamics on same plot as above, Overlapped to emphasize difference in time scales of responses.

Time series correlations and convolution analysis (asking for ridge later on)