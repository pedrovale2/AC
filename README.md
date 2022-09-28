# Machine Learning - Group 37

This project was developed in FEUP's school year 2021/2022 as part of the Machine Learning's class curriculum.

#### Members:

- Daniel da Silva Gonçalves
- André Pedro de Melo Malheiro
- Pedro Miguel Novais do Vale

The Project contents are separated into multiple folders, these have the following meanings:

- `/BankData/` - Contains all the given data files for the development of the Project. **It is important that this folder remains unchanged for the PythonScript to run without any issues.**
- `/KaggleResults/` - Used to store all the results that come from RapidMiner's output process.
- `/Powerpoint/` - The Presentation Document.
- `/RapidMiner - Processes/` - All essential .rpm files used in RapidMiner for the prediction phase.

### Python Scripts

There is only one universal script in our project. The name of the file is: `Data Compiler.ipynb`. It gathers all the necessary data from `/BankData/` and does all the processing by itself. By changing a specific flag variable in the script, we can produce either the _test_ contents or the _train_ contents.

The line that must be changed is:

`isTrainData = True` (4th line of the 1st cell)

### RapidMiner Processes

All processes are pretty straightforward (though we will have to change the input of the dataset if we change from one machine to another). However, in order to run these processes, the Toolbox Extension of RapidMiner will be necessary. Without it, the scripts **cannot** run. 

The outputs from RapidMiner (that go into the `/KaggleResults/` directory), will then need to be changed by a Python Script in order to be able to submit them in Kaggle. The script is the `Adapter.ipynb` script. It takes care of everything.
