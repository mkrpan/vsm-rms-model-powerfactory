# Virtual Synchronous Machine model for RMS simulations in DIgSILENT PowerFactory

This is the repository for PowerFactory RMS models of a VSM, as a supplement to the manuscript titled: _Modelling and Initialization of a Virtual Synchronous Machine for Power System Fundamental Frequency Simulations_

The model has been natively developed in DIgSILENT PowerFactory version v2019 SP4 and can be found in the file `VSM-v2019.pfd`. The model has also been exported to PF versions 2018 and 2017 (`VSM-v2018.pfd` and `VSM-v2017.pfd`, respectively), however there is some loss of data so it cannot be guaranteed that the model work correctly or at all. DC link is considered stiff and there are no associated DC link dynamics.

The model is intended for fundamental frequency (RMS) simulations. The 50 Hz 690 V grid consists of: 
- a static generator with VSM control
- an LC filter
- a line (X/R >> 1)
- loads
- a synchronous generator with _IEEE TGOV1_ turbine governor and _IEEET1_ excitation system.

There are four simulation events in the model: step change of active power set-point, step change of reactive power set-point, step change of internal voltage set-point and step change of load power.

Main developer of the model is Bojana Barać, with support and supervision by Matej Krpan, Tomislav Capuder and Igor Kuzle. Contact info of the authors can be found in the aforementioned paper.

If you find this work helpful, please give credit to: B. Barać, M. Krpan, T. Capuder, I. Kuzle, "Modelling and Initialization of a Virtual Synchronous Machine for Power System Fundamental Frequency Simulations," preprint: 10.13140/RG.2.2.30876.21126, 2021.

The preprint version of this paper is available online: https://www.researchgate.net/publication/352478576_Modelling_and_Initialization_of_a_Virtual_Synchronous_Machine_for_Power_System_Fundamental_Frequency_Simulations

_**2020-09-29: Two new models have been added: battery energy storage system operated as a VSM (includes DC link dynamics and battery dynamics) and a rooftop PV plant operated as a DCVQ VSM (includes PV plant dynamics and DC link dynamics). Both have been created in PowerFactory v2019.**_
