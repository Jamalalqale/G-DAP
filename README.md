# G-DAP

This is conducted by retrieving the top 1000 domains from each country and extracting their historical URLs. By segmenting and analyzing these URLs, we are identifying the top 1000 most frequent segments per country. This analysis offers insights into web content structure and trends, enhancing cybersecurity by detecting common patterns and potential vulnerabilities.


## Tools used
We are using Waybackurls tool to collect the historical URLs of each domain which produces tens of Gigabytes of data per country. Then we utilizes Pyspark (Python API for Apache Spark)for cleaning, processing and analyzing the big data we have.