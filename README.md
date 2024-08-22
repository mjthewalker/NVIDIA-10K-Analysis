<div align="center">
  <h1>⚡ Mohnish Hemanth Kumar - 180DC REC</h1>
  <h2>🤖 NVIDIA 10K ANALYSIS(2020-2024) using 🦙 llama 3.1 </h2>
  
</div>
<br/>
<div align="left">
<h1>About the task</h1>
</div>
In this task we will analyze the SEC 10K reports of <a href="https://www.nvidia.com/en-in/">NVIDIA</a> over the last 5 years and derive insights and conclude whether the company grew over the years or not. We will be using the RAG(Retrieval Augmented Generation) approach for this task.
<div align="left">
<h1>Getting the Data</h1>
</div>
We extract the data from <a href="https://www.sec.gov/search-filings">SEC's Official Website</a>  using the API service provided by <a href="https://sec-api.io/">SEC-API</a>. We extract only some sections of the filings in html format.
<div align="left">
<h1>🧹 Data Cleaning</h1>
</div>
We will be using 🦙 <a href="https://docs.llamaindex.ai/en/stable/llama_cloud/llama_parse/">llama parse</a> to parse the data. Since llama parse only accepts pdf files as input we will be converting the html files into pdf. After that we will merge all the parsed data into one single <a href = "https://github.com/mjthewalker/Mohnish_231CS235_ML_WORKFLOW/blob/main/Data/final_parse.md">.MD file.</a>
<div align="left">
<h1>Analysis</h1>
</div>
We will be using RAG approach. We first split the data into small chunks using RecursiveCharacterTextSplitter(), Then we embed the data using 'BAAI/bge-base-en-v1.5' model. We then use qdrant to create a vector database which also contains a vector search engine for RAG. We use flashrankrerank to rerank the data. Finally we will be using llama 3.1 llm with the help of <a href="https://groq.com/">Groq</a> API to derive insights.


<img src='Images/rag-pipeline.png'>
<div align="left">
<h1>📓 Notebook</h1>
</div>
The source code for this task is available <a href="https://github.com/mjthewalker/Mohnish_231CS235_ML_WORKFLOW/blob/main/Notebook/180dc%20(2).ipynb">here</a>
<div align="left">
<h1>Results</h1>
</div>
<div align="left">
<h1>Financial Analysis 1</h1>
</div>
<img src="Images/fa1.jpg">
<img src="Images/fa2.jpg">
<div align="left">
  <div align="left">
<h1>Financial Analysis 2</h1>
</div>
<img src="Images/f1.jpg">
<img src="Images/f2.jpg">
<img src="Images/f3.jpg">
<img src="Images/f4.jpg">
<img src="Images/f5.jpg">

<h1>Visualizations</h1>
</div>
<img src="Images/i5.jpg">
<img src="Images/i9.jpg">
<img src="Images/i6.jpg">
<img src="Images/i7.jpg">
<div align="left">
<h1>Creative Insights</h1>
</div>
<img src="Images/i1.jpg">
