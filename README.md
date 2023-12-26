# Load  Files from Storage Account into CogSearch 
### The files from Storage Account are loaded into CogSearch by following below steps
- Establish a connection with Storage Account using the Python SDK.
- Retrieve the required files from Storage Account container using the file stream download method.
- Use Azure AI Document Intelligence to parse the PDF files from Storage Account.
- Divide the PDF into smaller, manageable page chunks for easier processing.
- Index the parsed chunks into Azure Cognitive Search.
- Repeat the process for all the required files.

#### Using the Azure Storage Pyhon SDK  to fetch the file stream and use PYPDF and Document Intelligence to chunk the page in memory and create a vector index
- Azure Python SDK https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/storage/azure-storage-blob
- Refer to https://github.com/MSUSAzureAccelerators/Azure-Cognitive-Search-Azure-OpenAI-Accelerator/blob/main/04-Complex-Docs.ipynb for loading large documents using PYPDF and Document Intelligence
