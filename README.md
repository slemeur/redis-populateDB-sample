# redis-populateDB-sample

This repository provides a basic sample code that can help you populate a Redis Database with dummy data.

## Pre-requisites

- Have Jave installed
- Have Maven installed
- Have an IDE (simplest would be VSCode)
- Have a Redis database running

## Steps

### 0 Open a terminal

### 1 Clone the repository

```
git clone https://github.com/slemeur/redis-populateDB-sample.git
```

### 2 Open the project in your IDE

Open a If you are using VSCode:
```
username> code .
```

When opening VSCode, it will ask if you want to install Java tooling (if you don't have it already), install it.

### 3 Make sure to connect your database

Open the file `PopulateSample001.java` in the folder `/redis-populateDB-sample/src/main/java/io/redis/populate/`

Go to the line 15
```
JedisPool jedispool = new JedisPool(new JedisPoolConfig(), "localhost", 6379);
```

This is where you can configure the information about your database. In this case, the database is running locally and using port 6379.

### 4 Run the script

Still in the file  `PopulateSample001.java` in the folder `/redis-populateDB-sample/src/main/java/io/redis/populate/`

Go line 13. You should see in the editor, inline buttons to `Run | Debug`. Hit the `Run` button.

If you don't, make sure to install the Java tooling for VSCode.

### 5 Check in RedisInsight the added data


