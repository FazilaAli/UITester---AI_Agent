# 🧪 UI_Agent

AI-powered UI testing agent that compares baseline and new screenshots, analyzes differences using LLM reasoning, and enables intelligent decisions like updating baselines or reporting bugs directly to Jira.

---

## 🚀 Overview

UI_Agent is designed to automate visual regression testing with intelligence.

It compares **new UI screenshots** against **baseline screenshots**, detects changes, and uses an AI model to determine whether the change is expected or a defect.

Based on the analysis, it provides two clear actions:

* ✅ Promote the new screenshot as the updated baseline
* 🐞 Create a detailed Jira bug automatically

---

## ✨ Features

* 📸 Visual comparison between baseline and new UI screenshots
* 🧠 AI-powered analysis of UI differences
* 📊 Generates human-readable test reports
* 🔁 Option to update baseline when UI changes are intentional
* 🐞 Automatic Jira bug creation with:

  * Description
  * Priority
  * Severity
  * Sprint assignment
  * Assignee
* ⚡ Reduces manual effort in visual regression testing

---

## 🧠 How It Works

1. Capture a new UI screenshot
2. Retrieve the corresponding baseline screenshot
3. Perform visual comparison
4. Pass differences to LLM for intelligent analysis
5. Generate a detailed report

### Based on the report, user can:

* **Promote Baseline**

  * Accept the new UI as expected
  * Replace the old baseline screenshot

* **Create Jira Bug**

  * Generate a bug with structured details
  * Include difference context and impact

---

## 🏗️ Architecture

Baseline Screenshot + New Screenshot
→ Visual Comparison
→ AI (LLM) Analysis
→ Report Generation
→ Decision Layer (Promote / Create Bug)

---

## 📌 Example Scenario

**Input:**

* Baseline: Login button (blue)
* New UI: Login button (red)

**AI Analysis:**

* Detects color change
* Evaluates potential UI inconsistency

**Output Options:**

1. Promote new screenshot (if change is expected)
2. Create Jira bug (if change is unintended)

---

## 🎯 Why UI_Agent

Traditional visual testing tools:

* Flag all differences ❌
* Require manual review ❌

UI_Agent:

* Understands context using AI ✅
* Reduces false positives ✅
* Speeds up decision-making ✅
* Integrates directly with Jira ✅

---

## 🛠️ Tech Stack

* n8n
* Visual comparison tools
* AI / LLM-based reasoning
* Jira API
* Screenshot capture tools

---

## ⚠️ Note

This repository is for showcase purposes only.

* Internal workflows are not included
* n8n implementation is abstracted
* Credentials and integrations are omitted
* Proprietary logic is not exposed

---

## 👨‍💻 Author

AI-driven UI testing and automation system using intelligent agents and workflow orchestration.

---

## ⭐ Support

If you find this interesting, consider giving it a star ⭐
