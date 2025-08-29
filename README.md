# ML/AI Use Cases RAG Assistant (Bring Your Own Key)

An AI-powered assistant that provides business advice based on real ML/AI implementations from 60+ companies with 400+ use cases. This app uses Retrieval-Augmented Generation (RAG) to find relevant company examples and provides actionable recommendations. The data are collected from https://github.com/mallahyari/ml-practical-usecases and Google's context_utl is used to extract information and generate the summaries and keywords from the articles describing the use cases.

link to hf space:
https://huggingface.co/spaces/ClaCe/FindHugForPMwithKey

**🔑 Bring Your Own Key:** This version requires users to provide their own HuggingFace API key, ensuring zero cost to the space owner while maintaining full functionality.

## Features

- **🔑 BYOK (Bring Your Own Key)**: Use your own HuggingFace API key for secure, cost-effective access
- **🔍 Semantic Search**: Find relevant ML/AI use cases from a comprehensive database
- **🤖 AI-Powered Advice**: Get personalized recommendations using HuggingFace Inference API
- **📊 Model Recommendations**: Discover fine-tuned and foundation models for your specific use case
- **🏢 Real Company Examples**: Learn from actual implementations across various industries
- **🔒 Privacy-First**: Only embeddings are used - no raw company data is exposed
- **💰 Zero Cost to Owner**: No API costs for the space owner - users bring their own keys

## How It Works

1. **🔑 API Key Setup**: Provide your HuggingFace API key for secure access
2. **📝 Query Processing**: Your business problem is analyzed and converted to embeddings
3. **🔍 Semantic Search**: The system searches through 400+ pre-processed ML use cases
4. **📚 Context Building**: Relevant company examples are selected as context
5. **🤖 AI Generation**: Your API key powers the language model to generate tailored advice
6. **📊 Model Matching**: HuggingFace API provides relevant model recommendations using your key

## Technology Stack

- **Backend**: FastAPI with async support and BYOK architecture
- **Vector Database**: ChromaDB for semantic search
- **Embeddings**: Sentence Transformers (all-MiniLM-L6-v2)
- **Language Model**: HuggingFace Inference API (Gemma 2 2B with fallbacks)
- **Frontend**: Modern HTML/CSS/JavaScript with Tailwind CSS
- **Security**: User API keys never stored, used only for requests

## Security & Privacy

- **🔐 API Key Security**: Your API key is never stored permanently, only used for requests
- **📊 No Raw Data**: Only vector embeddings and metadata are stored
- **🏢 Company Privacy**: Original datasets remain private
- **🛡️ Secure Processing**: All processing happens within the secure HuggingFace environment
- **💾 Local Storage**: API keys stored locally in your browser for convenience

## Getting Started

### 1. Get Your HuggingFace API Key
1. Visit [HuggingFace Settings](https://huggingface.co/settings/tokens)
2. Click "Create new token"
3. Select "Read" access (sufficient for this app)
4. Copy your token (starts with `hf_`)

### 2. Use the Assistant
1. Enter your API key in the secure input field
2. Describe your business problem in natural language:
   - "I want to reduce customer churn in my SaaS business"
   - "How can I implement fraud detection for my e-commerce platform"
   - "What ML approach works best for demand forecasting in retail"

### 3. Get AI-Powered Results
- **Solution Approach**: Detailed technical recommendations
- **Company Examples**: Real implementations from similar businesses
- **Model Recommendations**: Specific HuggingFace models for your use case

## Model Information

This space uses pre-computed ChromaDB embeddings generated from a curated dataset of ML/AI use cases. The language model runs efficiently on CPU with fallback options for reliability.

## Requirements & Limitations

### Requirements
- Valid HuggingFace API key (free to obtain)
- Internet connection for API calls

### Limitations
- Responses are generated based on training data patterns
- Model recommendations are sourced from HuggingFace Hub API
- Processing time may vary based on query complexity and API response times
- API rate limits apply based on your HuggingFace account tier

---

*Built with ❤️ using HuggingFace Spaces*
