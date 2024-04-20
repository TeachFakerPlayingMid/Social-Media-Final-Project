# Social-Media-Final-Project
## Data Overview

This dataset is constructed for a network analysis project centered around fifteen Artificial General Intelligence (AGI) influencers and the individuals they follow on Twitter. The dataset includes data for each profile both for the influencers (Key Opinion Leaders - KOLs) and their followings (followers - FOs). Each row in the dataset represents a relationship between a KOL and a FO, detailing various attributes related to both parties.

### Key Columns Described

- **profileUrl**: URL to the Twitter profile of the follower.
- **screenName_fo**: Twitter handle of the follower.
- **userId_fo**: Unique identifier for the follower's Twitter account.
- **name_fo**: Full name of the follower as displayed on Twitter.
- **imgUrl_fo**: URL to the follower's profile image.
- **bio_fo**: Bio of the follower, summarizing their interests or professional background.
- **website_fo**: The website linked in the follower’s Twitter profile.
- **location**: Geographic location provided by the follower.
- **location_cleansed**: Standardized format of the geographic location.
- **createdAt_fo**: Date and time when the follower’s Twitter account was created.
- **followersCount_fo, friendsCount_fo, tweetsCount_fo**: Numbers representing the followers, friends, and total tweets of the follower respectively.
- **certified_fo**: Indicates whether the follower's Twitter account is verified.
- **timestamp_fo**: Timestamp noting when the data was collected.
- **position_categorized**: Standardized job role or position of the follower.
- **highest_level_org**: The most significant organization associated with the follower.
- **screenName_kol, userId_kol, name_kol**: Corresponding details for the influencer.
- **bio_kol**: Bio of the influencer, providing insight into their professional and personal focus areas.
- **createdAt_kol**: Creation date of the influencer’s Twitter account.
- **followersCount_kol, friendsCount_kol, tweetsCount_kol**: Social media metrics for the influencer.
- **certified_kol**: Verification status of the influencer's account.

### Usage of the Dataset

This dataset is valuable for understanding the network dynamics, influence patterns, and potential information dissemination among key players in the field of AGI on social media. By analyzing the relationships and attributes such as follower counts, verification status, and positions held, researchers can infer influence trends, network robustness, and pivotal nodes within this social graph. This analysis can further be applied to study how information related to artificial intelligence is shared, perceived, and proliferated among industry experts and enthusiasts on platforms like Twitter.


# Potential Ideas

## Analysis of Professional Backgrounds and Organizational Influence in Network Dynamics

### Objective
To explore how the professional roles and organizational affiliations of influencers and followers shape the network structure and influence patterns within the AGI community on Twitter.

### Methodology
1. **Role-Based Network Analysis**:
   - **Categorize nodes based on roles**: Utilize the cleaned and categorized roles (e.g., researcher, public figure, author) to categorize the nodes. This will allow you to analyze the network characteristics of each category, such as centrality measures, connectivity, and influence within and across groups.
   - **Examine influence by role**: Investigate whether certain professional roles are more influential in terms of network metrics such as betweenness centrality (indicating nodes that bridge different parts of the network) and degree centrality (indicating nodes with the most connections).

2. **Organizational Influence**:
   - **Map organizational affiliations**: Create sub-networks based on organizational affiliations to see how individuals connected to major organizations (like Google DeepMind, OpenAI, etc.) cluster and interact.
   - **Analyze inter-organizational connections**: Determine how organizations influence the AGI discussion by looking at connections between individuals from different organizations. This could reveal alliances or rivalries, as well as collaborative clusters in the AGI field.
   - **Organizational roles in spreading information**: Track how information (e.g., news articles, research papers, major announcements) originates and spreads from individuals associated with key organizations.

3. **Comparative Analysis**:
   - **Cross-analyze role and organization influence**: Compare the influence patterns based on roles and organizational affiliation to see which factor plays a more significant role in defining network structures and influence. For instance, do individuals from prestigious organizations hold more sway regardless of their role, or do roles like 'researchers' or 'public figures' have consistent influence across different organizational contexts?

4. **Visualization**:
   - **Visual network mapping**: Use network visualization tools to illustrate the role and organization-based clusters within the broader AGI influencer network. Highlight key nodes, illustrate pathways of information flow, and depict inter-organizational links.

### Expected Outcomes
- Insights into how professional roles impact the dissemination and reception of AGI-related information.
- Understanding of how organizational affiliations shape the network, potentially influencing collaborative projects and policy directions within the AGI community.
- Enhanced comprehension of the structural roles organizations play in the AGI discourse on social media.


## Identifying Emerging Founders in the AGI Field through Network Analysis

#### Objective
To identify lesser-known yet influential founders in the Artificial General Intelligence (AGI) sector using network centrality and community detection methods. This approach aims to spot potential investment leads by highlighting founders who, despite having a smaller overall following, play critical roles within key AGI networks.

#### Methodology
1. **Identify Founders**:
   - **Tag Profiles**: Use the cleaned data to tag profiles based on their roles, specifically marking those who are categorized as 'founders'. This could involve a text search for keywords like "founder", "co-founder", or "CEO" within their bio or position descriptions.

2. **Measure Influence**:
   - **Centrality Analysis**: Apply centrality metrics such as betweenness, closeness, and eigenvector centrality to understand the roles these founders play in the network. High betweenness centrality might indicate founders who act as bridges between different influential communities or networks.
   - **Influence beyond Followers**: Look for founders with high centrality scores but relatively lower follower counts, suggesting they are influential within important niches but not widely recognized outside.

3. **Community Detection**:
   - **Detect Subnetworks**: Use community detection algorithms to find clusters within the network that are dense with founders. Analyze these clusters to determine if they consist of individuals from related startups or from certain subfields within AGI.
   - **Cross-Cluster Influence**: Identify founders who have links across multiple high-influence communities or who are central in clusters predominantly featuring well-known influencers.

4. **Visualization and Reporting**:
   - **Network Maps**: Create visualizations showing the position and connectivity of these founders within the AGI community. Highlight founders with high centrality but lower visibility in terms of follower count.
   - **Report Generation**: Develop reports listing potential founders who meet the criteria for influence within key communities but are less known in broader circles, providing a resource for venture capitalists.

#### Expected Outcomes
- A curated list of emerging founders in the AGI sector who are recognized within influential circles but are not widely known to the public.
- Insights into the structural roles these founders play within the AGI community, which could guide investment decisions.
- Enhanced understanding of sub-communities within the AGI field, potentially revealing new trends and areas ripe for investment.