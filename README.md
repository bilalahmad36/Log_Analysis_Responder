# Log_Analysis_Responder
An AI-powered agent for real-time log analysis and automated security alerts. Built with LangGraph and OpenAI's API.


This project showcases a system for analyzing log files and automating security alerts in real-time. It was developed as a final year project to explore the practical applications of agentic workflows and large language models (LLMs).

The Workflow
The system uses a two-agent architecture built with LangGraph. The process is designed to be simple and efficient:

Classifier Agent: This agent receives a log entry and uses an LLM to classify it as either "critical" or "not critical." It also provides a brief explanation for its decision.

Responder Agent: The responder agent acts based on the classifier's output.

If the log is classified as "critical," the responder immediately sends an email alert with the log details to a designated cyber analyst.

If the log is "not critical," the workflow concludes without further action.

This automation ensures that potential security threats are flagged and communicated instantly, streamlining the work of security teams.

Technologies Used
LangGraph: Used for building the stateful, two-agent workflow.

OpenRouter: Provides access to the Deepseek Chat v3.1 LLM for classification.

Python: The core programming language.

smtplib: The library used to handle email alerts.
