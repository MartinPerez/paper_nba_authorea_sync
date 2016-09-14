### Dynamics of complete sentence processing

As explained in the section "Simplified approach to the blackboard architecture", since we are not modeling the mutually inhibitory link between compartment circuits in the connection matrices of the blackboard circuit, we simply need to instantiate as many compartment circuits as necessary to simulate complete sentence processing. Moreover the only thing that could diverge between the activity of different compartment circuits is the particular time moments at which their dynamics are developed, since the dynamics themselves are identical.

We can identify, in the binding activity profile, four segments of neural dynamics that are dependent on Ctl events and WM events leading to activation of MAs. Between this segments periods of steady state activity can easily be adjusted to model different parameters of sentence processing like time of word presentations and the moments at which parsing operations would take place. The neural dynamic segments are highlighted in Figure \ref{dynamic_segments}. The first segment corresponds to the first MA activation and goes from 501ms to 607ms (106ms duration). The second segment incorporates activation of the second MA followed by Ctl activation just 50ms after for a duration of 100ms, in total the dynamics range from 801ms to 1240ms (439ms duration). The third segment is related to deactivation of the first MA and goes from 1550ms to 1720ms (170ms duration). Finally the fourth segment corresponds to deactivation of the second MA followed by deactivation of the binding WM, it goes from 1850ms to 2350ms (500ms duration).

Moreover from the partial activity profile of circuit activity we can extract an additional segment representing the stop of the first MA of activity when no other dynamics took place in the circuit, that goes from 1550ms to 1650ms (100ms duration). This is useful to model the case of list of words processing, in which MAs activity would be instantiated but no binding would take place.

Once we have the neural dynamic segments of the compartment circuit, we need specification of the timing of parsing operations, the hypothesized tree structure to represent and the desired duration of WM activity. The number of compartment circuits necessary to make the simulation simply come from the tree structure. The timing of parsing operations is the time at which we expect each of the nodes of the tree structure to be translated into the WM activity of some compartment circuit. One can see in Figure \ref{sentence_example} how the hypothesized tree structure of a sentence and the timing of the activation of tree nodes is transformed into the neural activity of a blackboard.

We assume that WM activation is long enough to allow all bindings in the tree to happen as words are incorporated in blackboard. For example if words are presented every 600 ms, we assume WM is active for around 3 seconds to bind the first word to an awaited phrase node activated after a fifth word, if WM was active for say less than 2.4s then activation of the MA would cease before the other MA and Ctl populations come into play for that compartment circuit.

Control delay considered 50ms after target word for 100ms, very naive version of xxx parsing. important to have in mind that there are other parsing possibilities. Look into generalized left corner parsing of Hale.

We take activity minus baseline activity to look at differences in neural activity.

We normalize time series to look at relative and qualitative effects. Moreover to give equal weight to time series in a regression model and allow the betas to be determined then...

Example activation for a right branch tree the same as above but summing across all cells. Moreover introducing groupings of populations.

Explain patterns in phrases vs list of words for right branched trees for Simpcomp.

Preparation of data for Bold-fMRI. Example plot of hemodynamics on same plot as above, Overlapped to emphasize difference in time scales of responses.

Time series correlations and convolution analysis (asking for ridge later on)