### Compartment circuit specification

Previous simulations of the blackboard approximate the mean activity of neural assemblies with Wilson Cowan dynamics \cite{Frank_2014} \cite{de2015combinatorial}. Nonetheless direct simulations of LIF neurons have faster transient behavior than the pseudo dynamics described by the Wilson Cowan equations, which only allow to approximate correctly the steady state of neural populations by suggesting what firing rates should be after certain period of time, as explained by De Kamps \cite{de_Kamps_2008}. 

We consider that given the quick nature of sentence parsing and 

with population density methods and restrict ourselves only for the simulation of the mechanisms responsible for the representation of a composed structure. The latest simulations use Cowan  and \cite{de2015combinatorial},, arguments against Cowan in stat\cite{de_Kamps_2008}... then we simulate LIF and take advange of population density techniques developed by De Kamps\cite{de2013generic} and implemented in the software MIIND\cite{de_Kamps_2008}\cite{harrison2011new}...

LIF populations. As a first approach, although conductance models are desirable and should eventually be implemented under population density methods as mentioned in \cite{de2013generic}

Simplify modeling of WM as a delay circuit instead of modeling it explicitly with neural populations. This is done as a first approximation but should be replaced for an actual circuit. Nonetheless there are many ways to implement the same qualitative behavior, not sure how to justify this...

We do not consider SAs as reverberating neural populations like is the case of WM, since the way we consider control activation makes it unnecessary. Contrary to our argmunets on \cite{velde2015ambiguity}. We model MA separately from a WM that leads its activation.

Diagram of actual circuit with parameters

### Parameter selection

Firing rates. \cite{Roxin_2011}. Most neurons in the circuit silent, (look for study) but close to fire stimulated by baseline to accept to be driven by coming activity without excessive oscillatory behavior.... In general a very strong oscillatory behavior will be triggered if populations are activated disproportionately with respect to their initial level of activity... fluctuation driven regime around 5hz, so we move WM a bit above this level for its sustained activity and keep the circuit under reasonable levels of activity. Although this is a complex topic that requires study and tuning out of the scope of this work, in any case we only like at the qualitative behavior. We can also inform firing rates from the review of neural activity during decision making \cite{Wohrer_2013}. There is even different firing rate between layers, in some as reported by Kerr\cite{Kerr_2005} less than 0.1 Hz. Attention to the fact that distributions of spontaneous and evoked firing rate are highly similar

Synaptic efficacy. Where we get the 0.03 from? As exposed by London\cite{London_2002}, current understanding of synapsis is limited and even contextual measurements of efficacy might be more appropriate to understand the impact of synapcic input on spike output that actual set parameters of the synapse. Moreover recent evidence \cite{Briggs_2013} even shows that synaptic efficacy might be modulated by attention processes and is naive to consider it as a fixed parameter in a circuit. We decide to leave this parameter fixed and homogeneous across the circuit under the lack of appropriate hypothesis to tinker it. From Briggs paper it seems that synchronous firing of an input has probabilities between 3.1 and 7.6 while single firing from 28 to 36.

Connectivity is another topic to take carefully. Connection distribution can have an impact in spike based communication\cite{Teramae_2012}, here we are simply considering homogenous connections.

### Circuit dynamics

We mantain a rate of activity transmission with the number of connections. Our simple approach ignore the intrincacies found in different regimes to transmit information in enural networks, where some regimes might allow rich internal computations. \cite{Ostojic_2014}. We simply focus on passing forward mean activity to be able to instantiate binding with WM activation.

issues encountered on oscillatory behavior, accounted by near threshold firing with baseline activity and smoothing rate activity increase

Control noise resilience can be shown in case controls get activated, baseline levels do not activate WM.

two MA activity necessary for WM activated. Otherwise it does not activate. Can show plot.

MA active creates elevated levels of activity in SA that would facilitate information flow and WM further prolonged activity.

To improve the future circuit implementation more realistic rest state of the network could have been achieved by balanced networks\cite{Wolf_2014}. This is a future expansion too. Also it might be desirable to move to more realistic network models like conductance? and implement dynamic synaptic efficacy enhancement during processing?

CONNECTIVITY PARAMETER SELECTION, DYNAMICS AND ISSUES CAN BE TURNED INTO THE STUDY THE BLACKBOARD CIRCUIT STATE SPACE WITH THE HELP OF MARC.

Balckboard code provided in github....

Plot of activation example for all time series. Legend for selected time series. And Plot of total activation of compartment circuit.

Selection of compartment circuit dynamics to facilitate simulation of complete blackboard based on key points... show in plot selected intervals that can be filled up by a stable state for the remaining time, such that the complete blackboard time series are implemented in python. Python code provided in github...

### Complete sentence processing simulation

Example activation for a right branch tree the same as above but summing across all cells. Moreover introducing groupings of populations.

Preparation of data for Bold-fMRI. Example plot of hemodynamics on same plot as above, Overlapped to emphasize difference in time scales of responses.

Time series correlations and convolution analysis (asking for ridge later on)