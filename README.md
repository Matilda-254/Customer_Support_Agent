This project is a customer support agent designed to automatically categorize customer queries, analyze their sentiment, generate appropriate responses, and escalate negative queries to human agents. The workflow is built using LangGraph, LangChain, and a large language model (LLM) from Groq.

It  demonstrates workflow automation, natural language understanding, and response generation.

Key Components

The project uses the following components:

State Management: TypedDict is used to define and manage the state of each customer query.

Query Categorization: Customer queries are classified as Technical, Billing, or General.

Sentiment Analysis: Determines whether a query has Positive, Neutral, or Negative sentiment.

Response Generation: Produces appropriate responses based on query category and sentiment.

Escalation Mechanism: Queries with negative sentiment are automatically escalated to human agents.

Workflow Graph: LangGraph is used to create a flexible and extensible workflow.

Methods and Workflow

The agent follows these steps to process customer queries:

Environment Setup: Import required libraries and load API keys from .env.

State Definition: Create a structure to hold query, category, sentiment, and response information.

Node Functions: Implement functions for query categorization, sentiment analysis, and response generation.

Graph Construction: Use StateGraph to define workflow nodes and edges representing the support process.

Conditional Routing: Queries are routed based on their category and sentiment.

Workflow Compilation: The graph is compiled into an executable application.

Processing Queries: Queries are passed through the workflow and results are retrieved.
