Memory Data/Buffer Register (MDR), a register contained within the [[CU]], holds the **data** that is to be used by the [[ALU]] and then saved to the [[RAM]].

> [!Tip] MDR vs [[MAR]]
Whichever memory address location the [[MAR]] is holding, the corresponding content will be loaded onto the MDR for processing. 

After the processing has taken place, the [[CU]] places the result from the [[ALU]] onto the MDR and the data is coped to the memory address location in [[RAM]] specified by the [[MAR]] via the *Data Bus*

In order for the MDR to communicate with [[Computer Hardware|primary memory]], a connection via *the Data Bus* is necessary.
