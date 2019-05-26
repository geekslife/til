# Concepts

* [The Internals of Apache Spark](https://jaceklaskowski.gitbooks.io/mastering-apache-spark/) : Spark 의 내부 설명
* [Spark Under the Hood: Partition](https://medium.com/@thejasbabu/spark-under-the-hood-partition-d386aaaa26b7) : 파티션의 개념 이해
  * 파티션은 RDD 가 처리하는 데이터를 논리적으로 분할한 단위
  * Spark Executor 는 Partition 데이터로 Task 를 수행한다.
