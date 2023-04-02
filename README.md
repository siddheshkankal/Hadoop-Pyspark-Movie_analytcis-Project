<h1 align="center">Hi 👋, I'm Siddhesh Kankal</h1>
<h3 align="center">A passionate data engineer</h3>

- 🔭 I’m currently working on [Movie analytics Project](https://github.com/siddheshkankal/Hadoop-Pyspark-Movie_analytcis-Project)

- 👨‍💻 All of my projects are available at [https://github.com/siddheshkankal](https://github.com/siddheshkankal)

- 📝 I regularly write articles on [Data engineering tech stack](Data engineering tech stack)

- 📫 How to reach me **dksidd96@gmail.com**

<h3 align="left">Connect with me:</h3>
<p align="left">
<a href="https://linkedin.com/in/https://www.linkedin.com/in/siddhesh-kankal-bhavsar-20101996" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="https://www.linkedin.com/in/siddhesh-kankal-bhavsar-20101996" height="30" width="40" /></a>
</p>

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://www.docker.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original-wordmark.svg" alt="docker" width="40" height="40"/> </a> <a href="https://hadoop.apache.org/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/apache_hadoop/apache_hadoop-icon.svg" alt="hadoop" width="40" height="40"/> </a> <a href="https://hive.apache.org/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/apache_hive/apache_hive-icon.svg" alt="hive" width="40" height="40"/> </a> <a href="https://pandas.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/2ae2a900d2f041da66e950e4d48052658d850630/icons/pandas/pandas-original.svg" alt="pandas" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> </p>

## Table of contents
* [General info](#general-info)
* [Technologies](#technologies)
* [Architecture](#Architecture)
* [Setup](#setup)

## General info
This project is about Movie Analytics.
	
## Technologies
Project is created with:
* Hadoop
* Hive
* Spark
* Python
	
## Architecture

![image](https://user-images.githubusercontent.com/118110193/229354513-19a21c27-4482-4c5e-bc53-3d3f297f45e8.png)


Detailed Explanation: For this project there are 3 data sources named as ratings.csv,users.csv,movies.csv. In the ratings.csv there are 4 columns userid , movieid , rating, timestamp. The userid gives the detail about the user,the movieid gives the information of the movie to which user gave rating. The rating will be in between 1 to 5. In the users.csv we have 4 columns userid,gender,occupation,zip-code.The userid gives information about the user.the gender gives information regarding the gender of the user and the occupation gives the info regarding occupation of the user and zipcode gives the information about the zipcode of the user. In the movies.csv we have 3 columns. we have information regarding movieid,title genre.the moviid gives the id of the movie,the title represents the title for the movieand genre gives the information regarding to which genre it belongs to this columnis again delimted by ‘|’.it has various values in that column like action, Thriller etc.

Our data is picked from the hdfs layer and read by the spark engine. After reading the data We can perform various analytical queries on the data and extract useful business insights like top 10 viewed movies,distinct list of genres,to which genre audience are giving more ratings etc.So that the movie industry can analyze the trends and can know the audience interests. Storage: Finally we can store the data as table in hive meatstore if required we can also create real time dashboards by using some dashboarding tools.

## Setup
To run this project, install it locally:
first copy all files from local to HDFS location

```
$ hdfs dfs -put users.csv /
$ hdfs dfs -put movies.csv /
$ hdfs dfs -put ratings.csv /
```
Then on the Spark shell run the below command from CLI
```
$ Python main.py
or
$ spark-submit main.py
```
