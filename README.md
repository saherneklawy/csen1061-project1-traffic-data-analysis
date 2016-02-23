# Project 1: Traffic Data Analysis
project duration: 24/2/2016 - 7/4/2016

## Project Description

We all suffer from traffic, and as data scientists looking into this data is a gold mine.
Such data can be seen in bey2ollak.com, where the state of the roads is reported by people around Cairo and Alexandria.
People can report the state of traffic into one of the following categories:

- 7alawa
- lazeez
- mashy
- za7ma
- mafeesh 2amal

as well as ask for updates.

You are provided with data of reports from Feb 6 2016 to Feb 20 2016 (around 2 weeks of data).
Given this data set, you need to apply the concepts introduced to you so far in the course to come up with a data analysis report. This should include:

1. Figure out the different metrics of interest in this dataset.
2. Figure out the dimensions by which you could aggregate, group, or facet the metrics of interest.
3. Apply what you learned about descriptive statistics to investigate the metrics and dimensions.
4. Apply what you learned about data visualization and distribution investigation.
5. Apply what you learned about parameter inference to calculate confidence intervals for some of the descriptive statistics you calculated.
6. [Bonus] Come up with at least 2 hypotheses and verify/disprove them using "Null Hypothesis Testing" supported with textual commentary.

See "Data Analysis Getting Started" below.

Note that for all the above you need to support your conclusions and observations with textual commentary.

Furthermore, you are expected to augment, manipulate, clean the data to reach more information. For example the data doesn't include the city for the given road. You need to figure this out.


## Data definition

You can obtain the data itself from the following link: https://www.dropbox.com/s/b19mm1b44anpo6s/traffic-data.csv.gz?dl=0
The data set contains the following columns:

* crawl_date
* ad.aid
* ad.bgcl
* ad.bgcls
* ad.fncl
* ad.fncls
* ad.lid
* ad.logo
* ad.logo2x
* ad.logoAndroidS
* ad.logoAndroidH
* ad.cm
* ad.url
* ad.g
* rd.nm
* rd.ri
* rd.stid
* rd.hr
* rd.mn
* rd.new
* rd.img
* rd.cl
* rd.strq
* rd.cmrq
* rd.rp.nm
* rd.rp.fullnm
* rd.rp.hr
* rd.rp.mn
* rd.rp.stid
* rd.rp.cm
* rd.rp.cmid
* rd.rp.rpImg
* rd.rp.img
* rd.rp.type


The data was acquired by crawling bey2ollak.com at a 30 minute interval. This provides details about:
 
* crawl_date: the date this data was crawled in UTC (this is 2 hours behind Cairo time)
* an advertisement that is shown for each road (ad.*)
* road information (rd.*)
* report submitted by a user (rd.rp.*)

Note that looking at the html of bey2ollak.com will prove to be useful :)


## Deliverable

You are expected to submit data analysis report in the form of a R Markdown report showing each step of your work in processing, cleaning, augmenting, and describing the data.

This should be submitted by pushing your work regularly on a repo on github that is forked from https://github.com/saherneklawy/csen1061-project1-traffic-data-analysis
Make sure to commit and push regularly your work. Having commits only on the last day will not be accepted.

After the submission deadline, you will be expcted to review/comment on 2 other EDAs that you will be assigned.


## Data Analysis Getting Started

1. Exploratory Data Analysis:
    1. Identify metrics and dimensions
    1. Descriptive Statistics
        1. Summary statistics
            1. Measures of central tendency
            1. Measures of spread
            1. Enumeration
        1. Data Visualization
            1. Summary statistics i.e. Box Plot
            1. Distribution & Normality (i.e. histogram, empirical cumulative density function, Q-Q plot)
        1. Commentary    
    
    To Remember: Grouping a metric by a dimension then running analysis. 
2. Inferential Data Analysis:
    1. Parameter Inference (confidence intervals)
    1. Hypothesis Testing (null hypothesis testing)
