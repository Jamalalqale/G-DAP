# G-DAP (Global Domain Analysis Project)

This involves retrieving the top 1000 domains from each country and extracting their historical URLs. By segmenting and analyzing these URLs, we identify the most frequent segments as well as the top keys and values of the GET method per country. This analysis provides insights into web content structure and trends, enhancing cybersecurity by detecting common patterns and potential vulnerabilities. So far, the published countries are France and Italy.

## Top segments

WE identify the most 1000 frequent segmnres per country. we have cleanded each urls from Get paramerters before. 

![alt text](https://github.com/Jamalalqale/G-DAP/blob/main/Report/FranceTopSegments.png?raw=true)


![alt text](https://github.com/Jamalalqale/G-DAP/blob/main/Report/ItalyTopSegments.png?raw=true)



## Top Keys

We extract GET parameters (keys and values) from the URLs and identify the 1000 most frequent keys for each country. Then, we determine the top frequent value for each key. For example, in the France-Top_1000-Keys list, the 'language' key ranks 5th, appearing 6,755,432 times, with 'en' being its most frequent value, paired 337,244 times with the key, accounting for 4.9% of all values for this key. The remaining percentages are distributed among various other values. Sometimes, the most frequent value for a key is empty; this is not an error, as it has been verified. For instance, in the France-Top_1000-Keys list, the most frequent value for the 'url' key is null/empty.

![alt text](https://github.com/Jamalalqale/G-DAP/blob/main/Report/FranceTopKeyReport.png?raw=true)


![alt text](https://github.com/Jamalalqale/G-DAP/blob/main/Report/ItalyTopKeyReport.png?raw=true)


## Top Values

We extract GET parameters (keys and values) from the URLs and identify the 1000 most frequent values for each country. Then, we determine the top frequent key for each value. For example, in the Italy-Top_1000-Values list, the 'crop' value ranks 8th, appearing 3,485,752 times, with 'fit' being its most frequent key, paired 3,054,793 times with the value, accounting for 87.6% of all keys for this value.

## Tools used
We use the Waybackurls tool to collect the historical URLs of each domain, producing tens of gigabytes of data per country. Then, we utilize PySpark (Python API for Apache Spark) for cleaning, processing, and analyzing the big data. Additionally, we use Microsoft Power BI for data visualization