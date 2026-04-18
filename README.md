# AI-powered Salesforce Case Intelligence System

An AI-driven case analysis system built within Salesforce that automatically processes incoming support cases and generates structured insights including summaries, priority classification, recommended actions, and customer-ready responses.

This system integrates Salesforce Flow, Apex callouts, and OpenAI APIs to automate case triaging and reduce manual effort in customer support operations.

---

## 🚀 Key Features

- Automatic case analysis on record creation
- AI-generated case summary and classification
- Dynamic priority recommendation (High / Medium / Low)
- Suggested customer response generation
- Next-best action recommendations for support agents
- Seamless integration with Salesforce Case object

---

## 🧠 Architecture

Salesforce Case Created  
→ Record-Triggered Flow  
→ Apex Invocable Action  
→ OpenAI API (via Named Credential)  
→ Structured JSON Response  
→ Case Record Updated with AI Insights  

---

## 🔍 Technical Highlights

- Designed Invocable Apex method to enable Flow-to-AI interaction
- Implemented secure API integration using Named Credentials
- Engineered structured prompts to enforce JSON-based AI responses
- Built robust JSON parsing logic to extract and map AI outputs to Salesforce fields
- Handled asynchronous execution using Flow to avoid UI blocking

---

## 🛠️ Tech Stack

- Salesforce Flow (Record-Triggered Automation)
- Apex (Invocable Methods, HTTP Callouts)
- OpenAI API (LLM Integration)
- Named Credentials (Secure API access)
- JSON Parsing (Structured AI Output Handling)

---

## ⚙️ How It Works

1. A new Case is created in Salesforce
2. Record-triggered Flow executes asynchronously
3. Flow invokes Apex method with case details
4. Apex sends structured prompt to OpenAI
5. AI returns JSON response with:
   - Summary
   - Priority
   - Suggested Response
   - Next Action
6. Flow updates Case fields with AI-generated insights

---

## 📈 Business Impact

- Reduces manual case triaging effort
- Improves response time for support teams
- Standardizes customer communication quality
- Enables scalable AI-assisted support workflows

---

## 📸 Sample Output

<img width="1910" height="858" alt="Screenshot_18-4-2026_213118_capcom3-dev-ed develop lightning force com" src="https://github.com/user-attachments/assets/f73da604-815a-43ef-bdca-b1ced813b77c" />
<br>
<img width="1904" height="910" alt="Screenshot_18-4-2026_215316_capcom3-dev-ed develop lightning force com" src="https://github.com/user-attachments/assets/53e408da-d965-4327-998d-475d6f4c2f59" />

---

## 🔮 Future Improvements

- Retry mechanism for failed API calls
- Confidence scoring for AI responses
- Human-in-the-loop validation
- Multi-language support

