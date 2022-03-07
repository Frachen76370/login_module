import pandas as pd
import numpy as np

import matplotlib.pyplot as plt
df=pd.read_csv("dataset.csv",engine="python")


def movie_name():
    a=str(input("ENTER MOVIE NAME TO FIND IT'S RELEASE DATE"))
    details=df[df['title']==a]
    for i in details['release date']:
        print(i)


def movie_country():
    b=str(input("ENTER MOVIE NAME TO FIND IT'S COUNTRY OF ORIGIN"))
    details=df[df['title']==b]
    for i in details['country']:
        print(i)

def movie_ratings():
    c=str(input("ENTER MOVIE NAME TO FIND IT'S RATINGS"))
    details=df[df['title']==c]
    for i in details['ratings']:
        print(i)


def movie_duration():
    d=str(input("ENTER MOVIE NAME TO FIND IT'S DURATION IN MINUTES"))
    details=df[df['title']==d]
    for i in details['duration(min)']:
        print(i,'min')


