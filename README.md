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

open each `Solr Admin UI`

- http://localhost:8983/solr/#/
- http://localhost:8984/solr/#/

# References

- Solr
    - https://solr.apache.org/guide/solr/latest/index.html
    - https://solr.apache.org/guide/solr/latest/deployment-guide/solr-in-docker.html
- CheckStyle
  - https://checkstyle.sourceforge.io/index.html
  - https://github.com/nablarch-development-standards/nablarch-style-guide/blob/master/java/staticanalysis/checkstyle/docs/Checkstyle-commentary.md
- SpotBugs
  - https://spotbugs.github.io/
  - https://spotbugs.readthedocs.io/ja/latest/
  - https://github.com/spotbugs/spotbugs-gradle-plugin
- Sentry
  - https://sentry.io/welcome/
  - https://docs.sentry.io/platforms/java/guides/spring-boot/