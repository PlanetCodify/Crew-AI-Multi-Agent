# Crew-AI-Multi-Agent

## Agent Creation for Contract Analysis Workflow

### Purpose

This Python script defines a function, `create_agents`, which initializes three specialized AI agents designed to process and analyze contract data. Each agent has a unique role in the workflow, equipped with specific tools, goals, and memory capabilities.

---

### Agents Created

1. **PDF Data Extractor Agent**:
   - **Role**: `PDF Data Extractor`
   - **Goal**: Extract key contract terms from PDF files.
   - **Backstory**: An expert in identifying and extracting important contractual information from PDFs.
   - **Tools Used**: `PdfReadTool` for processing PDF content.
   - **Memory**: Enabled for maintaining context during task execution.
   - **LLM**: Uses `ChatOpenAI` with a temperature of 0.7 and the `gpt-4` model for generating context-aware responses.

2. **Data Comparison Analyst Agent**:
   - **Role**: `Data Comparison Analyst`
   - **Goal**: Compare the extracted contract terms against predefined reference values.
   - **Backstory**: A specialist in analyzing and validating contract data for accuracy.
   - **Tools Used**: `ReferenceDataTool` for accessing the standard reference data.
   - **Memory**: Enabled for maintaining contextual continuity during analysis.
   - **LLM**: Utilizes `ChatOpenAI` with a temperature of 0.7 and the `gpt-4` model.

3. **Compliance Report Generator Agent**:
   - **Role**: `Compliance Report Generator`
   - **Goal**: Generate a detailed compliance report highlighting deviations in contract terms.
   - **Backstory**: An expert in drafting compliance documentation based on contract analysis.
   - **Tools Used**: `ReferenceDataTool` for retrieving reference values for comparison.
   - **Memory**: Enabled for efficient report creation and historical context.
   - **LLM**: Powered by `ChatOpenAI` with a temperature of 0.7 and the `gpt-4` model.

---

### Key Features

- **Role Definitions**: Each agent is assigned a distinct role with a clear goal and relevant tools to perform specific tasks in the contract analysis process.
- **Backstory**: Provides a narrative for each agent, enhancing its contextual and operational understanding.
- **Memory**: Ensures that agents can retain and use context throughout their task execution.
- **Tools Integration**: Associates each agent with the necessary tools (`PdfReadTool` or `ReferenceDataTool`) to perform their tasks effectively.
- **Verbose Mode**: Enabled for detailed logging of each agent's operations.
- **Interactive Display**: Utilizes `boxen` to display formatted profiles for each agent, making their roles and goals visually clear.

---

### Workflow

1. **Initialization**: 
   - The `create_agents` function initializes and configures the three agents.
2. **Display Profiles**:
   - Each agent's profile (role, goal, and backstory) is printed in a visually styled box for clarity.
3. **Return Agents**:
   - Returns the three agents: `researcher_agent`, `writer_agent`, and `review_agent` for further use in the workflow.

---

### Example Use Case

This setup is ideal for automating the following contract analysis workflow:
1. Extract terms from a contract using the **PDF Data Extractor Agent**.
2. Validate and compare the terms with predefined reference values using the **Data Comparison Analyst Agent**.
3. Generate a compliance report highlighting any deviations using the **Compliance Report Generator Agent**.
   
## <img width="1453" alt="Screenshot 2025-02-25 at 5 04 20 PM" src="https://github.com/user-attachments/assets/a0d4fe2c-d10c-4a30-8be2-3a018ea31808" />

## <img width="1453" alt="Screenshot 2025-02-25 at 5 05 39 PM" src="https://github.com/user-attachments/assets/d42a0d33-c20e-4a7b-9885-8d7198cf4d31" />


