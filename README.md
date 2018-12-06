# PatternEx domain feed

![Domain detection initiative](figures/dd_logo.jpg)

We provide a list of malicious domains identified with one of the AI models developed at [PatternEx](https://www.patternex.com). The list is updated on a regular basis and reports malicious domains weeks before they are flagged on any other blacklist. The feed is released as a set of csv files, each with a maximum of 100K domains, where each line contains:
- the detection date (yyyy-mm-dd)
- the reported domain (for instance windowdowngradegreataflash[.]icu) 
- the category (currently we are reporting social engineering domains)
- the score (probability of the domain being malicious)

Below we show a sample of domains detected on 2018-11-14:

```
detection_date,domain,category,score
2018-11-14,topgreatdowngradeaflash[.]icu,social engineering,1.0
2018-11-14,upgradedowngradegreataflash[.]icu,social engineering,1.0
2018-11-14,upgradegreatdowngradeaflash[.]icu,social engineering,1.0
2018-11-14,windowdealdowngradeaflash[.]icu,social engineering,1.0
2018-11-14,windowdowngradegreataflash[.]icu,social engineering,0.9993
```

## How to use the feed? 
The feed is available for non-commercial use and without warranty; it may be used for any activity ranging from AI/ML learning, threat hunting, or live detection. We encourage users to check whether the correlation of the PatternEx feed with the network traffic logs of their organization results in malicious findings missed by existing organizational security defenses. We would love to hear your success (or failure) stories! 

## Initial stats of the feed: 
As of the day of the writing this document (2018-11-14), the feed contains 197.6K malicious domains. These domains are retrieved from the zone files of multiple top level domains (.bid, .date, .download, .fun, .host, .icu, .loan, .online, .pro, .review, .site, .space, .stream, .tech, .top, .trade, .website, .win, and .xyz) available via the Centralized Zone Data Service (https://czds.icann.org/en). 

Additional stats of the feed and the results of a comparative analysis will be presented at IEEE BigData in December 2018 (http://cci.drexel.edu/bigdata/bigdata2018/). 

## Call to action: 
We look forward to expanding the feed by either analyzing other open data sources, or by detecting other categories of malicious domains. Either way, if you would like to contribute to this project please do get in touch!  


## Copyright
Copyright (c) 2018 PatternEx Inc. The data is distributed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA) license. [![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/). You may use the data for limited, non-commercial purposes and with no expectation of warranty nor support. 

For further information please contact: threatex@patternex.com
