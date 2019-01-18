# Python based Text Analysis of San Francisco 311 non emergency dataset

Data Mining for better resource allocation to better serve 311 non emergencies at San Franscisco

Size of dataset: 16 * 2022095.
Period: July 2008 to Oct. 2016.
Location: San Francisco.
Missing data: Total 2702233 (8.35% of total dataset). 
Column names/type: CaseID - (Numeric); Opened - (Timestamp); Closed - (Timestamp); Updated - (Timestamp); Status - (Text); Status Notes - (Text); Responsible Agency - (Text); Category - (Text); Request Type - (Text); Request Details - (Text); Address - (Text); Supervisor District - (Numeric); Neighborhood - (Text); Point - (Geometry: Point); Source - (Text); Media URL - (Text);


Actionable insights from San Francisco 311 request dataset
The dataset consists of details for San Francisco's 311 call requests along with the phone call descriptions for the period 2008 to 2017.

The data set was narrowed down to 6 target neighborhoods at San Franscisco. 2 neighborhoods were chosen for further analysis where there were no abrupt changes in the number of complains over the period 2008 to 2017. For the remaining 4 neighborhoods, the complaints changed abrupty over the timeline, indicating that the state borders may have chnaged over the years.

Next, a top down analysis of the neighborhoods was done based on the trend of the number of requests for each category in the 2 targetted neighborhoods.

For the sake of simplicity, 2 categories of requests were identified, one with an increasing trend and the other with a decreasing trend for each of the 2 neighborhoods.

The following category requests were chosen for each neighborhood.

For the neighborhood: Mission,
1) 311 External Requests (increasing trend in number of requests) and
2) Tree_Maintenance (decreasing trend in in number of requests)
For the neighbourhood: Nob Hill,
1) Graffiti Private Property (increasing trend in number of requests) &
2) Sidewalk or Curb (decreasing trend in in number of requests)
Using text analysis in Python,

1) the top 10 most important call request issues were identified for the request types with increasing trend in number of requests received and,
2) the 10 least important call request issues were identified the request type with decreasing trend in number of requests received
The above analysis was done for the years 2015 & 2016 only (among the period 2008 to 2017) for the most recent trend associated with each request type. The data for 2017 was not used because data for the entire year 2017 was not available.

Based on the above analysis, actionable insights for the managers in the 311 departments can be a more efficient resource allocation by transfering the resources associated with the bottom most 10 types of issues for the category with decreasing trend to the top 10 most important issues for the category with increasing trend for each of the above neighborhood.
