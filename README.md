# Social Computing Project

This repository contains the code and datasets for a project that analyzes the voting patterns of countries in the UN Security Council. The project leverages socio-economic data, resolutions, and voting behavior to understand geopolitical dynamics and uses a Retrieval-Augmented Generation (RAG) model to generate detailed responses based on the data.

## Project Objectives

- **Scrape and Process Data**: Automate the collection of Security Council resolutions from the UN's Digital Library.
- **Analyze Voting Patterns**: Examine how socio-economic factors influence voting behaviors in the Security Council from 2000 to 2020.
- **Data Visualization**: Use statistical and visualization techniques to present insights into geopolitical stances.
- **Retrieval-Augmented Generation**: Use a RAG model to synthesize responses that provide in-depth analysis of specific geopolitical scenarios and voting patterns.

## Project Structure

```
/
|-- social_computing_project.ipynb   # Main Jupyter notebook
|-- UN DATA.csv          # CSV file containing resolutions data
|-- soci_econ_country_profiles.csv  # CSV file containing socio-economic data
|-- requirements.txt # File listing all the necessary Python packages
```

## Generated files once executed

```
/
|-- Folder containing all the scraped resolutions
|-- Full_UN_Resolutions.csv          # CSV file containing resolutions data
|-- Encoded_UNSC_Voting_Data.csv     # CSV file containing processed voting data
```

## Getting Started

### Prerequisites

- Python 3.x
- Jupyter Notebook or JupyterLab
- Libraries: pandas, numpy, matplotlib, seaborn, beautifulsoup4, requests, pdfplumber, pymupdf, fitz, langchain, langchain-groq, faiss-cpu, python-dotenv, sentence-transformers

### Installation

```
git clone <repository-url>
cd <repository-name>
pip install -r requirements.txt
```

### Running the Notebook

```
jupyter notebook
```

Execute the notebook cells sequentially to reproduce the analysis.

## Retrieval-Augmented Generation (RAG) Component

The project utilizes a Retrieval-Augmented Generation model, which integrates powerful retrieval capabilities with a transformer-based language model to generate detailed, context-aware responses. This RAG system is pivotal in answering complex queries by synthesizing information from a comprehensive database containing UN resolutions, socio-economic profiles, and historical voting data.

### Sample Query Execution

Below is a shortened example of how the RAG model is queried to generate an in-depth analysis based on the socio-economic data and resolutions. This example showcases the model's ability to synthesize and structure output correctly by fetching relevant data and generating coherent insights:

```
Querying the RAG model...
> Question: Analyze Germany's economic policies and their impact on the European Union's economic stability and growth.

> Response: "Answer: Based on the provided socio-economic data, Germany's economic policies and their impact on the European Union's economic stability and growth can be analyzed as follows:

**Economic Performance:**

Germany's GDP per capita is the highest among all the countries listed, at $41,686.2 (2017). This indicates a strong economy with a high standard of living. Germany's GDP growth rate is also one of the highest, at 1.7% (annual, constant 2005 prices). This suggests that Germany's economy is growing steadily and is likely to be a driving force for economic stability and growth in the European Union.

**Industry and Services:**

Germany's industry sector accounts for 30.5% of its GDP, which is relatively high compared to other countries in the European Union. This suggests that Germany has a strong industrial base and is likely to be a significant contributor to the EU's industrial growth. The services sector, which accounts for 59.5% of Germany's GDP, is also significant, indicating a strong service sector that is likely to drive economic growth.

**Agriculture:**

Germany's agriculture sector accounts for only 0.6% of its GDP, which is relatively low compared to other countries in the European Union. This suggests that agriculture is not a significant contributor to Germany's economy, but it is still an important sector for food production and rural development.

**Impact on EU Economic Stability and Growth:**

Germany's strong economy and high GDP per capita make it an important contributor to the European Union's economic stability and growth. As one of the largest economies in the EU, Germany's economic performance has a significant impact on the EU's overall economic performance. Germany's strong industrial base and service sector also make it an important driver of EU economic growth.

**Challenges:**

Despite Germany's strong economy, there are still some challenges that need to be addressed. For example, Germany's high labor costs and strict labor laws may make it difficult for other EU countries to compete with Germany in terms of labor costs. Additionally, Germany's strong economy may also lead to trade tensions with other EU countries, particularly if there are disagreements over trade policies and regulations.

**Recommendations:**

Based on the analysis, the following recommendations can be made:

1. **Encourage trade and investment:** Germany should continue to encourage trade and investment with other EU countries to promote economic growth and stability.
2. **Support small and medium-sized enterprises (SMEs):** Germany should support SMEs to promote entrepreneurship and job creation.
3. **Address labor market challenges:** Germany should address labor market challenges, such as high labor costs and strict labor laws, to make it easier for other EU countries to compete with Germany.
4. **Promote EU integration:** Germany should continue to promote EU integration to promote economic stability and growth.

In conclusion, Germany's economic policies have a significant impact on the European Union's economic stability and growth. While there are some challenges that need to be addressed, Germany's strong economy and high GDP per capita make it an important contributor to the EU's overall economic performance. By encouraging trade and investment, supporting SMEs, addressing labor market challenges, and promoting EU integration, Germany can continue to promote economic stability and growth in the EU.

**Voting Patterns:**

Based on the provided context, it is not possible to analyze the voting patterns of the countries listed. However, it is possible to analyze the voting patterns of the UN General Assembly and the UN Security Council.

The UN General Assembly is a forum for all UN member states to discuss and vote on various issues, including economic development and cooperation. The UN Security Council is a forum for the five permanent members (China, France, Russia, the United Kingdom, and the United States) to discuss and vote on issues related to peace and security.

Based on the provided context, it is not possible to determine the voting patterns of the countries listed. However, it is possible to analyze the voting patterns of the UN General Assembly and the UN Security Council based on the provided context.

**UN Resolutions:**

The provided context includes several UN resolutions related to economic cooperation and development. These resolutions emphasize the importance of promoting economic cooperation and development, particularly in post-conflict countries.

The resolutions also emphasize the importance of addressing the root causes of conflict, including poverty, inequality, and lack of access to basic services. The resolutions also emphasize the importance of promoting peacebuilding efforts, including the establishment of the rule of law, respect for human rights, and management of natural resources.

Based on the analysis, the following recommendations can be made:

1. **Promote economic cooperation and development:** The UN should continue to promote economic cooperation and development, particularly in post-conflict countries.
2. **Address the root causes of conflict:** The UN should address the root causes of conflict, including poverty, inequality, and lack of access to basic services.
3. **Promote peacebuilding efforts:** The UN should promote peacebuilding efforts, including the establishment of the rule of law, respect for human rights, and management of natural resources.

In conclusion, the UN resolutions emphasize the importance of promoting economic cooperation and development, particularly in post-conflict countries. By promoting economic cooperation and development, addressing the root causes of conflict, and promoting peacebuilding efforts, the UN can help to promote economic stability and growth in post-conflict countries."
```

This detailed query process demonstrates the RAG model's functionality:
- **Data Retrieval**: The model retrieves specific socio-economic metrics and resolution texts relevant to Germany from the dataset.
- **Contextual Analysis**: It contextualizes the economic data within the framework of recent UN resolutions that discuss Germany's economic role and initiatives.
- **Insightful Synthesis**: The model synthesizes the information to provide a structured analysis of Germany's economic impact on the EU, considering both internal policies and their alignment with international commitments as outlined in UN resolutions.
- **Recommendations and Forecasts**: It includes strategic recommendations based on the analysis, which are useful for policymakers and analysts studying European economic dynamics.

This example effectively illustrates how the RAG model integrates complex data to generate insightful, accurate, and relevant policy analyses.


This prompt ensures that the model's responses are detailed and focused on providing precise and insightful analysis based on socio-economic data and resolutions. This functionality is central to understanding complex international relations and policy decisions.

## Contributing

Contributions to this project are welcome. Please fork the repository and submit a pull request with your proposed changes or enhancements.

## Acknowledgments

- Data sourced from the UN's digital library and other socio-economic datasets.
- This project uses various Python libraries for data scraping, processing, and visualization, along with advanced AI models for data analysis and response generation.
