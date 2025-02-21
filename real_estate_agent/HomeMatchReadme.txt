Additional dependencies:
  - pandas 
  - langchain_chroma 
  - langchain_openai 
  - langchain_core


To generate the listing and store the same in Chroma DB, use the function generate_and_store_listings(n_listing). This takes a parameter n_listing which is an integer. The listing generated will be equal to the value of n_listing

To generate a home recommendation, call the function recommend_home(interactive=False). This function takes a parameter interactive. If True, it asks the user to give answers to the questions, otherwise it uses pre-defined answers. The set of question/answer pairs are summarized using an LLM and the summary is passed to the LLM along with the results of semantic similarity from Chroma DB to generate a home recommendation.