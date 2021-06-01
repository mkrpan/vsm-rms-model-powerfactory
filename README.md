# Virtual Synchronous Machine model for RMS simulations in DIgSILENT PowerFactory

This is the repository for PowerFactory RMS models of a VSM, as a supplement to the manuscript titled: _Modelling and Initialization of a Virtual Synchronous Machine for Power System Fundamental Frequency Simulations_

The model has been natively developed in DIgSILENT PowerFactory version v2019 SP4 and can be found in the file `VSM-v2019.pfd`. The model has also been exported to PF versions 2018 and 2017 (`VSM-v2018.pfd` and `VSM-v2017.pfd`, respectively), however there is some loss of data so it cannot be guaranteed that the model work correctly or at all. DC link is considered stiff and there are no associated DC link dynamics.

The model is intended for fundamental frequency (RMS) simulations. The 50 Hz 690 V grid consists of: 
- a static generator with VSM control
- an LC filter
- a line (X/R >> 1)
- loads
- a synchronous generator with _IEEE TGOV1_ turbine governor and _IEEET1_ excitation system.

Main developer of the model is Bojana Barać, with support and supervision by Matej Krpan, Tomislav Capuder and Igor Kuzle. Contact info of the authors can be found in the aforementioned paper.
