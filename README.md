# ElasticSearch-Vue.js
FOR WINDOWS: 

1) In Node.js CMD PROMPT run --> npm i elasticsearch body-parser express if you do not already have these settings

2) Next, head to elastic.co and install the newest client (Current version is 6.7.0)

3) Configure a JDK environment variable by going to ---> Environment Variables... --> In System Variables hit NEW..--> then write VAR_NAME = JAVA_HOME and 
VAR_PATH = C:\Program files\Java\jdk-12 (or Whatever your current version is). 

4) Check if elastic search and env vars are properly configured by going into your current version of elasticsearch\bin and then double clicking on elasticsearch.bat.
It will lead to a JSON file that looks like this. The location and port is: localhost:9200 

{
  "name" : "TAOU2k8",
  "cluster_name" : "elasticsearch",
  "cluster_uuid" : "kjDGChQnTMqSozstcoi1qw",
  "version" : {
    "number" : "6.7.0",
    "build_flavor" : "default",
    "build_type" : "zip",
    "build_hash" : "8453f77",
    "build_date" : "2019-03-21T15:32:29.844721Z",
    "build_snapshot" : false,
    "lucene_version" : "7.7.0",
    "minimum_wire_compatibility_version" : "5.6.0",
    "minimum_index_compatibility_version" : "5.0.0"
  },
  "tagline" : "You Know, for Search"
}

5) Now in Node.js terminal or CMD PRMT cd into C:User\..\Downloads\elasticsearch-6.7.0\bin>

6) From here, you will install elastic search if you have not already. Run elasticsearch-service.bat install

7) Finally, you can restart elasticsearch quickly and easily by staying within the directory and running elasticsearch-service.bat install|remove|start|stop|manager
