An important current issue in linguistic composition is to assess the biological neural circuitry that could be responsible for its dynamics and the associated syntactic representations. The simplicity of the SimpComp trials, that can be hypothesized as size increasing right branched trees under phrase structure grammars for both noun and verb phrases, give us the opportunity to evaluate simple predictions.

One promising approach is the blackboard architecture circuits detailed by Van der Velde and De Kamps\cite{van_der_Velde_2006}. As explained by the authors, the architecture deals simultaneously with several important issues raised by Jackendoff to model neural language processes\cite{Jackendoff_2002}. Moreover there are already implementations of the blackboard circuits that approximate biological reality with Wilson Cowan population dynamics. Some of the simulations attempt to address diverse aspects of language processing like ambiguity\cite{velde2015ambiguity}, while others address circuit related issues like tuning the syntactic control mechanisms\cite{van_der_Velde_2010}. Nonetheless previous simulations were not evaluated directly against neuroimaging measurements, but provided qualitative comparisons between the simulation results and the cognitive and neuroimaging literature. To our knowledge this work is the first attempt to test a blackboard circuit prediction directly in neuroimaging data.

Here we implement blackboard circuits partially. We implement only the necessary parts to model the neural activity related to building the representation of the sentence structure. This means that we simplify two important aspects of the circuit for which we can not test empirically the circuit structure. The first is that we will provide the signals of control directly to the circuit to derive the activity related to sentence processing in the blackboard. Previous attempts to train the control mechanism\cite{van_der_Velde_2010} were tailored only to specific grammatical cases and creating a general control mechanism to test the neural activity patterns would require a more varied dataset in grammatical categories and computational linguistic efforts out of the scope of this work. The second is that we do not model the dynamic inhibition of competing blackboard cells since this would require hypothesis about the size of the blackboard, which would be related to memory limitations and the total number of possible grammatical categories to link in binary trees which again would require out of scope computational linguistic research. Moreover the simplest selection mechanism behind competing blackboard cells can be hypothesized to be at random.

This means that we are only testing predictions based on average neural activity time series of blackboard cell neural population categories. These time series should allow us to differentiate different syntactic tree morphologies and sizes. In the case of Bold-fMRI differences in the activity attributed to syntactic trees of similar shape but with different grammatical category nodes could give us some insights in the spatial distribution of blackboard circuits. Nonetheless the first test to be passed is if the modeled circuit can adequately account for effect patterns on tree size, otherwise any apparent spatial distributions difference could easily be attributed to diverse sources of noise in Bold-Fmri.