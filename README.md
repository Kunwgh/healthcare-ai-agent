# HealthChain – Healthcare AI Agent

HealthChain is a Python-based healthcare AI framework that enables AI agents to work with **FHIR/EHR data** using validated and structured healthcare tools.

It combines **LLMs, AI agents, FHIR, MCP, and LangChain** to build healthcare applications that can securely access, process, and work with clinical data.

## 🚀 Features

* 🤖 **AI Agents** – Build LLM-powered healthcare agents
* 🏥 **FHIR Support** – Work with structured healthcare resources
* 🔌 **EHR Integration** – Connect with FHIR-compatible healthcare systems
* 🛠️ **Agent Tools** – Provide validated FHIR tools to AI agents
* 🔗 **MCP Support** – Expose healthcare tools through Model Context Protocol
* 🦜 **LangChain Integration** – Use FHIR tools with LangChain agents
* ✅ **FHIR Validation** – Validate healthcare data before processing
* ⚡ **FastAPI Support** – Build and expose healthcare AI APIs

## 🛠️ Tech Stack

* **Python**
* **LangChain**
* **MCP (Model Context Protocol)**
* **FHIR / EHR**
* **FastAPI**
* **LLMs / Generative AI**
* **Docker**

## 📦 Installation

```bash
pip install healthchain
```

## ⚡ Quick Start

Create a new FHIR Gateway project:

```bash
healthchain new my-app -t fhir-gateway
cd my-app
healthchain serve
```

## 🤖 Using FHIR Tools with an AI Agent

```python
from healthchain.tools import FHIRToolkit

kit = FHIRToolkit(bundle="patient_bundle.json")

# Use with MCP
kit.as_mcp().run()

# Use with LangChain
tools = kit.as_langchain()
```

You can also start the MCP server directly:

```bash
healthchain mcp --bundle patient_bundle.json
```

## 🏥 Example Use Cases

* Healthcare AI assistants
* Patient Q&A systems
* Clinical data analysis
* EHR-integrated AI agents
* FHIR data processing
* Healthcare automation
* AI-powered clinical workflows

## 📚 Documentation

[HealthChain Documentation](https://healthchainai.github.io/HealthChain/)

## 🤝 Contributing

Contributions, ideas, and improvements are welcome. Feel free to open an issue or submit a pull request.

## 📄 License

This project is open source. See the [LICENSE](LICENSE) file for details.
