# reward-analysis

This repository is meant to provide tools to analyze your deepracer reward function before it undergoes training.

# Acknowledgments

Most of this work was originally built on the work done by the [AWS deepracer community](https://deepracing.io/). Check out their repository to see additional tools they have developed
(https://github.com/aws-deepracer-community).


# Setup

To run the reward analysis you must have python installed.

In addition to python it is recommend you install [VS Code](https://code.visualstudio.com/).

Lastly, it is recommend you install [conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html).

Once you have everything installed and have restarted your computer, you run the following command (in command prompt or terminal):

    $ conda create --name <env_name> --file <the_relative_path_to_requirements_file>

    # example below

    $ conda create --name deepracer_env --file requirements.txt


Doing this will create a virtual environment called deepracer_env and download all the packages. We will be using this to run the reward_analysis.ipynb notebook.

Now in VSCode open the reward_function.ipynb file. You should be able to select the *deepracer_env* from the ones listed. 

You should be able to run the notebook. If not checkout the **Troubleshooting** section.

# Troubleshooting

### Help! I do not see *deepracer_env* environment.

Start by reloading the developer window in vs code. Press F1 or cntl+shift+p to open the vs code console and search for *"Developer: Reload Window"*. This will reset vs code without closing and opening it. Check if the *deepracer_env* environment now appears.

### Help! I get something like the below error.

    VS code needs to install jupyter notebooks in order to run this notebook.

Run the command it tell you to run in the command prompt or terminal.

### Help! Something funky is going on with the package download.

Try using python version 3.10.6 it is what I used when running the notebook. Do this by adding the python version to the end of the command:

    $ conda create --name temp_env2 --file requirements.txt python=3.10.5

### Help! This troubleshooting is not working!

Welp ¯\\\_(ツ)_/¯ just google it then if that doesn't work ask someone.