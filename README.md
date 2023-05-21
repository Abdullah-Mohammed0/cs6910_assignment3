# CS6700 - Fundamentals of Deep Learning
## Assignment 3

### Instructions for executing the program:

The code for the model is contained in the Python notebook **A3.ipynb**. 

The initial cells contain the code as developed during the coding phase.

The code for each question is separately contained in the final cells of the notebook. Each question is coded as a function, and the calls to all functions corresponding to the questions have been commented out. To execute a particular question, uncomment the corresponding function call and execute the cell.

**Note:** Ensure that the cells are executed in the order presented in the notebook. Not doing so may result in incorrect results and/or errors.

The trained encoder and decoder for the vanilla and attention-based models have been stored in the folders **vanilla_model** and **attention_model** respecively. The functions Q4() and Q5() in the notebook contain the code used to generate them as well as the corresponding outputs, which are stored in the folders **prediction_vanilla** and **predictions_attention** respectively,

### Instructions to install font for Manipuri:

Since the models have been trained to achieve transliteration from English to Manipuri, the font associated with Manipuri has also been provided in this repository as **NotoSansMeeteiMayek-Regular.ttf**. This font needs to be installed in the system to view the cell outputs. 

On Linux, this installation can be done simply by opening the associated file and clicking on 'Install'. 

Furthermore, to view the Manipuri letters in the attention heatmaps, the same file needs to be copied to /home/<user_name>/.local/lib/<python_version>/site-packages/matplotlib/mpl-data/fonts/ttf, where <user_name> is replaced with the user name in the system, and <python_version> is replaced with the appropriate version of Python used in the system.


