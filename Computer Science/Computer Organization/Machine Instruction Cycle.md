Computer programs are stored in the [[Computer Hardware|primary memory]] as a series of instructions in machine code. For these instructions to be executed alongside any necessary data, the following cycle is employed

#### Fetch
The [[CU]] sends an appropriate address through the *Memory (Address) Bus* to [[Computer Hardware|primary memory]]. The instruction that resides in the specific address is then copied into the *Data Bus* and sent to the [[MDR]]

#### Decode
The received instructions are decoded, a process which allows the [[CPU]] to become aware of any additional data that are necessary for the execution of instructions. The addresses of the required data are placed into the *Memory (Address) Bus* and the corresponding data are received by the [[MDR]] via the *Data Bus*

#### Execute
The [[CPU]], mainly with the [[ALU]], executes the instruction using the necessary data that have been loaded and calculates a result. Any additional data that might be required is once again [[#Fetch|fetched]] 

#### Store
After executing and computing, the [[CPU]] stores the result in [[Computer Hardware|primary memory]]. The [[MAR]] contains addresses where the result will be stored. The addresses and corresponding result are sent via the *Memory (Address)* and *Data* buses, respectively

