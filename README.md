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
8. Type ```pip install py27``` to install py27.
9. To understand how to initiate PySpark on your own machine please refer to __DataPreparation-2.2__ notebook.


