# Conglomerate Benchmark V1 Lite

Conglomerate Benchmark V1 Lite is an algorithmically generated benchmark designed to test AI and conversational data analysis tools. It features an ontology with 109 interconnected tables representing a diversified conglomerate business with over 10 subdivisions, including healthcare, medical devices, chemical manufacturing, logistics, CRM, and database tools.

The benchmark includes 18 question-answer pairs covering a broad range of capabilities such as text-to-SQL, Python scripting, data prediction, plotting, and exporting functionalities. The primary challenge for tools evaluated by this benchmark is navigating complex schemas, executing multi-table joins, and effectively managing searches across extensive dimensions and metrics.

This repository contains the publicly available **V1 Lite**, accessible at `/v1/lite/`.

## Tested Tools

Seven enterprise-grade data analysis tools were tested:

- **Ana Enterprise**
- **Ana Small**
- **Deepnote**
- **Amazon Q**
- **Databricks Genie**
- **Hex**
- **Snowflake Cortex**

## Methodology

Due to differences in tool capabilities and intended workflows, scoring was based on each tool's effectiveness in providing accurate answers through their primary interfaces:

- Responses were scored as correct if they produced usable, accurate answers.
- Follow-up interactions were permitted for interactive tools needing additional context.
- Ana Enterprise and Ana Small were evaluated solely on initial responses.

## Results Overview

- **Ana Enterprise:** 91%
- **Ana Small:** 76%
- **Deepnote:** 74%
- **Amazon Q:** 35%
- **Databricks Genie:** 26%
- **Hex:** 21%
- **Snowflake Cortex:** 0% (unable to process datasets exceeding 10 tables or 50 columns)

### Tool-Specific Notes

- **Amazon Q:** Partial credit given when retrieved data led to correct conclusions.
- **Hex and Deepnote:** Scored based on accuracy and practicality of notebook-generated outputs.
- **Snowflake Cortex:** Did not complete benchmark queries due to dataset size constraints.

Complete benchmark details and data can be accessed at `/v1/lite/`.
