# k-means-clustering
import pandas as pd 
import numpy as np 
from sklearn.cluster import KMeans
from sklearn import datasets
iris=datasets.load_iris()
iris
iris.data
iris.feature_names
X=pd.DataFrame(iris.data)
X.columns=['sepal length',
 'sepal width ',
 'petal length ',
 'petal width ']
 X
 Y=columns=['Targets']
Y
model=KMeans(n_clusters=3)
model.fit(X)
import matplotlib.pyplot as plt 
import seaborn as sns
plt.scatter('X.petal_length','X.petal_width')
colormap=np.array(['red','green','yellow'])
