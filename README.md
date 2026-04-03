# 📉 E-commerce Sales Funnel Diagnostic

This project analyzes a critical drop-off in the customer journey of an online food delivery platform. Using Python and interactive visualizations, I identified a major failure in the final conversion step.

## 📊 The Business Scenario
The funnel tracks 30,000 visitors through the purchasing process. While the initial engagement is high, the data reveals a catastrophic failure at the very end:

* **Website Visitors**: 30,000 (Baseline)
* **Added to Cart**: 19,589 (~65% conversion)
* **Started Checkout**: 14,694 (~75% from previous step)
* **Payment Window**: 12,586 (~85% from previous step)
* **Completed Order**: **0 (100% Critical Drop-off)**

## 🛠️ Tech Stack
* **Python**: Data structuring and logic.
* **Plotly Graph Objects**: Used to create a specialized Funnel Chart for professional business diagnostics.

## 📈 Visual Analysis
The chart below highlights the steady flow of users until the final "Complete Order" action, where all revenue is lost.

![Sales Funnel Chart](sales_funnel_chart.png)

## 🧐 Diagnostic & Hypotheses
A **0% completion rate** after 12,500+ people reached the payment window is a clear indicator of a **technical blocker** rather than a lack of interest.

### My Hypotheses:
1.  **Critical System Bug**: The "Complete Order" button may have a JavaScript error preventing form submission.
2.  **Payment Gateway Failure**: An API disconnection between the store and the bank/processor.
3.  **UX/UI Blocker**: The final button might be hidden or non-functional on specific mobile browsers.

## 🚀 Recommended Action
I recommend an immediate **Quality Assurance (QA) audit** on the checkout page to fix the code error and recover the lost revenue flow.
