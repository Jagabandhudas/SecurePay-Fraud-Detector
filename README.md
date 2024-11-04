# SecurePay-Fraud-Detector
<h1>Credit Card Fraud Detection</h1>

<h2>Project Overview</h2>
<p>This project aims to develop a machine learning model to accurately detect fraudulent transactions in credit card data. With the significant financial impact of credit card fraud, identifying these transactions in real time is critical. Using historical transaction data, the model learns patterns of both valid and fraudulent transactions to improve fraud detection accuracy.</p>

<h2>Dataset</h2>
<p>The dataset includes anonymized credit card transactions. Each row represents a transaction, with features like transaction amount, time, and several anonymized variables derived from PCA. The target variable (<code>Class</code>) indicates whether a transaction is fraudulent (1) or valid (0). The dataset is highly imbalanced, with fraudulent transactions making up only a small fraction of entries.</p>

<h3>Key Statistics</h3>
<ul>
    <li><strong>Total Transactions:</strong> 284,807</li>
    <li><strong>Fraudulent Transactions:</strong> 492 (0.172% of data)</li>
    <li><strong>Valid Transactions:</strong> 284,315</li>
</ul>

<h2>Project Workflow</h2>
<ol>
    <li><strong>Data Exploration:</strong>
        <p>Analyzed the dataset to understand variable distributions and class imbalance. Visualized the correlation matrix to identify feature relationships.</p>
    </li>
    <li><strong>Data Preprocessing:</strong>
        <p>Handled any missing values to ensure clean input for the model. Adjusted class distribution to improve fraud detection sensitivity.</p>
    </li>
    <li><strong>Feature Selection:</strong>
        <p>Separated features and target variable, focusing on the attributes contributing most to predictive performance.</p>
    </li>
    <li><strong>Model Training:</strong>
        <p>Implemented a <code>RandomForestClassifier</code> for training, chosen for its effectiveness with imbalanced data. Split the dataset into training and testing sets to evaluate generalization.</p>
    </li>
    <li><strong>Model Evaluation:</strong>
        <p>Evaluated performance using metrics like accuracy, precision, recall, F1 score, and Matthews Correlation Coefficient (MCC). Used a Confusion Matrix to visualize the rates of true positives and negatives.</p>
    </li>
</ol>

<h2>Results</h2>
<ul>
    <li><strong>Accuracy:</strong> High accuracy in distinguishing valid and fraudulent transactions.</li>
    <li><strong>Precision & Recall:</strong> Achieved high recall for fraud detection to minimize false negatives.</li>
    <li><strong>F1 Score:</strong> Balanced precision and recall, indicating a robust model.</li>
</ul>

<h2>Conclusion</h2>
<p>This project demonstrates the effectiveness of machine learning for real-time fraud detection, reducing financial losses. The Random Forest model achieves high accuracy and recall, making it suitable for deployment in environments that require strong fraud detection capabilities.</p>

</body>
</html>
