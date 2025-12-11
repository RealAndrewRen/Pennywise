# Pennywise - A Financial Literacy Large Language Model

### 👥 **Team Members**

**Example:**

| Name             | GitHub Handle | Contribution                                                             |
|------------------|---------------|--------------------------------------------------------------------------|
| Andrew Ren    | @taylornguyen | Data exploration, visualization, overall project coordination            |
| Nailya Alimova   | @jramirez     | Data collection, exploratory data analysis (EDA), dataset documentation  |
| Anjali Amin     | @aminahassan  | Data preprocessing, feature engineering, data validation                 |
| Marvin Hoang      | @pmehta       | Model selection, hyperparameter tuning, model training and optimization  |
| Naisha Mistry       | @naishahmistry    | Model evaluation, performance analysis, results interpretation           |

---

## 🎯 **Project Highlights**

- Developed a machine learning model using a GPT-style transformer fine-tuned with supervised instruction data to address the challenge of building a finance-domain conversational assistant.

- Achieved substantial improvements in domain-specific response quality compared to the base model, demonstrating strong applicability for finance-related support.

- Generated actionable insights by analyzing conversation patterns and user intents, helping inform feature planning and product direction.

- Implemented a structured SFT (Supervised Fine-Tuning) pipeline optimized for small-to-medium datasets, addressing constraints around limited compute and reproducibility expectations.

---

## 👩🏽‍💻 **Setup and Installation**

**Provide step-by-step instructions so someone else can run your code and reproduce your results. Depending on your setup, include:**

* How to clone the repository
* How to install dependencies
* How to set up the environment
* How to access the dataset(s)
* How to run the notebook or scripts

---

## 🏗️ **Project Overview**

**Describe:**

- How this project is connected to the Break Through Tech AI Program
- Your AI Studio host company and the project objective and scope
- The real-world significance of the problem and the potential impact of your work

---

## 📊 **Data Exploration**

**You might consider describing the following (as applicable):**

* The dataset(s) used: origin, format, size, type of data
* Data exploration and preprocessing approaches
* Insights from your Exploratory Data Analysis (EDA)
* Challenges and assumptions when working with the dataset(s)

**Potential visualizations to include:**

* Plots, charts, heatmaps, feature visualizations, sample dataset images

---

## 🧠 **Model Development**

### Base Model Architecture
- Base model: GPT-2 Small (123.65M parameters)
- Rationale: lightweight, fast to train, well-documented for domain adaptation, and ideal for small applications or teaching

### Pre-Training for Domain Adaptation
**Goal: Teach the base GPT-2 model to understand fundamental financial concepts and build general domain knowledge around finance/economics**
- Initialized from the GPT-2 Small (123.65M) pretrained checkpoint
- Trained on the processed financial pre-training datasets mentioned above
- Hyperparameters Tuned
  - Number of training iterations: 6k, 20k, 50k
- Evaluation Metrics
  - Coherence, Accuracy, and Relevance
  - All metrics were measured by manually evaluating responses to the following prompt: “Why can’t we print more money? Because inflation…”

### Supervised Fine-Tuning (SFT)
**Goal: Enable chatbot-style functionality by training the model to provide structured, straightforward, and easy-to-understand answers to personal finance questions**
- Fine-tuned by initializing from the 20k-iteration checkpoint from pre-training
- Trained on the processed SFT datasets mentioned agove
- Hyperparameters Tuned:
  - Number of training iterations: 4.3k, 10k
- Evaluation Metrics
  - Coherence, Accuracy, and Relevance
  - All metrics were measured by manually evaluating responses to the following prompt:  “What are stocks and why should I start trading them?”

---

## 📈 **Results & Key Findings**

### Pre-Training Results


### SFT Results

**You might consider describing the following (as applicable):**

* Performance metrics (e.g., Accuracy, F1 score, RMSE)
* How your model performed
* Insights from evaluating model fairness

**Potential visualizations to include:**

* Confusion matrix, precision-recall curve, feature importance plot, prediction distribution, outputs from fairness or explainability tools

---

## 🚀 **Next Steps**

**You might consider addressing the following (as applicable):**

* What are some of the limitations of your model?
* What would you do differently with more time/resources?
* What additional datasets or techniques would you explore?

---

## 📝 **License**

If applicable, indicate how your project can be used by others by specifying and linking to an open source license type (e.g., MIT, Apache 2.0). Make sure your Challenge Advisor approves of the selected license type.

**Example:**
This project is licensed under the MIT License.

---

## 📄 **References** (Optional but encouraged)

Cite relevant papers, articles, or resources that supported your project.

---

## 🙏 **Acknowledgements** (Optional but encouraged)

Thank your Challenge Advisor, host company representatives, TA, and others who supported your project.
