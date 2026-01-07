<div align="center">

[![Hebrew](https://img.shields.io/badge/עברית-Click-blue)](README.md)
[![English](https://img.shields.io/badge/English-Click-yellow)](README_EN.md)
[![Portuguese](https://img.shields.io/badge/Português-Click-green)](README_PT.md)

</div>

# AI Analyzer - Enhancement for n8n-workflows

**Eliad Shahar**, I invite you to evaluate this implementation. As someone who greatly appreciates the work you've put into n8n-workflows, I believe the AI Analyzer adds significant value to the community by making workflows accessible to less technical users and saving time for professionals. I would love to collaborate, receive feedback, and assist in merging these capabilities into your official repository.

*Demo Video: AI Analyzer - Enhancement for n8n-workflows*

[![AI Analyzer Demo](https://img.youtube.com/vi/LGa-HX_uU9U/0.jpg)](https://www.youtube.com/watch?v=LGa-HX_uU9U)

## About
This project introduces **AI Analyzer**, a significant add-on to the excellent original project [n8n-workflows](https://github.com/Zie619/n8n-workflows).
The goal of this add-on is to enrich the user experience by adding an Artificial Intelligence layer that analyzes, explains, and optimizes complex automation workflows.

> **Disclaimer:** This development is an independent improvement and a voluntary initiative submitted for the consideration of the original creator, Eliad Shahar. It is not an official part of the original project until potentially merged.

---

## AI Analyzer Capabilities
The AI Analyzer transforms technical JSON files into clear business insights. Key capabilities include:

*   **Smart Workflow Analysis**: The system "reads" the JSON structure, ignoring generic descriptions and focusing on the actual logic of Nodes and their connections.
*   **Pattern & Anomaly Detection**: Automatic detection of hardcoded values that might trip up users, such as specific Sheet IDs, email addresses, or API keys.
*   **Optimization Suggestions**: AI-driven recommendations for improving workflow efficiency and adapting it to different business needs.
*   **Transparent Integration**: The tool is embedded naturally within the existing User Interface (Workflow Details Modal), requiring no complex external installations.

---

## Advantages & Benefits
The analysis produced by the AI Analyzer comprehensively covers the following points:

*   🎯 **Core Purpose ("Elevator Pitch"):** A concise and focused summary (2 sentences) of the workflow's value and result.
*   ⚡ **Logic Step-by-Step**: A narrative and simple explanation of the flow: Trigger -> Action -> Result, avoiding confusing technical jargon.
*   🛠️ **Configuration Points:** A precise list of nodes requiring manual configuration by the user. For example: "In the 'Gmail' node, change the recipient address to your own."
*   💡 **Real-World Use Cases:** Concrete examples of how the workflow saves time or money.
*   ⚠️ **Prerequisites:** Details on required credentials, API keys, or database columns.
*   🚀 **Customization Tips:** Creative ideas for using the workflow for different business types or alternative integrations (e.g., swapping Slack for WhatsApp).

**Multi-Model & Multi-Language Support:** The system supports various languages (Hebrew, English, Spanish, Russian, etc.) and allows the user to edit the System Prompt to refine results or change the AI persona.

---

## Technical Section & Implementation
*   **Code Structure:** Changes are primarily concentrated in `static/index.html` and associated JavaScript files, where the `WorkflowApp` logic and Prompt interaction are defined. Additionally, new files have been added: `ai_analyzer.py` containing the JSON analysis logic, and `system_prompts.py` which centralizes system instructions for all languages. Also, `.env.example` should be used as a template for environment variable configuration.
*   **Compatibility:** The development was designed to be fully compatible with the original project. It requires no changes to the existing database or Backend server (Python/FastAPI).
*   **Testing:**
    1.  Run the project (`python run.py`).
    2.  Open a browser at the local address.
    3.  Click on any workflow to open the modal.
    4.  Click the "AI Analyzer" button (or select a language) to see the magic happen.
