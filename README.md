# pyParkinsons

pyParkinsons is a project used for finding early detections of Parkinsons disease using machine learning librairies [pandas](https://pandas.pydata.org/) and [XGBoost](https://xgboost.readthedocs.io/en/latest/)

## Requirements

This repository has included a requirements.txt file for all the required dependencies.
A virtual environment is also reccomended for all python projects, but it is optional.

Virtual python environment installation using [pip](https://pip.pypa.io/en/stable/)

```bash
pip install virtualenv
```

Dependency librairies installation using [pip](https://pip.pypa.io/en/stable/)

```bash
pip install numpy pandas sklearn xgboost
```

## Usage

This program can be used with a different .data file, as the data filed included is just an example. I used the [UCI Parkinsons Data Set](https://archive.ics.uci.edu/ml/datasets/parkinsons) to train the algorithim. To have the program work correctly, the .data file needs to be structured in columns with 

* name - ASCII subject name and recording number
* MDVP:Fo(Hz) - Average vocal fundamental frequency
* MDVP:Fhi(Hz) - Maximum vocal fundamental frequency
* MDVP:Flo(Hz) - Minimum vocal fundamental frequency
* MDVP:Jitter(%),MDVP:Jitter(Abs),MDVP:RAP,MDVP:PPQ,Jitter:DDP - Several measures of variation in fundamental frequency
* MDVP:Shimmer,MDVP:Shimmer(dB),Shimmer:APQ3,Shimmer:APQ5,MDVP:APQ,* Shimmer:DDA - Several measures of variation in amplitude
* NHR,HNR - Two measures of ratio of noise to tonal components in the voice
* status - Health status of the subject (one) - Parkinson's, (zero) - healthy
* RPDE,D2 - Two nonlinear dynamical complexity measures
* DFA - Signal fractal scaling exponent
* spread1,spread2,PPE - Three nonlinear measures of fundamental frequency variation

## Contributions

Pull requests are welcome, major changes should be taken up with an issue to first discuss what you would like to change

## License

[MIT](https://choosealicense.com/licenses/mit/)
