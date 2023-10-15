# Current Plan (Will Update readme with full report later on)
## Salient Features
1. Reads PDFs and stores them by paragraphs in db.
2. Uses Vector Indexes to gather sentence embeddings.
3. Takes in query and gets top 10 paragraphs with highest similarity score.
	a. User can change limit for number of relevant paragraphs
	b. And it then outputs the documents in order of highest similarity (calculated as average of 		    similarity score for all paragraphs). Use queries to consolidate the documents.
	c. This is the most basic implementation as needed.
Now we talk about additional features which we can add:
4. Use ChatGPT to summarize the relevant paragraphs for the user, so that they can also get summary for their query.
5. Use different Sentence Feature Extractor through different model (probably OpenAI) and qualitatively compare the output.
6. Use ChatGPT or GPT4All to also summarize the documents in 1 line for the user and store in MyPDFs. If user asks for summary, just output the summary of all documents.

## Additional Details
Will think if we can add more features like document clustering and more advanced queries like “Tell me about spring in context of computer science”, this will only get results from documents clustered under computer science and give info about spring framework for Java. Or “Tell me about spring in context of nature”, this will get results documents clustered under nature and give info about the spring season. Otherwise this can be taken up in Project 2.