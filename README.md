# Computational-neuroscience-project

In this project we modeled an artificial neural network to implement the neurorobotics experiment. 
The following are the steps to be performed to correctly setup the enviroment.

1) Access the neurorobotic platform and create a new experiment selecting the template 'Empty World Enviroment'. When creating the enviroment, change from
   PyNN-NEST to NEST. Do not change any setting of the enviroment.
2) Open the 'object library' tab and place the iCub robot at the following coordinates: (x, y, x) = (2, 0, 0.622). Do not change the rotation parameters.
3) Open the 'State machine' tab and copy and paste the 'StateMachine_final' code (only the part you need to model the input, either red, blue or both). 
   Then click verify and close the tab. If an error occurs, close the enviroment and rerun the experiment.
4) Open the 'Brain' tab and copy and paste the 'Brain_final' code. Then click verify and close the tab. If an error occurs, close the enviroment and
   rerun the experiment. Once this has been done, click on [+] to add new populations, respectively (with the EXACT same name as below):
   - recorders: from 0 to 100 with step 1
   - sensors: from 0 to 5 with step 1
   - actuators: from 4 to 84 with step 1 (PopA will be from neuron 4 to 43, PopB from neuron 44 to 83)
5) Open the 'Transfer functions' tab, click [+] and copy and paste the transfer functions in the 'TransferFunctions_final' code, respectively:
   - ##################### Spike recorder
   - #################### iCub eye detection(new)
   - ################### iCube head motion
   Each transfer function must be added separately clicking [+] every time to add a new one, from ############ to # in the code. Then click verify all. If an error occurs, 
   close the enviroment and rerun the experiment.
6) Open the 'Spike train' tab to monitor neuronal spiking, press play and enjoy the decision-making experiment.

(This project is the result of teamwork)
