# ApacheSpark

클러스터 mesos를 사용하기로 함

(http://hoondongkim.blogspot.kr/2015/10/spark-yarn-cluster-vs-spark-mesos.html)

Spark Stand Alone (X) : 단일job빠름 but, 멀티job X

Spark Yarn Cluster (X) : biz연산(cpu/mem)보다 raw(disk,network)한 대량처리 작업은 빠름. hdfs 특징이 잘 드러남

Spark Mesos Cluster (O) : biz연산(cpu/mem)은 yarn 보다 2배 이상 빠름. 


2018/01/23 현재 버전

Spark 2.2.1 (17년 12월 릴리즈)

Mesos 1.4.1

mesos는 mesosphere로 설치함




















