## **Update October 24, 2022:**


Scope of metrics related to human capital/human resources themes now include continuous variables as well as discrete scores. Columns include:
- Severity of Employee Health & Safety Controversies (discrete, precomputed score, possible values: 1-10)
- Total Recordable Incident Rate
- Fatalities/Employees - Most Recent
- Lost Time Incident Rate (per million hours) - Most Recent
- Percentage of Health & Safety System Certified to OHSAS 18001
      - OHSAS 18001 focuses on controlling hazards. It provides a framework for the effective management of occupational health and safety including all aspects of           risk management and legal compliance. It addresses occupational health and safety rather than any specific product safety matters.
- Severity of Discrimination & Workforce Diversity Controversies (discrete, precomputed score, possible values: 1-10)
- Severity of Labor Management Relations Controversies (discrete, precomputed score, possible values: 1-10)
- Severity of Collective Bargaining & Union Controversies (discrete, precomputed score, possible values: 1-10)
- Major Layoffs
- Over 20% of workforce considered part-time or temporary (-1,0)
- Percentage of women in executive management (%)
- Percentage of women in workforce (%)
- Annual employee turnover (%)
- Professional development annual training hours per employee
- Percentage of women in senior management (%)
- Severity of Supply Chain Labor Standards Controversies (discrete, precomputed score, possible values: 1-10)
- Severity of Impact on Local Communities Controversies (discrete, precomputed score, possible values: 1-10)
- Severity of Civil Liberties Controversies (discrete, precomputed score, possible values: 1-10)
- Severity of Human Rights Concerns Controversies (discrete, precomputed score, possible values: 1-10)
- Severity of Other Human Rights Controversies (discrete, precomputed score, possible values: 1-10)
- Severity of Child Labor Controversies (discrete, precomputed score, possible values: 1-10)
- Severity of Other Labor Rights Controversies (discrete, precomputed score, possible values: 1-10)
- Severity of Supply Chain Labor Standards Controversies (discrete, precomputed score, possible values: 1-10)


Current areas of focus include:
- due to differences in data coverage across the full inventory of metrics, need to determine whether to focus only on observations with valid values across all metrics or allow for some metrics to be NaN. If so, how to process NaN in conditional independence testing. 
- developing framework to evaluation independence-relationship between continious and discrete variables. Will explore possible encoding or bucketing of continious variables to make discrete. 


## **Update October 7, 2022:**


##### *FIGURES SHOULD BE ABLE TO BE UPLOADED BY EARLY WEEK OF 10/10* -- finalizing permissions to upload.


Initial EDA on HCM-related KPIs was conducted on the set of continuous variables. Characteristics examined:

- distribution of each variable
- pairwise scatterplot matrix
- (ADDITIONAL COMPONENTS TO BE ADDED)

*Sample figure created can be found in the figure folder.* 

In addition to developing EDA capabilities, have focused on conditional independence/regression testing and graph visualization.

**Conditional Independence/Regression Testing:**

Within the larger CDT library, using specific capabilities within the Independence.Stats component. Initial analysis will focus on running pairwise indepdence tests with each relevant data column (some test results depdend on the direction i.e. A, B is different than B, A). Initial results are being reviewed within a N x N (for N data columns) pairwise matrix. 

Initial tests being conducted:
- Spearman and Pearson correlations
- Mutual Information Regression     

**Graph Visualization:**

Using Python library Algorithmx, have begun building out initial capabilities for graph visualization. 

*Sample figure created can be found in the figure folder.* 

## **Update September 30, 2022:**

The data associated with a given issue follows the given structure:
- individual KPIs mapped to issues (focus area of research)
- issues mapped to themes, themes mapped to E, S, G pillars

Each KPI can be one of the following types of metrics:
- continuous series
- binary (policy focused)
- discrete scores (focused on severity)

The first iteration of the analysis will focus just on the continious-type KPIs, but will explore the introduction of binary and other discrete metrics later on.

Preliminary issue in focus will be within the human capital management (HCM) space. Query for data was created and collects data for a given set of KPIs on a single day. Will focus initially on developing framework on data for a single day (given data is cross sectional), but once framework for a single day is created, will look into running over certain look back window (either average the framework results on a daily basis or input average lookback period metrics into framework). 

## **Update September 23, 2022:**

Focusing on causal modeling to determine the dependent relationship between variables common to a single issue. The overall objective is to determine a systematic framework the can provide a more informed view into how to combine the underlying metrics to create an aggregate issue score. The approach would be based on the results of conditional independence tests, regressions, and correlation-based analyses. 

Ultimately, the goal would be first to get a better understanding of the relationship between data points within a given theme (which can in turn provide a greater level of transparency to clients and ratings creations). Secondly, the framework would help provide a scalable solution to creating more granular issue ratings.
