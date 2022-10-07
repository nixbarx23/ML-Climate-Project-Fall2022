
## **Update October 7, 2022:**

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
