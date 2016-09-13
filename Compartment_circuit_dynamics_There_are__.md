### Compartment circuit dynamics

There are four possible states of the compartment circuit 
\ref{circuit_dyn}

How baseline activity affects an isolated node... How baseline activity drives the completely connected circuit...
How MA activation is driven by WM...
How letting MA activation pass through with control affects the circuit...
How the circuit behaves when both MA and controls are active...

Simplify circuit simulation by characterizing the 4 segments of activity... plot them separately and explain them...

Plot baseline activity of circuit, show how its different across the nodes.

Control noise resilience can be shown in case controls get activated, baseline levels do not activate WM. two MA activity necessary for WM activated. Otherwise it does not activate. WM active creates elevated levels of activity in SA that would facilitate information flow and WM further prolonged activity.

Plot of activation example for all time series. Legend for selected time series. And Plot of total activation of compartment circuit.


To improve the future circuit implementation more realistic rest state of the network could have been achieved by balanced networks\cite{Wolf_2014}. This is a future expansion too. Also it might be desirable to move to more realistic network models like conductance? and implement dynamic synaptic efficacy enhancement during processing?


Selection of compartment circuit dynamics to facilitate simulation of complete blackboard based on key points... show in plot selected intervals that can be filled up by a stable state for the remaining time, such that the complete blackboard time series are implemented in python. Python code provided in github...