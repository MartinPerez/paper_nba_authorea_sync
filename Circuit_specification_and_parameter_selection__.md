### Circuit specification and parameter selection

Diagram of actual circuit with parameters
Code available in Github...

Neuron model parameters... taken from MIIND?
Parameters used in the study
by Omurtag et al. (2000). The membrane
potentials are rescaled relative to the
threshold potential, and therefore
dimensionless

Here τ is the membrane time constant, V rev the reversal potential, I e
an externally applied current, and R m the membrane resistance. The
model is completed by a threshold potential V th . If the membrane
potential approaches V th from below, the membrane potential is
instantaneously reset to V reset . Sometimes a refractive period τ re f is
introduced, during which the neuron is inactive. After this period,
the mebrane potential will V reset .

A population density is defined on a grid. It needs a minimum
and a maximum potential and a number of bins. The maximum po-
tential is naturally defined by the threshold potential. The minimum
must be chosen so as to cover the density throughout the simulation;
for the current simulation V min = 0 would be sufficient, we chose it
slightly smaller (V min = − 0.02). We use 500 bins.


Firing rates. \cite{Roxin_2011}. Most neurons in the circuit silent, (look for study) but close to fire stimulated by baseline to accept to be driven by coming activity without excessive oscillatory behavior.... In general a very strong oscillatory behavior will be triggered if populations are activated disproportionately with respect to their initial level of activity... fluctuation driven regime around 5hz, so we move WM a bit above this level for its sustained activity and keep the circuit under reasonable levels of activity. Although this is a complex topic that requires study and tuning out of the scope of this work, in any case we only like at the qualitative behavior. We can also inform firing rates from the review of neural activity during decision making \cite{Wohrer_2013}. There is even different firing rate between layers, in some as reported by Kerr\cite{Kerr_2005} less than 0.1 Hz. Attention to the fact that distributions of spontaneous and evoked firing rate are highly similar

Synaptic efficacy. Where we get the 0.03 from? As exposed by London\cite{London_2002}, current understanding of synapsis is limited and even contextual measurements of efficacy might be more appropriate to understand the impact of synapcic input on spike output that actual set parameters of the synapse. Moreover recent evidence \cite{Briggs_2013} even shows that synaptic efficacy might be modulated by attention processes and is naive to consider it as a fixed parameter in a circuit. We decide to leave this parameter fixed and homogeneous across the circuit under the lack of appropriate hypothesis to tinker it. From Briggs paper it seems that synchronous firing of an input has probabilities between 3.1 and 7.6 while single firing from 28 to 36.

Connectivity is another topic to take carefully. Connection distribution can have an impact in spike based communication\cite{Teramae_2012}, here we are simply considering homogenous connections.

Duration of WM and Ctl can be anything...
slope of activation increase in WM of 0.01 and in Ctl of 0.01. At the end is the same thing with variable duration...

Circuit baseline of activation given by fixed 1 Hz rate with connectivity of (16, 0.36) and slope... its another delay assembly...