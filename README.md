# AI-DATA-ANALYSIS-AGENT
AI Agent Workflow using n8n  This project demonstrates an AI Agent workflow built using n8n to automate tasks, process user inputs, and generate intelligent responses. It showcases workflow automation, AI integration, and the use of connected nodes to build an efficient and functional AI-powered solution.


# AI Agent for Data Analysis using n8n

# EXPLAINATION VIDEO

 **On TELEGRAM BOT (https://drive.google.com/file/d/1qZ4INOArXXT0uN2Xi8Z9uBwcW-HGOwSH/view?usp=drivesdk)**
 **On N8N Agent (https://drive.google.com/file/d/1gUlbgJgwukWvCLjE1hCBwCek3pl3yJbt/view?usp=drivesdk)**

## 📌 Project Overview

This project is an AI-powered Data Analysis Agent built using **n8n**. It accepts a tabular dataset, understands natural-language questions, analyzes the available data using connected tools, and generates answers based on the dataset.

The goal is to make data analysis easier by allowing users to ask questions in plain English instead of manually writing queries or performing calculations.

## 🚀 Features

- **Natural Language Queries:** Ask questions about a dataset using simple English.
- **Data Analysis:** Analyze tabular data and retrieve relevant information.
- **Tool-Based Workflow:** Use n8n workflow nodes and AI Agent tools to process questions and data.
- **Automated Responses:** Generate answers based on the available dataset.
- **CSV and Excel Support:** Prepare tabular data for analysis, depending on the configured workflow.
- **Memory Design (Optional):** Maintain conversational context across multiple questions if memory is configured.

## 🛠️ Tools and Technologies

- **n8n:** Workflow automation and agent orchestration.
- **AI Model / Chat Model:** Understand natural-language questions and generate responses.
- **Data Processing Tools:** Read, filter, calculate, or analyze tabular data through configured nodes or tools.
- **CSV / Excel:** Store structured records for analysis.
- **Webhook (Optional):** Allow an external website or application to send questions to the workflow.

## ⚙️ Setup Instructions

### Prerequisites

Before running the project, make sure you have:

- An n8n account or local n8n installation.
- Access to a supported AI model and its required credentials.
- A sample CSV or Excel dataset.
- The exported n8n workflow JSON file.

### Step 1: Import the Workflow

1. Open your n8n instance.
2. Create a new workflow or open the workflow menu.
3. Import your exported workflow JSON file.
4. Check that all nodes are connected correctly.

### Step 2: Configure Credentials

1. Open the AI Agent or Chat Model node.
2. Configure the required AI provider credentials.
3. Configure any additional credentials required by your workflow.
4. Test the connections before proceeding.

**Security note:** Never upload API keys, passwords, or other secrets to GitHub.

### Step 3: Prepare the Dataset

1. Place your sample dataset in the location or storage service expected by your workflow.
2. Ensure the dataset contains column headers and properly formatted records.
3. Update the relevant file-reading or data-processing node to point to the dataset.

For example, a student dataset might contain:

- Admission Number
- Student Name
- Date of Joining
- Class
- Section
- Recent Test Marks

The actual columns depend on the dataset you configure.

### Step 4: Execute the Workflow

1. Activate the appropriate trigger or start a manual test.
2. Submit a question through the configured input method.
3. Allow the agent to process the dataset using its connected tools.
4. Review the generated answer and verify it against the source data.

### Step 5: Test the Agent

Try questions such as:

- How many records are present in the dataset?
- What is the average test score?
- Which class has the highest average marks?
- Find the record with a particular admission number.
- Summarize the dataset by class or section.

These are example questions. Results depend on the dataset and the tools implemented in the workflow.

## 🧠 Memory Design (If Implemented)

Memory can help the agent understand follow-up questions by retaining relevant conversational context.

For example:

**Question 1:** What is the average score in Class 10?

**Question 2:** Which section has the highest average in that class?

With suitable memory and data-processing configuration, the agent can interpret the second question in the context of the first.

Possible memory approaches include:

- **Conversation Buffer Memory:** Retains recent conversation history.
- **Session-Based Memory:** Separates conversation context between users or sessions.
- **Persistent Memory:** Stores selected information in a database for later retrieval.

Memory should not replace the original dataset or the calculations needed to answer questions accurately. If memory was not implemented, this section describes a possible extension rather than a completed feature.

## 🔄 Workflow Architecture

User Question → Input Trigger → AI Agent → Data Analysis Tool(s) → Result Processing → Final Answer

The exact nodes and connections depend on the exported n8n workflow.

## 📁 Repository Structure

```text
ai-agent-data-analysis/
├── README.md
├── workflow.json
├── data/
│   └── sample_dataset.csv
└── screenshots/
    └── workflow.png
```

This is a suggested structure. Include only files that actually exist in your repository. Avoid uploading confidential or personal student data.

## 🔒 Security and Limitations

- Keep API credentials in n8n credentials or environment variables.
- Use anonymized sample datasets when sharing the project publicly.
- Validate calculations against the source dataset.
- Large datasets may require optimized processing or database integration.
- AI-generated answers can be incorrect; verify important results.
- Memory, webhook access, and Excel processing work only when appropriately configured.

## 🎯 Learning Outcomes

Through this project, I explored:

- Building AI-powered workflows using n8n.
- Connecting language models with tools.
- Processing structured datasets.
- Asking natural-language questions about data.
- Designing automated analysis workflows.
- Exploring conversational memory and context management.

## 👨‍💻 Conclusion

This project demonstrates how an AI agent can combine natural-language understanding, workflow automation, and data-processing tools to simplify data analysis. It also provides a foundation for future improvements, such as persistent memory, database integration, and website-based access.

**Project Status:** Update this section with the features you have implemented and tested.

**Built with n8n and AI-powered data analysis.**
