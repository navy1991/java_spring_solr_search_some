# java_spring_solr_search_some

Sample implementation of Java + Spring Boot + Apache Solr for study.

# Architecture

- Sprint Boot
- PostgreSQL
- Solr Cloud (Cluster)
    - solr1
    - solr2
- ZooKeeper

# Get Started


```
docker compose up
```
```
docker exec solr1 bin/solr create_collection -c gettingstarted -shards 2 -replicationFactor 1 --solr-url http://localhost:8983/solr -z zoo:2181
```

open each admin ui

- http://localhost:8983/solr/#/
- http://localhost:8984/solr/#/

# References

- Solr
    - https://solr.apache.org/guide/solr/latest/index.html
    - https://solr.apache.org/guide/solr/latest/deployment-guide/solr-in-docker.html