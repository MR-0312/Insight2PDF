# Insight2PDF

## Project Overview

This repository contains the development of a sophisticated chatbot designed to answer questions based on content extracted from PDF documents. The project leverages advanced natural language processing (NLP) techniques and is implemented using a combination of various modern technologies such as TypeScript, Docker, Supabase, and NLP frameworks including OpenAI and Huggingface APIs.

## Objectives

- Develop a chatbot capable of interacting with PDF content to provide accurate answers.
- Utilize advanced NLP models to interpret and process textual data.
- Implement robust backend services using Supabase for efficient data management.
- Ensure seamless deployment and integration using Docker and ngrok.

## Core Elements

### Database Tables

- **audit_urls**: Manages URLs subject to auditing.
- **audits**: Stores audit information including metadata like name and market cap.
- **audits_data**: Keeps detailed audit data such as scores and dates.
- **pdf_image_embeddings**: Contains embeddings generated from images extracted from PDFs.
- **pdf_text_embeddings**: Stores text chunks extracted from PDF documents along with their embeddings.

### Triggers

- **trigger_process_audit_url**: Triggered after inserting a new record into the audit_urls table.
- **trigger_process_audit_url_update**: Triggered before updating a record in the audit_urls table.
- **trigger_process_audits**: Triggered after inserting a new record into the audits table.

### Edge Functions

- **get_audits_pages**: Fetches pages of audit information from a base URL.
- **get_audits**: Retrieves specific audit data from a URL.
- **get_audits_data**: Fetches detailed audit data from a URL.

### Flask PDF Processing MicroService

- Extracts textual and graphical content from PDFs.
- Stores the extracted content in Supabase.
- Uses tools like Sentence Transformers and ResNet50 for text interpretation and image detail extraction.

## Weekly Reports

### Week 1 (09/05/2024 - 18/05/2024)

**Work Done:**

- Learned data scraping techniques.
- Studied Supabase as a backend service.
- Developed an NLP model using Langchain for database search.
- Integrated the model with Supabase.
- Learned about embeddings and stored them in Supabase using PG vector.
- Developed a model to search similar images from input images or text.

**Challenges:**

- Encountered a dimension error during the image search process.

**Plans:**

- Resolve the dimension error.
- Conduct testing and debugging.
- Further study embeddings to improve model performance.

### Week 2 (20/05/2024 - 25/05/2024)

**Work Done:**

- Learned about embeddings and their storage in Supabase.
- Stored images and text embeddings.
- Created a model for image search.
- Developed a UI for the chatbot.
- Used OpenAI and Huggingface APIs to convert text into embeddings for PDF-based Q&A.

**Challenges:**

- Model failed in searching due to a dimension error.

**Plans:**

- Improve the model for better image retrieval.
- Optimize the model for efficient token usage.
- Conduct extensive testing.

### Week 3 (27/05/2024 - 01/06/2024)

**Work Done:**

- Learned TypeScript for static typing in JavaScript.
- Gained knowledge on edge functions in Supabase.
- Created and deployed an edge function for web scraping.
- Explored use cases for edge functions.

**Plans:**

- Develop additional edge functions.
- Create an NLP/LLM model for PDF interaction via chat.

### Week 4 (03/06/2024 - 08/06/2024)

**Work Done:**

- Tested edge functions deployed on Supabase.
- Learned about ngrok and Docker for deployment.
- Written project documentation.

**Plans:**

- None specified.

## Technologies Used

- **Programming Languages**: TypeScript, Python
- **Frameworks and Libraries**: Langchain, OpenAI API, Huggingface API
- **Backend Services**: Supabase
- **Deployment Tools**: Docker, ngrok

## References

- [TypeScript Documentation](https://www.typescriptlang.org/docs/)
- [Supabase Documentation](https://supabase.io/docs)
- [PG Vector Documentation](https://github.com/memgraph/pgvector)
- [OpenAI API Documentation](https://beta.openai.com/docs/)
- [Huggingface API Documentation](https://huggingface.co/docs)
- [Ngrok Documentation](https://ngrok.com/docs)
- [Docker Documentation](https://docs.docker.com/)

## Author

**Meet Sureshbhai Radadiya**  
Student ID: 22AIML042
