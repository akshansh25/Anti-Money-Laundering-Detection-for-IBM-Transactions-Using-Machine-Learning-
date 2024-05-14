# Anti-Money-Laundering-Detection-for-IBM-Transactions-Using-Machine-Learning-
The dataset is from Kaggle :

https://www.kaggle.com/datasets/ealtman2019/ibm-transactions-for-anti-money-laundering-aml

**Data Preparation & Feature Engineering:**

Data from transactions is merged, cleaned, and preprocessed. Features like account information and transaction details are extracted and transformed for analysis. 

**Model Building & Evaluation:**

Machine learning models are trained on historical data to identify suspicious transactions. These models are then evaluated for accuracy and effectiveness. 

**Data Standardization and Feature Engineering:**

1)Utilized ‘pd.options.display.float_format’ to standardize Money columns like Amount Received and Amount Paid,
Features like account information and transaction details are extracted and transformed for analysis.

2)Label encoding categorical columns with sklearn label encoder.

3)Combined ‘From Bank’ and ‘Account’ column to create unique identifiers.

4)Created a function which prepares the data by extracting relevant account and bank information.

**Node Feature**

1)The feature performs data preprocessing on financial transaction data by calculating average paid and received amounts for each currency per account, encoding categorical bank names, and normalizing numerical attributes.

2)These processed data can be further used for tasks such as fraud detection or network analysis in financial systems.

**Edge Feature**

1)The use of the edge feature is to provide additional information or attributes associated with the transaction (edges ) in the graph.

2)These features includes transaction amounts, timestamp, or any other relevant information that might help in analyzing patterns in the transactions.

3)By using this feature machine learning models can better understand the relationship between accounts and help identifying suspicious transaction.

**Model Architecture**

1)We defined Graph Attention Network (GAT) model using PyTorch and PyTorch Gemoetry.

2)This GAT model is designed to process graph-structured data with node features and edge features.

3)It leverages attention mechanism to capture the relationship between nodes in the graph and produce node-level predictions.

**Model Training and accuracy**

1)Here we used GAT model, which is a type of graph neural network (GNN).

2)The accuracy metrics reaching more than 90% indicates that the percentage of correctly predicted labels in the validation set increases over epochs, which suggests that the model is making accurate prediction on validation data.

**References**

Anti Money Laundering Detection with GNN for IBM Transactions. ISSAC CHAN

https://www.kaggle.com/code/issacchanjj/anti-money-laundering-detection-with-gnn

**Some other references regarding Anti Money Laundering and crypto currency for laundering**

Financial Crimes Enforcement Network. What is money laundering?

https://www.fincen.gov/what-money-laundering#:~:text=Money%20laundering%20involves%20disguising%20financial,with%20an%20apparently%20legal%20source.

United Nations Office on Drugs and Crime (UNODC). (2023). ANTI-MONEY LAUNDERING AND COMBATING THE FINANCING OF TERRORISM (AML/CFT)

https://www.imf.org/en/Topics/Financial-Integrity/amlcft

IDnow. How criminals leverage non-compliant crypto exchanges for money laundering.

https://www.idnow.io/blog/how-criminals-leverage-crypto-money-laundering/#:~:text=Thanks%20to%20weak%20AML%20and,(government%2Dissued%20currency).













