# MBA Finance Assistant Chatbot (Dialogflow Essentials) 🏦🤖

An intelligent, conversational AI agent designed to assist users with core financial principles, investment planning, and personal banking utilities. Built using **Dialogflow Essentials (ES)**, this agent parses natural language queries to deliver accurate financial definitions, calculations, and structured advice typical of an MBA corporate finance curriculum.

---

## 🗺️ Chatbot Intent Architecture

The agent architecture, as configured in the Dialogflow console interface, includes a comprehensive suite of financial intents designed to route user queries seamlessly:

* **`Welcome_Finance`:** Greets users and provides a directory of supported features (e.g., investment planning, loan guidance, ratio analysis).
* **`ROI_Intent`:** Explains Return on Investment parameters and outlines foundational math formulas.
* **`EMI_Calculator`:** Outlines Equated Monthly Installment factors such as principal amounts, loan tenures, and changing interest rates.
* **`Credit_Score_Advisor`:** Diagnoses credit score health and categorizes ratings from excellent to poor.
* **`Loan_Advisor`:** Guides users through matching target milestones to credit products (e.g., Home, Education, Auto, or Business Loans).
* **Advanced Metrics (Configured Intents):** Includes `Break_Even_Intent`, `Budgeting_Advice`, `Current_Ratio_Intent`, `Debt_Equity_Intent`, `Insurance_Advisor`, `IRR_Intent`, `NPV_Intent`, and `Tax_Saving_Advisor`.

---

## 💬 Conversational Triggers & Sample Logic

Below are specific conversation simulations mapped directly to the system platform configurations:

### 1. Welcome & Capabilities Discovery
* **User Utterance:** *"Hello Hi Start Finance help I need finance assistance"*
* **Intent Mapped:** `Welcome_Finance`

<img width="1600" height="900" alt="welcome jpg" src="https://github.com/user-attachments/assets/b4b26a05-4428-4be6-bc46-9eb10f1869b1" />


* **Agent Response:** Provides an onboarding menu offering guidance across investment metrics, loan configurations, credit analysis, and financial ratios.

### 2. Return on Investment (ROI) Breakdown
* **User Utterance:** *"Investment Intent"*
* **Intent Mapped:** `ROI_Intent`

<img width="1600" height="900" alt="roi jpg" src="https://github.com/user-attachments/assets/f4bdc394-55a4-4925-9b29-3b3a2c4706c8" />


* **Agent Response:** > ROI means Return on Investment. It shows how much profit you earn from an investment.
  > **Formula:** ROI = (Net Profit / Investment Cost) × 100
  > *Example:* If you invest ₹1,00,000 and earn ₹20,000 profit, ROI is 20%.

### 3. Loan & Credit Structuring
* **User Utterance:** *"Loan Intent"*
* **Intent Mapped:** `Loan_Advisor`

<img width="1600" height="900" alt="loan jpg" src="https://github.com/user-attachments/assets/4c8061e9-37c1-4126-8f6b-4f405eee312f" />


* **Agent Response:** Categorizes loan products by intent (e.g., Buying a house → Home Loan; Higher studies → Education Loan) and prompts the user for monthly income metrics to evaluate basic affordability.

### 4. EMI Computations
* **User Utterance:** *"how to calculate emi"*
* **Intent Mapped:** `EMI_Calculator`

<img width="1600" height="900" alt="emi jpg" src="https://github.com/user-attachments/assets/24c7e680-77b3-4f86-a693-9b33b5f13d21" />


* **Agent Response:** Outlines monthly amortization dynamics. Employs real-world lookup values (e.g., a sample principal of ₹10,00,000 at 9% interest for 10 years maps to an estimated monthly payment of ~₹12,668).

### 5. Credit Score Grading Scales
* **User Utterance:** *"credit score"*
* **Intent Mapped:** `Credit_Score_Advisor`

<img width="1600" height="900" alt="credit jpg" src="https://github.com/user-attachments/assets/033d9bd4-62ee-4aaf-8a4a-ae23d89b8839" />


* **Agent Response:** Returns tier brackets utilized by lending institutions:
  * **Excellent:** 750 and above
  * **Good:** 700 to 749
  * **Average:** 650 to 699
  * **Needs Improvement:** Below 650

---

## 🚀 Deploying & Importing to Dialogflow

To import this agent architecture configuration matrix into your Google Cloud platform:

1. Download the zipped backup archive (`MBAFinanceAssistant.zip`) from this repository.
2. Navigate to the [Dialogflow ES Console](https://dialogflow.cloud.google.com/).
3. Create a clean workspace agent named `MBAFinanceAssistant`.
4. Click the gear icon next to your agent name → select the **Export and Import** settings tab.
5. Choose **Restore from ZIP** and upload the archive package to instantly populate all corresponding intents, training phrases, and default fulfillment parameters.

---

## 📄 License
This conversational design configuration is distributed under the MIT License. See `LICENSE` for more info.
