# TCHotTakes_Template
Some starter code for the Tech Connect "Hot Takes" Challenge. To view the sample project, look at [mine](https://github.com/agindi/TCHotTakes_SampleProject).

This template uses Python, so if you'd like to use it please install a recent version of Python - the below instructions are for Windows but feel free to scour the internet for analygous instructions on your system. Also, if you'd like to use Jupyter Notebook, the process may be simpler, but it's also fun to get down in the weeds, and if you're new to Python I suggest following the steps below.

## Getting started
Download this starter code into your directory of choice. Then, open up the command prompt, navigate to your directory, and issue the command `python --version` to ensure that Python is properly installed.

## Setting up your Virtual Environment
This step is not strictly necessary, but it will help to isolate your project's dependencies. For more information about Virtual Enviroments, google it. But if you're incurious and just want to get the job done, run the command `python -m venv .venv`, which will create a new, fresh python interpreter in the local directory `.venv`. To activate that environment, run the command `.venv/Scripts/activate`. Reminder - this is for Windows, you may need a different command on your own system. You will know that the activation command worked if your command line is prepended by **(.venv)**

## Getting the Dependencies
First, to ensure that your virtual environment is running well, I suggest you run the command `python -m pip list`. It should look something like this:

```
(.venv) PS C:\dev\Projects\CodingChallenge\HotTakes> python -m pip list
Package    Version
---------- -------
pip        21.2.3
setuptools 57.4.0
WARNING: You are using pip version 21.2.3; however, version 22.1.2 is available.
```

If it tells you to upgrade pip (like mine did) run the command `python -m pip install --upgrade pip`. Now, to install the dependencies for this proeject, you'll need to run the commands:

```
python -m pip install numpy
python -m pip install pandas
python -m pip install matplotlib
```

Now, when you run the command `python -m pip list` your output should contain the following items:

```
(.venv) PS C:\dev\Projects\CodingChallenge\HotTakes> python -m pip list
Package         Version
--------------- -------
cycler          0.11.0
fonttools       4.33.3
kiwisolver      1.4.3
matplotlib      3.5.2
numpy           1.23.0
packaging       21.3
pandas          1.4.3
Pillow          9.1.1
pip             22.1.2
pyparsing       3.0.9
python-dateutil 2.8.2
pytz            2022.1
setuptools      57.4.0
six             1.16.0
```

## Running your Project
Now, running the project is simple! Run the command `python app.py` and your result should look like this:
```
(.venv) PS C:\dev\Projects\CodingChallenge\HotTakes> python app.py
    location       cohort school_year  greener  hotdog  ... ketchup  pineapple  lasagna monsters_inc  pizza_fold
0    Buffalo  2022 Intern      Senior        0       1  ...       0          0        1        Blink           1
1    Buffalo  2022 Intern      Senior        1       1  ...       0          0        1        Blink           1
2    Buffalo     2020 TDP         NaN        0       0  ...       0          1        1         Wink           0
3    Buffalo  2022 Intern      Junior        1       1  ...       0          1        1        Blink           1
4    Buffalo  2022 Intern      Senior        1       1  ...       1          0        1        Blink           0
..       ...          ...         ...      ...     ...  ...     ...        ...      ...          ...         ...
103  Buffalo     2020 TDP         NaN        0       1  ...       0          0        2        Blink           0
104  Buffalo     2021 TDP         NaN        1       0  ...       0          0        2        Blink           0
105  Buffalo     2021 TDP         NaN        1       0  ...       0          1        2         Wink           0
106  Buffalo     2021 TDP         NaN        0       0  ...       0          0        2        Blink           0
107  Buffalo     2021 TDP         NaN        1       0  ...       0          0        2        Blink           0

[108 rows x 16 columns]
```

All that's left for you to do is open up app.py and augment the main() and display_visual() functions! Happy Coding!
