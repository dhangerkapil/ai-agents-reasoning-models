## Azure AI Agent Service Enterprise Demo Changelog

<a name="1.1"></a>
# 1.1 (2025-02-08)

**Features / Enhancements**  
- **Optional Direct Azure AI Search Integration**  
  - Thanks to [@farzad528](https://github.com/farzad528) for adding a feature that allows direct Azure AI Search usage alongside the existing vector store approach.  
  - The notebook logic now checks if a `FileSearchTool` is present; if not, it configures Azure AI Search using `AZURE_SEARCH_CONNECTION_NAME` and `AZURE_SEARCH_INDEX_NAME` from your `.env`.  
- **Logic App Integration for `send_email`**  
  - Replaced the local/mocked `send_email` function with an HTTP call to a Logic App.  
  - Added a `LOGIC_APP_SEND_EMAIL_URL` parameter to `.env.example`, along with instructions and an ARM template (`send_email_logic_app.template.json`) for deploying the Logic App.  
- **Environment Configuration Updates**  
  - Revised `.env.example` to unify all optional parameters (Bing, Logic App, Azure Search, etc.) in one place.  
  - README now describes how to set these environment variables and clarifies how each integration (Bing, Logic App, Azure AI Search) is triggered.

**Bug Fixes**  
- **Correction of swapped OpenWeather parameters**  
  - Thanks to [@gerbermarco](https://github.com/gerbermarco) for fixing the `OPENWEATHER_ONE_API_KEY` and `OPENWEATHER_GEO_API_KEY` variable values in `.env.example`.

**Breaking Changes**  
- None.

---

<a name="1.0"></a>
# 1.0 (2025-01-27)

**Features**  
- Initial release of an enterprise-grade streaming agent built on [Azure AI Agent Service](https://learn.microsoft.com/azure/ai-services/agents/).  
- Demonstrates programmatic creation or reuse of an agent model (e.g., GPT-4o).  
- Integrates local enterprise data (HR, PTO, policy files) into a vector store for retrieval-augmented generation (RAG).  
- Offers optional Bing grounding and custom Python functions (e.g. weather, stock lookup, email sending).  
- Shows how to stream partial responses and tool calls in real-time.  
- Includes a [Gradio](https://github.com/gradio-app/gradio) interface for interactive demos.  

*Bug Fixes*  
_None_

*Breaking Changes*  
_None_
