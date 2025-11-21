<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>🍷 Wine Quality Analysis</title>
  <style>
    :root{
      --bg:#0f1724;
      --card:#0b1220;
      --muted:#9aa4b2;
      --accent:#f59e0b;
      --glass: rgba(255,255,255,0.03);
      --radius:14px;
      font-family: Inter, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
      color-scheme: dark;
    }
    html,body{height:100%;margin:0;background:
      linear-gradient(180deg,#071024 0%, #071827 60%); color:#e6eef6;}
    .container{max-width:980px;margin:40px auto;padding:28px;background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));border-radius:var(--radius);box-shadow:0 8px 30px rgba(2,6,23,0.6);}
    header{display:flex;gap:16px;align-items:center;margin-bottom:18px;}
    .emoji{font-size:36px}
    h1{margin:0;font-size:26px;letter-spacing:0.2px}
    p.lead{margin:8px 0 20px;color:var(--muted)}
    section{margin-bottom:18px;padding:14px;border-radius:12px;background:var(--glass);border:1px solid rgba(255,255,255,0.02)}
    h2{margin:0 0 10px;font-size:18px;color:#fff}
    ul{margin:8px 0 0 20px;color:var(--muted)}
    code, .inline-code{background:rgba(255,255,255,0.03);padding:2px 6px;border-radius:6px;font-family:monospace;color:#dbeafe}
    .two-col{display:grid;grid-template-columns:1fr 1fr;gap:12px}
    pre{white-space:pre-wrap;background:rgba(255,255,255,0.02);padding:12px;border-radius:10px;overflow:auto;color:var(--muted);font-family:monospace}
    .footer{font-size:13px;color:var(--muted);margin-top:12px}
    @media (max-width:720px){.two-col{grid-template-columns:1fr}}
  </style>
</head>
<body>
  <div class="container" role="main">
    <header>
      <div class="emoji">🍷</div>
      <div>
        <h1>Wine Quality Analysis</h1>
        <p class="lead">A data analysis and machine learning project based on the Wine Quality dataset. The goal is to explore wine characteristics, understand correlations between features, and build predictive models to classify wine quality.</p>
      </div>
    </header>

    <section aria-labelledby="overview">
      <h2 id="overview">📌 Project Overview</h2>
      <p style="color:var(--muted);margin:6px 0 0;">
        This project involves:
      </p>
      <ul>
        <li>Loading and cleaning the Wine Quality dataset</li>
        <li>Performing Exploratory Data Analysis (EDA)</li>
        <li>Understanding relationships between chemical properties</li>
        <li>Building a machine learning model to predict wine quality</li>
        <li>Evaluating accuracy and performance metrics</li>
      </ul>
      <p style="color:var(--muted);margin-top:10px">It is implemented using a Jupyter Notebook.</p>
    </section>

    <section aria-labelledby="dataset">
      <h2 id="dataset">🗂️ Dataset</h2>
      <p style="color:var(--muted);margin:6px 0 0;">The dataset contains various physicochemical tests of red or white wine, including:</p>
      <ul>
        <li>Fixed acidity</li>
        <li>Volatile acidity</li>
        <li>Citric acid</li>
        <li>Residual sugar</li>
        <li>Chlorides</li>
        <li>Free sulfur dioxide</li>
        <li>Total sulfur dioxide</li>
        <li>Density</li>
        <li>pH</li>
        <li>Sulphates</li>
        <li>Alcohol</li>
        <li>Quality (target)</li>
      </ul>
    </section>

    <section aria-labelledby="eda">
      <h2 id="eda">🔍 Exploratory Data Analysis (EDA)</h2>
      <p style="color:var(--muted);margin:6px 0 0;">In EDA, the following steps were performed:</p>
      <ul>
        <li>Handling missing values</li>
        <li>Summary statistics</li>
        <li>Correlation matrix</li>
        <li>Heatmap to visualize relationships</li>
        <li>Distribution plots of chemical properties</li>
        <li>Boxplots to detect outliers</li>
      </ul>
    </section>

    <section aria-labelledby="models">
      <h2 id="models">🤖 Machine Learning Models Used</h2>
      <p style="color:var(--muted);margin:6px 0 0;">You can mention the ones you implemented:</p>
      <div class="two-col" style="margin-top:8px">
        <div>
          <ul>
            <li>Logistic Regression</li>
            <li>Random Forest Classifier</li>
            <li>Decision Tree</li>
            <li>Support Vector Machine</li>
          </ul>
        </div>
        <div>
          <p style="color:var(--muted);margin:0 0 6px;">Metrics included:</p>
          <ul>
            <li>Accuracy</li>
            <li>Classification Report</li>
            <li>Confusion Matrix</li>
          </ul>
        </div>
      </div>
    </section>

    <section aria-labelledby="results">
      <h2 id="results">📈 Results</h2>
      <p style="color:var(--muted);margin:6px 0 0;">
        The model achieves a good accuracy in predicting wine quality.
        Alcohol, sulphates, and volatile acidity showed strong impact on wine quality.
        (You can edit this based on your exact accuracy.)
      </p>
    </section>

    <section aria-labelledby="tech">
      <h2 id="tech">🛠️ Technologies Used</h2>
      <ul>
        <li>Python</li>
        <li>Pandas</li>
        <li>NumPy</li>
        <li>Matplotlib</li>
        <li>Seaborn</li>
        <li>Scikit-learn</li>
        <li>Jupyter Notebook</li>
      </ul>
    </section>

    <section aria-labelledby="example">
      <h2 id="example">📁 Example Project Structure</h2>
      <pre>
├── wine-quality-analysis.ipynb
├── data/
│   ├── winequality-red.csv
│   └── winequality-white.csv
├── notebooks/
│   └── EDA_and_models.ipynb
├── README.html (this file)
└── requirements.txt
      </pre>
    </section>

    <section aria-labelledby="run">
      <h2 id="run">🚀 How to Run (quick)</h2>
      <ol style="color:var(--muted);margin:6px 0 0 20px">
        <li>Clone the repository</li>
      </ol>
      <pre>git clone &lt;your-repo-url&gt;</pre>
      <ol start="2" style="color:var(--muted);margin:6px 0 0 20px">
        <li>Install dependencies</li>
      </ol>
      <pre>pip install -r requirements.txt</pre>
      <ol start="3" style="color:var(--muted);margin:6px 0 0 20px">
        <li>Open the notebook</li>
      </ol>
      <pre>jupyter notebook</pre>
    </section>

    <div class="footer">
      Tip: Save this as <code>README.html</code> or paste it into your project's GitHub Pages if you want a styled project preview.
    </div>
  </div>
</body>
</html>
