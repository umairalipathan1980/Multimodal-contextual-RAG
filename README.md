# Multimodal contextual RAG
This code implements Anthropic's contextual retrieval (https://www.anthropic.com/news/contextual-retrieval) with LlamaParse premium mode.  
Instead of chunks as used in Anthropic's blog, this implementation uses nodes which better represent document's structure, semantics, and metadata.  
The parsed files of the uploaded PDF document are in "parsed" folder. For using the RAG with the uploaded parsed files, keep PARSING = 0 in the notebook. At running, specify the name of the folder of the parsed files ("immigrant_stats").  
For parsing new files, store the files in "files2" folder and run the code with 'PARSING = 1'. Specify the name of the output directory at runtime. The new directory will be created in "parsed" folder.  
OpenAI API key is required to run the code with parsed files. For parsing new files, create an account at Llama Cloud and get a free API key for LlamaParse.  
For using Cohere's re-ranker model, get a free API key from Cohere's website. For using the re-ranker, keep the variable 're_ranking = 1' in the code. 
