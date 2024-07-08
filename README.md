# Langgraph

Langgraph is a sophisticated language model graph that utilizes three specialized language models to answer diverse queries in the domains of economy, sports, and general knowledge. This project demonstrates how to route questions to the appropriate specialized models to provide accurate and context-specific answers.

## Overview

The following diagram illustrates the architecture of Langgraph:

![image](https://github.com/Sghosh1999/LangGraph-MultiAgent-Routing/assets/44112345/f71caa6f-d65f-4c90-a38f-20aeee1920e1)


### Explanation of Graph Nodes

1. **Economy LLM:**
   - **Function:** This agent is tailored to handle queries related to economic news, trends, market analysis, financial reports, and other economic-related information.
   - **Specialization:** The Economy LLM is trained on a wide array of economic data, ensuring accurate and up-to-date responses for any economic inquiry.

2. **Sports LLM:**
   - **Function:** This agent focuses on queries related to sports, including live scores, player statistics, game results, and sports news.
   - **Specialization:** The Sports LLM is optimized with extensive sports data, making it the go-to model for any sports-related questions.

3. **General LLM:**
   - **Function:** This agent addresses general questions that do not specifically pertain to economy or sports. It covers a broad range of topics and provides versatile answers.
   - **Specialization:** The General LLM is trained on diverse datasets, ensuring comprehensive and accurate responses for a variety of general queries.

## How It Works

1. **Start Node:**
   - The process begins at the start node, where the user submits a query.
   
2. **Agent Node:**
   - The agent node routes the query to the appropriate specialized LLM based on the query's content and domain.
   
3. **LLM Call Nodes:**
   - Depending on the query, the agent directs the call to one of the three LLMs (Economy, Sports, or General) to obtain the most accurate and relevant answer.

4. **End Node:**
   - The response from the selected LLM is then sent to the end node, where it is delivered back to the user.
