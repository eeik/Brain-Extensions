# Brain-Extensions
A few augmentative ideas for expanding capabilities of TheBrain 🧠


## Logfile Parsing, Storage, and Visualization w/ Elastic Stack
* parse TheBrain logfiles
* output to Elasticsearch
* Kibana scripted fields to unlock insights into logfile data
* Kibana search queries to build custom dashboards atop for historical review

## Pre-requisites
* [Elasticsearch](https://www.elastic.co/downloads/elasticsearch) for storing and indexing logfile entries
* [Kibana](https://www.elastic.co/downloads/kibana) for local visualizations and search of Elasticsearch index
* [Logstash](https://www.elastic.co/downloads/logstash) for *.log file parsing and storage into Elasticsearch index

## Config and logfile parsing logic
* [Config for parsing TheBrain logfiles](https://github.com/eeik/Brain-Extensions/blob/master/BrainLogs.config)
* [Kibana scripted fields](https://github.com/eeik/Brain-Extensions/blob/master/Scripted%20Field%20Code.txt)

![Image](https://github.com/eeik/Brain-Extensions/blob/master/Core%20Dashboard.png)


## Django Inlay/Overlay App
*for interrogating and visualizing TheBrain w/ logfile historical overlay*
* R/O connection to TheBrain database for real-time state insights
* dynamically rendered Kibana search filters for historical context
    - think *rich personal history* for the ongoing *use* of TheBrain
* full capabilities of Python for
    - script integration and process automation
    - AI based review of TheBrain context/graph to pre-fetch/search suggestions
    - *example:* download image, crop to dimensions, search and extract image features, save locally (not TheBrain's DB), and visualize output in some sort of novel way

**more info on this second piece forthcoming...**
![Image](https://github.com/eeik/Brain-Extensions/blob/master/BrainConsole%20App.png)
