# CS6700 - Fundamentals of Deep Learning
## Assignment 1

### Instructions for training and evaluating the model:

The following command will train a neural network with the specified parameters and evaluate the model on the test set. Specify the *wandb_entity* and *wandb_project* to track the experiment in the Weights & Biases dashboard. If *wandb_entity* and *wandb_project* are not specified, the experiment will **not** be tracked.

```
python train.py --wandb_entity myname --wandb_project myprojectname
```

### Arguments supported

| Name | Default Value | Description |
| :---: | :-------------: | :----------- |
| `-wp`, `--wandb_project` | None | Project name used to track experiments in Weights & Biases dashboard |
| `-we`, `--wandb_entity` | None  | Wandb Entity used to track experiments in the Weights & Biases dashboard. |
| `-d`, `--dataset` | fashion_mnist | choices:  ["mnist", "fashion_mnist"] |
| `-e`, `--epochs` | 20 |  Number of epochs to train neural network.|
| `-b`, `--batch_size` | 64 | Batch size used to train neural network. | 
| `-l`, `--loss` | cross_entropy | choices:  ["mean_squared_error", "cross_entropy"] |
| `-o`, `--optimizer` | nadam | choices:  ["sgd", "momentum", "nag", "rmsprop", "adam", "nadam"] | 
| `-lr`, `--learning_rate` | 0.001 | Learning rate used to optimize model parameters | 
| `-m`, `--momentum` | 0.5 | Momentum used by momentum and nag optimizers. |
| `-beta`, `--beta` | 0.9 | Beta used by rmsprop optimizer | 
| `-beta1`, `--beta1` | 0.9 | Beta1 used by adam and nadam optimizers. | 
| `-beta2`, `--beta2` | 0.999 | Beta2 used by adam and nadam optimizers. |
| `-eps`, `--epsilon` | 1e-8 | Epsilon used by optimizers. |
| `-w_d`, `--weight_decay` | 0.0 | Weight decay used by optimizers. |
| `-w_i`, `--weight_init` | xavier | choices:  ["random", "Xavier"] | 
| `-nhl`, `--num_layers` | 2 | Number of hidden layers used in feedforward neural network. | 
| `-sz`, `--hidden_size` | 128 | Number of hidden neurons in a feedforward layer. |
| `-a`, `--activation` | tanh | choices:  ["identity", "sigmoid", "tanh", "ReLU"] |


**Note:** The default values for the arguments are the best performing hyperparameters for the given dataset based on the sweep results.


### Instructions for executing the program question-wise:
The code for each question is present in the notebook **A1.ipynb**. Each question is coded as a function, and the calls to all functions corresponding to the questions have been commented out. To execute a particular question, uncomment the corresponding function call and execute the cell.

**Note:** Ensure that the cells are executed in the order presented in the notebook. Not doing so may result in incorrect results and/or errors.