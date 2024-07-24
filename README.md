# Diet Expert Assistant: RAG-Enhanced Nutritional Guidance

## Introduction

This project presents a Retrieval-Augmented Generation (RAG) chatbot specializing in nutritional advice. Leveraging a comprehensive PDF guide from Dietitian Services at HealthLinkBC, this AI-powered assistant provides accurate, context-aware responses to dietary inquiries.

## Core Technology

The Diet Expert Assistant utilizes cutting-edge natural language processing techniques:

1. **Large Language Model (LLM)**: HuggingFaceH4/zephyr-7b-beta
2. **Embedding Model**: all-MiniLM-L6-v2 sentence transformer
3. **Vector Database**: FAISS for efficient similarity search
4. **User Interface**: Gradio for an intuitive chat experience

## RAG Implementation

Our RAG system enhances the LLM's capabilities by incorporating domain-specific knowledge:

1. **Document Processing**: The HealthLinkBC PDF is parsed and segmented.
2. **Indexing**: Text segments are converted into vector embeddings and indexed.
3. **Retrieval**: User queries trigger a semantic search in the indexed documents.
4. **Augmented Generation**: Retrieved context is combined with the user query for informed LLM responses.

## Key Features

- Real-time nutritional guidance based on HealthLinkBC recommendations
- Dynamic response generation considering both user input and relevant guide sections
- Customizable chat parameters (max tokens, temperature, top-p) for tailored interactions
- Efficient information retrieval from a pre-processed nutritional knowledge base

## Setup and Usage

1. Clone the repository
2. Install dependencies: `pip install -r requirements.txt`
3. Ensure the HealthLinkBC PDF is in the project directory as "Punjabi Diet Expert-pdf.pdf"
4. Launch the application: `python app.py`
5. Interact with the chatbot through your web browser

## Example Queries

The Diet Expert Assistant can address various nutrition-related questions, such as:

- Daily serving recommendations for different food groups
- Portion size guidelines
- Balanced meal planning tips
- Nutritional content of common foods

## Technical Details

- **PDF Processing**: PyMuPDF (fitz) for text extraction
- **Embedding Generation**: SentenceTransformer for creating document and query vectors
- **Vector Similarity Search**: FAISS for rapid retrieval of relevant content
- **Response Generation**: Zephyr-7b-beta model for natural language generation

## Limitations and Ethical Considerations

- The assistant's knowledge is limited to the content of the HealthLinkBC guide
- It should not be considered a substitute for professional medical or nutritional advice
- Users should be aware of potential biases in AI-generated content

## Future Enhancements

- Incorporation of multiple authoritative nutritional sources
- Implementation of multi-modal interactions (e.g., image recognition for food items)
- Regular updates to the knowledge base for the most current dietary guidelines

## Contribution Guidelines

We welcome contributions to improve the Diet Expert Assistant. Please refer to our contribution guidelines for more information on submitting pull requests, reporting issues, or suggesting enhancements.

## Acknowledgments

- Dietitian Services at HealthLinkBC for the comprehensive nutritional guide
- The open-source community for the tools and libraries used in this project

## Contact

For inquiries or feedback, please contact ha4369939@alphacollege.me.

---

Disclaimer: This Diet Expert Assistant is designed for informational purposes only. Always consult with qualified healthcare professionals for personalized nutritional advice.
