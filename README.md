## Hi! I'm Dhruv Banerjee 

#### I'm a student at the London School of Economics, interested in the intersection of data science and public policy

- 🌱 I’m currently learning about how to use Data Science, Machine Learning, and Data Analysis with reference to policy-related areas such as education, health, and economics

- 🔭 I’m working on understanding better how data science and AI can be most beneficially incorporated into public services, and regulated to reduce risk without stifling growth. I genuinely believe that if used properly, technologies such as AI can evenly spread out economic growth. 

- 📫 How to reach me: via email at D.Banerjee1@lse.ac.uk or Linkedin at [Dhruv Banerjee](https://www.linkedin.com/in/dhruv-banerjee-514983287/) 

## **End-to-End ML Projects**

## Investment Atlas: AI-Powered Regional Economic Analysis

**The Challenge**

India's economic growth remains heavily concentrated in 15-20 metro districts, while 200+ districts continue to depend primarily on agriculture with limited access to diversified economic opportunities. This concentration creates significant market inefficiencies: 60% of the population resides in underutilized economic zones, investment capital clusters in saturated metro markets, and an estimated ₹10,000+ crores in annual potential remains untapped.

**The Solution**

I developed an end-to-end machine learning platform to systematically identify high-potential districts for strategic investment and economic diversification. The analysis covered 180 districts across four major states (Maharashtra, Tamil Nadu, Karnataka, Uttar Pradesh), representing a combined population of 510 million people.

**Technical Approach & Key Findings**

Using ensemble machine learning methods, I built a predictive model that revealed infrastructure connectivity as the single most important factor for investment success, accounting for 28% of the prediction weight. This finding challenges conventional wisdom—traditional indicators like literacy rates and population size ranked surprisingly low, suggesting that digital and physical connectivity are now the primary drivers of regional economic potential.

The model classified districts into three distinct economic profiles:
- **Advanced Economic Hubs:** 130 districts with established infrastructure
- **Industrial Transformation Zones:** 37 districts showing rapid industrial development
- **Agro-Processing Opportunities:** 13 districts with strong agricultural base and processing potential

<p align="center">
  <img src="https://github.com/user-attachments/assets/7bef6693-ff97-4951-92a7-1b84d7bc1416" alt="ML Model Results Dashboard" width="700" />
</p>

**Business Impact**

The analysis identified sector-specific opportunities with potential to create 16,000+ new business units. By matching sectors to regions with demonstrated comparative advantages, the platform provides actionable investment recommendations that balance risk across different economic models.

<p align="center">
  <img src="https://github.com/user-attachments/assets/11e0eda4-1582-4a54-9a9b-c1e62b9436e0" alt="Sectoral opportunity mapping across regions" width="700" />
</p>

**Strategic Value:** This methodology translates complex socioeconomic data into investment-grade intelligence, enabling data-driven capital allocation decisions for private equity, government planning, and corporate expansion strategies.

## Textual Analysis & Topic Modelling

Natural Language Processing has become increasingly valuable for policy research, enabling analysis of large-scale discourse patterns that would be impossible to detect manually. I've applied these techniques to examine how political priorities evolve over time and across different actors.

**Project: EU Policy Discourse Analysis (2009-2023)**

Working with a comprehensive dataset of 106,000+ speeches from European Parliament debates spanning 15 years, I developed a two-part analytical framework to uncover patterns in party priorities and policy evolution.

**Part 1: Political Similarity Analysis**

Using dimensionality reduction (PCA) and cosine similarity measures on speech embeddings, I mapped ideological proximities across party groups. The analysis revealed an unexpected pattern: centrist parties demonstrate significantly higher inter-group similarity compared to parties at either end of the political spectrum. This suggests centrist coalitions may find common ground more readily than left-wing or right-wing blocs among themselves.

<p align="center">
  <img src="https://github.com/user-attachments/assets/30aacd20-a2f9-4352-887d-9d4d9c8d6481" alt="PCA visualization of party similarity" width="450" />
  <img src="https://github.com/user-attachments/assets/3e972ad6-faa2-48ed-85b3-804cfc3c7cfe" alt="Cosine similarity heatmap" width="450" />
</p>

**Part 2: Temporal Topic Evolution**

After evaluating multiple approaches (LSA, LDA), I implemented BERTopic for its superior semantic understanding. The model identified 140 distinct topics, which I refined through hierarchical clustering and intertopic distance mapping. I selected six substantive policy themes that appeared frequently and demonstrated clear temporal patterns.

By tracking topic prevalence across years, I mapped how EU discourse shifted in response to external events—from financial crises to migration flows to climate negotiations. This temporal analysis provides quantifiable evidence of how legislative priorities respond to real-world developments.

<p align="center">
  <img src="https://github.com/user-attachments/assets/d672432f-b612-46f9-8eeb-57dd1e46d528" alt="Temporal trends in EU policy topics" width="800" />
</p>

**Impact:** This methodology can be applied to analyze any large corpus of institutional discourse, offering data-driven insights into policy shifts, coalition patterns, and emerging priorities—valuable for strategic planning in both public and private sectors.

