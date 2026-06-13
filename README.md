# 📊 FAIR Cyber Risk Quantification Engine

**[🔴 LIVE DEMO: Click here to run the calculator]([Insert Your Vercel Link Here])**

> **The Elevator Pitch:** > Security teams manage vulnerabilities; businesses manage risk. This tool bridges the gap by translating technical cyber threats into defensible, dollar-value financial metrics. It empowers CISOs to walk into a boardroom and say, *"Spending $50k on this control will reduce our financial exposure by $2.5M,"* backed by industry-standard math.

---

## 🛑 The Problem (Why I Built This)
In traditional security operations (SOC), teams speak in terms of CVE scores, threat actors, and alert volumes. But when you talk to the executive team or the Board of Directors, that language doesn't translate. Executives don't fund "threat mitigation"—they fund **Risk Return on Investment (ROSI)**. 

I built this tool because I saw a disconnect: security teams struggle to get budgets approved because they can't quantify the financial impact of a breach in a way the business understands.

## 💡 The Solution (What It Does)
This application is a lightweight, client-side risk calculator based on the **FAIR (Factor Analysis of Information Risk)** framework. 

Instead of qualitative "Red/Yellow/Green" heatmaps, it uses Monte Carlo simulations to calculate the **Annualized Loss Expectancy (ALE)** of a specific cyber threat. It looks at your organization's revenue, industry benchmarks, and current security controls to output a realistic financial exposure range.

## 🎯 Who Is This For?
* **For GRC & Security Analysts (The Input):** A streamlined interface to map threat scenarios, input organizational context, and audit missing security controls.
* **For CISOs & Executives (The Output):** A clean, bottom-line dashboard showing financial exposure (Inherent vs. Residual risk) and prioritized, ROI-driven treatment recommendations.

## ⚙️ How It Works (Under the Hood)
You don't need a PhD in statistics to use it. The tool simplifies complex risk modeling into four easy steps:

1. **Define the Context:** Input your industry, revenue, and data types (calibrated to the IBM Cost of a Data Breach Report).
2. **Set the Scenario:** Define the threat (e.g., Ransomware) and the assets at risk.
3. **Run the Math:** You input basic estimates (how often a threat might happen, how capable they are, how strong your controls are). Under the hood, the engine runs an 8,000-iteration **Monte Carlo simulation** to calculate thousands of possible outcomes, giving you a highly accurate estimate of potential financial loss.
4. **Get Actionable Results:** The tool outputs a dashboard that tells you:
   * How much risk you have *before* controls (Inherent).
   * How much risk you have *with* controls (Residual).
   * **Where to invest next:** It ranks missing controls based on how much financial loss they prevent versus how much they cost to implement.

## 📈 The Business Impact (How It Helps)
* **Defensible Budgets:** Replaces guesswork with mathematical modeling.
* **Strategic Alignment:** Maps directly to NIST CSF, ISO 27001, and CIS controls so you can see exactly where your compliance gaps are causing financial exposure.
* **Clear Risk Treatment:** Automatically recommends whether the business should **Accept, Mitigate, Transfer (Cyber Insurance), or Avoid** the risk based on the organization's predefined financial appetite.

## 🛠️ Technical Stack
Designed to be fast, serverless, and entirely client-side:
* **Frontend UI:** HTML5, CSS3
* **Risk Engine:** Vanilla JavaScript (Custom Monte Carlo / Beta-PERT Simulation Engine)
* **Data Visualization:** Custom SVG charting for Loss Exceedance Curves (LEC)
* **Deployment:** Vercel / GitHub Pages

---
*Built as a portfolio project to demonstrate the transition from operational security to strategic, business-aligned Governance, Risk, and Compliance (GRC).*
