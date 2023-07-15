```python
daniel_ubuntu@daniel:~$ pyspark
Python 3.10.6 (main, May 29 2023, 11:10:38) [GCC 11.3.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
23/07/06 20:31:56 WARN Utils: Your hostname, daniel resolves to a loopback address: 127.0.1.1; using 172.28.48.115 instead (on interface eth0)
23/07/06 20:31:56 WARN Utils: Set SPARK_LOCAL_IP if you need to bind to another address
Setting default log level to "WARN".
To adjust logging level use sc.setLogLevel(newLevel). For SparkR, use setLogLevel(newLevel).
23/07/06 20:31:58 WARN NativeCodeLoader: Unable to load native-hadoop library for your platform... using builtin-java classes where applicable
Welcome to
      ____              __
     / __/__  ___ _____/ /__
    _\ \/ _ \/ _ `/ __/  '_/
   /__ / .__/\_,_/_/ /_/\_\   version 3.4.1
      /_/

Using Python version 3.10.6 (main, May 29 2023 11:10:38)
Spark context Web UI available at http://172.28.48.115:4040
Spark context available as 'sc' (master = local[*], app id = local-1688686319204).
SparkSession available as 'spark'.
>>> df=spark.read.format("com.databricks.spark.csv")\
...    .option("header","true")\
...    .option("delimiter", "\t")\
...    .option("inferSchema", "true")\
...    .load("WorldEnergyOverview.csv")
>>>







```
