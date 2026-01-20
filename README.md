## Hi, I'm Dhruv Banerjee 

**MSc Data Science @ LSE** 

I'm obsessed with innovation, with experience in data science and AI across a range of sectors, including energy, policy, and business strategy. I'd be happy to have a chat if you're looking to drive impactful change!

**What I'm building:**
- Currently working on practical end-to-end agentic systems.
- In the works is a tool to link solutions from the latest academic research to industry-specific use cases.
- Really interested in the tech startup space, as well as those supporting such ventures.

**Background:**
- Pursuing an MSc in Data Science at the London School of Economics.
- BA in Politics (+ Data Science) at Sciences Po Paris 
- Experience applying data science and AI across commercial, policy, and energy sectors.

**Tech stack:** Python, PyTorch, scikit-learn, BERTopic, SQL, data visualization, agentic AI (Langchain, LangGraph)  
**Interests:** NLP, predictive modeling, causal inference, marketplace dynamics, investment research


**Let's connect:**  
📧 D.Banerjee1@lse.ac.uk | 💼 [LinkedIn](https://www.linkedin.com/in/dhruv-banerjee-514983287/) | 

---
## Agentic AI Systems
Modern AI development increasingly relies on multi-agent architectures where specialized models collaborate to solve complex problems. I've built systems that orchestrate multiple AI agents to process, analyze, and translate technical content at scale, demonstrating practical applications of LangGraph and production LLM workflows.

### **Project: Radar - AI Research Intelligence Agent**
**[GitHub Repository](https://github.com/Dhruv-baner/radar)** | **[Architecture Docs](https://github.com/Dhruv-baner/radar/blob/main/docs/architecture.md)** | **[Example Output](https://github.com/Dhruv-baner/radar/blob/main/docs/example-output.md)**

An autonomous multi-agent system that discovers, analyzes, and translates cutting-edge AI research from ArXiv into accessible insights for non-technical stakeholders. The system automatically processes 50-200 papers daily through a three-stage pipeline: 
- Paper Analyzer agent extracts technical insights
- Simplifier agent generates accessible explanations using a structured Challenge→Solution→Impact format
- Industry Matcher agent (in development) maps innovations to real-world applications across sectors.

<div align="center">
  <img src="https://raw.githubusercontent.com/Dhruv-baner/radar/main/assets/architecture-diagram.png" width="700" alt="Radar Agent Pipeline Architecture"/>
</div>

**Technical Architecture**

- The pipeline begins with ArXiv API integration filtering papers by AI/ML categories (cs.AI, cs.LG, cs.CL, cs.CV), followed by **PyMuPDF-based text extraction** that parses PDFs into structured sections. 
- The **LangGraph orchestration** layer manages state flow between specialized agents: the Paper Analyzer processes 8,000+ character inputs to extract methods, results, and limitations; the Simplifier transforms technical content through Claude Sonnet 4 into executive summaries, challenge context, and key technical points.
- All outputs are structured as JSON for downstream applications, achieving 100% processing reliability with 60-second average latency per paper.

**Technology Stack**

**Orchestration:** LangGraph, LangChain | **LLM:** Claude Sonnet 4 (Anthropic) | **Processing:** PyMuPDF, Python | **Data Source:** ArXiv API | **Storage:** JSON/CSV | **Development:** Jupyter, Git

**Impact & Scale**

Transforms dense academic papers (avg. 66,000 characters) into 2-minute accessible reads while preserving technical accuracy. Demonstrated on papers ranging from graph neural networks to ensemble decoding, achieving consistent quality across diverse AI subfields. System designed for daily automation via GitHub Actions to generate weekly research digests.

---

## MLOps 

### **Featured Project: UK Energy Grid Dashboard**

Real-time monitoring system analyzing UK electricity generation patterns with production MLOps infrastructure.

![UK Energy Dashboard](https://raw.githubusercontent.com/Dhruv-baner/uk-energy-grid/main/assets/uk_energy_dashboard.png)

**Key Findings:**
- UK grid averaged **49.6% renewable** energy (30-day analysis)
- **Wind generation (36.7%)** now rivals gas (38.1%)
- Peak renewable: **77.1%** | Coal completely phased out
- Built with Python, Plotly, Prophet forecasting & MLflow tracking

**[View Full Analysis](https://github.com/Dhruv-baner/uk-energy-grid)**
---

## Textual Analysis & Topic Modelling

Natural Language Processing has become increasingly valuable for policy research, enabling analysis of large-scale discourse patterns that would be impossible to detect manually. I've applied these techniques to examine how political priorities evolve over time and across different actors.


### **Project: Regulation Tracker**

**[Live Dashboard](https://regulationnews-khvu3dtti5pz8f2gr5dw9f.streamlit.app/)** | **[GitHub Repository](https://github.com/Dhruv-baner/regulation_news)**

An agentic intelligence platform monitoring regulatory developments across five major markets (USA, UK, France, Germany, Japan), processing 100+ articles daily through GPT-powered analysis to generate actionable insights for institutional investors. The system aggregates multi-source data, performs LLM-based relevance scoring and categorization, and delivers interactive visualizations for real-time regulatory intelligence.

<img src="https://raw.githubusercontent.com/Dhruv-baner/regulation_news/main/assets/screenshots/plot_2.png" width="400" align="left" alt="Market Overview"/>
<img src="https://raw.githubusercontent.com/Dhruv-baner/regulation_news/main/assets/screenshots/plot_3.png" width="400" align="right" alt="Distribution Analysis"/>

<br clear="both"/>

**Technical Architecture**

The data pipeline aggregates regulatory news from NewsAPI and Google News RSS feeds, performing automated deduplication and market-specific keyword filtering for regulatory authorities (SEC, FCA, BaFin, AMF, FSA). Custom GPT-3.5-turbo prompts analyze each article to generate structured outputs including relevance scores (0-10), impact classifications (High/Medium/Low), regulation categories (Data Privacy, Financial Services, AI/Tech, Environmental, Securities), key regulator identification, and executive summaries. The visualization layer features five interactive Plotly dashboards with real-time filtering capabilities by market, category, impact level, and relevance threshold.

**Technology Stack**

**Backend:** Python, Pandas, LangChain | **LLM:** OpenAI GPT-3.5-turbo | **Visualization:** Plotly, Streamlit | **Data Sources:** NewsAPI, Google News RSS | **Deployment:** Streamlit Cloud

<img src="https://raw.githubusercontent.com/Dhruv-baner/regulation_news/main/assets/screenshots/plot_4.png" width="400" align="right" alt="Regulation Categories by Market"/>
<img src="https://raw.githubusercontent.com/Dhruv-baner/regulation_news/main/assets/screenshots/plot_1.png" width="400" align="left" alt="Geographic Intelligence View"/>

<br clear="both"/>

**Key Capabilities**

The platform delivers intelligent scoring through GPT-powered relevance assessment on a 0-10 scale, prioritizing high-impact regulatory changes. It provides simultaneous monitoring across USA, UK, Germany, France, and Japan with market-specific authority tracking. Interactive filtering enables dynamic dashboard updates by market, category, impact level, and relevance threshold. The system performs automated daily processing of 100+ articles with structured categorization and executive summaries, delivering curated insights for investment decision-making.


### **Project: EU Policy Discourse Analysis (2009-2023)**

Working with a comprehensive dataset of 106,000+ speeches from European Parliament debates spanning 15 years, I developed a two-part analytical framework to uncover patterns in party priorities and policy evolution.

**Part 1: Political Similarity Analysis**

Using dimensionality reduction (PCA) and cosine similarity measures on speech embeddings, I mapped ideological proximities across party groups. The analysis revealed an unexpected pattern: centrist parties demonstrate significantly higher inter-group similarity compared to parties at either end of the political spectrum. This suggests centrist coalitions may find common ground more readily than left-wing or right-wing blocs among themselves.

  <img src="https://github.com/user-attachments/assets/30aacd20-a2f9-4352-887d-9d4d9c8d6481" alt="PCA visualization of party similarity" width="400" align="right"/>
  <img src="https://github.com/user-attachments/assets/3e972ad6-faa2-48ed-85b3-804cfc3c7cfe" alt="Cosine similarity heatmap" width="400" align="left"/>

  <br clear="both"/>


**Part 2: Temporal Topic Evolution**

After evaluating multiple approaches (LSA, LDA), I implemented BERTopic for its superior semantic understanding. The model identified 140 distinct topics, which I refined through hierarchical clustering and intertopic distance mapping. I selected six substantive policy themes that appeared frequently and demonstrated clear temporal patterns.

By tracking topic prevalence across years, I mapped how EU discourse shifted in response to external events—from financial crises to migration flows to climate negotiations. This temporal analysis provides quantifiable evidence of how legislative priorities respond to real-world developments.

<p align="center">
  <img src="https://github.com/user-attachments/assets/d672432f-b612-46f9-8eeb-57dd1e46d528" alt="Temporal trends in EU policy topics" width="500" />
</p>

**Impact:** This methodology can be applied to analyze any large corpus of institutional discourse, offering data-driven insights into policy shifts, coalition patterns, and emerging priorities—valuable for strategic planning in both public and private sectors.

---
## **End-to-End ML Projects**

### **Project: Investment Atlas - AI-Powered Regional Economic Analysis**

**The Challenge**

India's economic growth remains heavily concentrated in 15-20 metro districts, while 200+ districts continue to depend primarily on agriculture with limited access to diversified economic opportunities. This concentration creates significant market inefficiencies: 60% of the population resides in underutilized economic zones, investment capital clusters in saturated metro markets, and an estimated ₹10,000+ crores in annual potential remains untapped.

**Note: The project is deployed on Streamlit, with in-depth insights and interactive visualisations**

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
