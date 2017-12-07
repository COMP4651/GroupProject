![HSBC](https://powerbicdn.azureedge.net/cvt-cb6808dc8de685c328422c7fa5b16138849e38f4d5e3833593c0cb10421925c3/pictures/shared/integrations/2x/spark-on-azure@2x.png)
## COMP4651 Group Project
Please download the data file from [here](https://drive.google.com/open?id=1VsH5yNKl2ZBcvAUEhE1RlCUISnkAjZPI) and store it under __data__ folder.

DataPreparation notebook process the json file and perform data cleaning.

### Update 11.25 (Kung-hsiang, Huang)
Strongly recommend you to switch to Spark 2.2. The spark 2.2 version of DataPreparation has been complete. Should there be any problem, please do not hesitate to contact me.

Step to install anaconda and pyspark on your machine:
1. Choose your suitable [downloader](https://conda.io/miniconda.html) from miniconda's website.
2. Download and run
``` bash Mini .... .sh```.
3. Follow the instructions and type yes in the end.
4. Open up a new terminal window.
5. Type in terminal ```conda create -n py27 python=2.7 anaconda```.
6. Wait for a few minutes and everything will be ready.
7. Type ```source activate py27``` to enter the virtual environment.
8. Type ```pip install pyspark``` to install pyspark.
9. To understand how to initiate PySpark on your own machine please refer to __DataPreparation-2.2__ notebook.


Machine Learning Result: Given lyrics, predict genre.
### Logistic Regression with TF
|#Training | # Validation  | #Features     | Max Iteration      |Validation Accuracy  |
|----------| ------------- |------|-------| -----|
|   0.7    | 0.1      | 60000       |    100     | 0.819 |
|   0.7    | 0.1      | 60000       |    50     | 0.804 |
|   0.7    | 0.1      | 60000       |    10     | 0.708 |
|   0.7    | 0.1      | 30000       |    10     | 0.671 |
|   0.7    | 0.1      | 20000       |   10      | 0.636 |
|   0.7    | 0.1      | 15000       |   10      | 0.630 |
|   0.7    | 0.1      | 5000        |   10      | 0.588 |
|   0.7    | 0.1      | 2000        |   10      | 0.555 |
|   0.7    | 0.1      | 1000        |   10      | 0.554 |
|   0.7    | 0.1      | 500         |   10     | 0.542 |

Machine Learning Result: Given lyrics, predict genre.
### Logistic Regression with TF-IDF
|#Training | # Validation  | #Features     | Max Iteration      |Validation Accuracy  |
|----------| ------------- |------|-------| -----|
|   0.7    | 0.1      | 60000       |    100     | 0.809 |
|   0.7    | 0.1      | 60000       |    50     | 0.807 |
|   0.7    | 0.1      | 60000       |    10     | 0.704 |
|   0.7    | 0.1      | 30000       |    10     | 0.668 |
|   0.7    | 0.1      | 20000       |   10      | 0.642 |
|   0.7    | 0.1      | 15000       |   10      | 0.624 |
|   0.7    | 0.1      | 5000        |   10      | 0.589 |
|   0.7    | 0.1      | 2000        |   10      | 0.560 |
|   0.7    | 0.1      | 1000        |   10      | 0.549 |
|   0.7    | 0.1      | 500         |   10     | 0.531 |

### Random Forest with TF
|#Training | # Validation  | #Features    | #Trees       |Validation Accuracy  |
|----------| ------------- |-------------|----| -----|
|   0.7    | 0.1      | 100  |       30       | 0.503 |
|   0.7    | 0.1       | 1000 |       10       | 0.499 |
|   0.7    | 0.1      | 500  |       10       | 0.499 |
|   0.7    | 0.1      | 3000   |     10         | 0.496 |
|   0.7    | 0.1      | 100   |     10         | 0.496 |



### Random Forest with TF-IDF
|#Training | # Validation  | #Features    | #Trees       |Validation Accuracy  |
|----------| ------------- |-------------|----| -----|
|   0.7    | 0.1      | 3000   |     10         | 0.505 |
|   0.7    | 0.1      | 100  |       30       | 0.504 |
|   0.7    | 0.1       | 1000 |       10       | 0.502 |
|   0.7    | 0.1      | 500  |       10       | 0.508 |
|   0.7    | 0.1      | 100   |     10         | 0.508 |
