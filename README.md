# Forecast of Natural Gas Price with  Deep Learning

Hello everyone today I am going to **predict** the **Natural Gas Price** with **Deep Learning** using Time Series with **Deep Learning LST** . This project can be used to predict any times series data.

The **financial data** that we will use is  **investpy**  that is one of the most complete Python packages when it comes to financial data extraction to stop relying on public/private APIs since investpy is **free** and has **no limitations**.  Is one good of  financial data retrieval.

## Step 1. Creation of the environment

### Installation of Conda

First you need to install anaconda at this [link](https://www.anaconda.com/products/individual)

![img](assets/images/posts/Times%20Series%20with%20Deep%20Learning/1.jpg)

I will create an environment called **forecast**, but you can put the name that you like.

```
conda create -n forecast python==3.7
```

If you are running anaconda for first time, you should init conda with the shell that you want to work, in this case I choose the cmd.exe

```
conda init cmd.exe
```

and then close and open the terminal

```
conda activate forecast
```

then in your terminal type the following commands:

```
conda install ipykernel
```



```
python -m ipykernel install --user --name forecast --display-name "Python (Forecast)"
```

Then we install **Tensorflow**

```
pip install tensorflow==2.9.0
```

and **Keras**

```
pip install keras==2.9.0
```

If you will work with Forecasting projects I suggest install additional libraries:

```
pip install  statsmodels pandas matplotlib  sklearn  plotly  nbformat seaborn 
```

We need to install investpy which allows the user to download both recent and historical data from all the financial products indexed at Investing.com. 

we type

```
pip install investpy 
```

## Step 2   Download the Recent/Historical Data Retrieval

