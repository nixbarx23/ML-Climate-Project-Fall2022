**Problem Statement:**

In finance, ESG has gained more and more momentum with clients increasing their expectations of investment managers that can help achieve certain sustainability or other ESG-related objectives. While ESG has become more popular, some asset knowns are making their goals more precise when it comes to whether they relate to E (Environment), S (Social), or G (Governance). As the types of areas that investors and asset owners want to conceptually target, defining such a topic in terms of the available data can be challenging without the knowledge of which data point, or points, can best achieve the objective/target in question. Therefore, a framework that help inform the composition or definition of a theme in terms of data is needed.

An example: If a client is determined to target companies that produce excessive amounts of pollution & waste, what would be the best combination of metrics such as the amount of hazardous waste they create, non-recyclable waste, or different intensity metrics related to harmful emissions.

**Objective of Proposed Research:**

The ultimate objective of the research would be create a framework, based on causal discovery and modeling, that could inform the weighting of possible data points related to a specific theme. The goal would be to create a framework that is theme-agnostic so that it can be leveraged for themes across the E, S, and G pillars without imposing prior knowledge on the onset of the definition of the theme.

An example: Theme: Pollution & Waste Related data points: hazardous waste, non-recyclable waste, hazardous emissions Hypothetical Output: Based on the framework created, the informed combination of possible data points to define the theme of "pollution & waste" is 65% hazardous waste, 18% non-recyclable waste, and the remaining 17% equally distributed across the specific hazardous emission intensity metrics.

**Data Sources:**

The data used for this research will include a variety of data points focused on the "bottom-level" metrics associated with each theme. Each of these datasets would include values for a variety of companies that span different types of industries and region. The types of data will span continuous quantitative data, binary data, and other topic-specific precomputed scores.

An example: The structure of the data is organized as shown in the following outline. The idea would be to initially use only the individual metrics for a given theme. These individual data points have already been mapped to each theme. Later versions of this research could include using data points that are not explicitly mapped to a given theme in case there exists a relationship between the theme and a seemingly "unrelated" data point. 

Level 1: Theme A

    Level 2: Data 1A
    
    Level 2: Data 2A
    
    Level 2: Data 3A


Level 1: Theme B

    Level 2: Data 1B
    
    Level 2: Data 2B
    
    Level 2: Data 3B

**Overview of Research Approach:**

The majority of the desired framework that is to be the output will be based on causal modeling. One benefit of causal modeling is the interpretability of the results. Additionally, in the event that weights to combine individual metrics in order to construct a definition for a given theme is not possible, the causal model will hopefully provided a more informed view of the relationships between the individual components of  used for this research will include a variety of data points focused on the "bottom-level" metrics associated with each theme. The types of data will span continuous quantitative data, binary data, and other topic-specific precomputed scores.
