
버전 2018/01/24
-apache spark 2.2.1
-mesos 1.0.0 이상이면됨 여기에 추가 패치필요없음
 spark를 고려한 mesos 설치는 없으니 그냥 설치 할 것
 소스만제공하니 가져다가 빌드하고, 바이러리는 mesoshpere를 쓸 것
 
 
 
 
 
 
 따위는없음
 
 



spark 2.2.1 /w hadoop버전 다운로드
hdfs는 몇 버전?

sparck 설치 후
vi conf/spark-env.sh.
---------------------------------------------------------------------------------------
### in conf/spark-env.sh ###

# If 'hadoop' binary is on your PATH
export SPARK_DIST_CLASSPATH=$(hadoop classpath)

# With explicit path to 'hadoop' binary
export SPARK_DIST_CLASSPATH=$(/path/to/hadoop/bin/hadoop classpath)

# Passing a Hadoop configuration directory
export SPARK_DIST_CLASSPATH=$(hadoop --config /path/to/configs classpath)
---------------------------------------------------------------------------------------









# ApacheSpark

참조사이트

http://engineering.vcnc.co.kr/2015/05/data-analysis-with-spark/




클러스터 mesos를 사용하기로 함

(http://hoondongkim.blogspot.kr/2015/10/spark-yarn-cluster-vs-spark-mesos.html)

Spark Stand Alone (X) : 단일job빠름 but, 멀티job X

Spark Yarn Cluster (X) : biz연산(cpu/mem)보다 raw(disk,network)한 대량처리 작업은 빠름. hdfs 특징이 잘 드러남

Spark Mesos Cluster (O) : biz연산(cpu/mem)은 yarn 보다 2배 이상 빠름. 


2018/01/23 현재 버전

Spark 2.2.1 (17년 12월 릴리즈)

Mesos 1.4.1

mesos는 mesosphere로 설치함






















