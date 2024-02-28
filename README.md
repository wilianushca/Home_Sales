# Home_Sales

# Home Sales Analysis with Apache Spark

This project analyzes home sales data using Apache Spark. The dataset contains information about home sales, including prices, number of bedrooms and bathrooms, square footage, and other attributes.

## Installation

To run this project, you need Apache Spark installed. You can download Apache Spark from the (http://www.apache.org/dist/spark/) website and set up the environments following the instructions provided. Such as...

```python
spark_version = 'spark-3.5.1'
```

```bash
!apt-get update
!apt-get install openjdk-11-jdk-headless -qq > /dev/null
!wget -q http://www.apache.org/dist/spark/$SPARK_VERSION/$SPARK_VERSION-bin-hadoop3.tgz
!tar xf $SPARK_VERSION-bin-hadoop3.tgz
```

```bash
!pip install -q findspark
```

```python
import os

os.environ["JAVA_HOME"] = "/usr/lib/jvm/java-11-openjdk-amd64"
os.environ["SPARK_HOME"] = f"/content/{spark_version}-bin-hadoop3"
```

```python
import findspark
findspark.init()
```

Make sure you have Python installed on your system. This project requires the PySpark library 

## Usage

1. Clone the repository to your local machine.
2. Install Apache Spark and Python if you haven't already.
3. Set up the environment variables such as `SPARK_HOME` and `JAVA_HOME`.
