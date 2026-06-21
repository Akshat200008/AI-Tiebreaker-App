# The Tiebreaker: AI Decision-Making App ⚖️


## 📌 Project Overview
As part of the AI for App Building course by Google on Coursera, I developed "The Tiebreaker," an AI-powered application built directly within Google AI Studio. My primary goal for this project was to design an intuitive tool that helps users navigate complex choices by providing tailored, AI-generated perspectives. To bring this idea to life, I engineered the application to break down everyday dilemmas into actionable insights, allowing users to weigh their options through detailed Pros and Cons lists, Comparison Tables, and comprehensive SWOT analyses.


## 🛠️ Tech Stack & Tools
* **Platform:** Google AI Studio
* **Core Concepts:** Prompt Engineering, Rapid Prototyping, AI-assisted Debugging (Auto-fix)

---

## 🚀 Development Process & Testing

### 1. Defining the Application
I started by utilizing AI Studio's "Build AI apps" feature. Through natural language prompting, I defined the core functionality of the app:
> *"I am envisioning an app named The Tiebreaker designed to assist me in making informed decisions. The app should allow me to input a specific decision I need to make, and in return, it should leverage AI technology to present a comprehensive analysis of various pros and cons associated with each option. This analysis could be displayed in multiple formats to cater to different preferences, such as a detailed pros and cons list, a structured comparison table, or an in-depth SWOT analysis. The goal is to provide a clear and balanced view of the potential outcomes, helping me weigh my choices more effectively."*

<img width="1470" height="791" alt="first ss" src="https://github.com/user-attachments/assets/3dee068a-c5f5-4814-ac30-9094d333db6f" />



### 2. Real-World Scenario Testing
To ensure the model understood the prompt, I tested it with a business-oriented decision:
* **User Input:** *"Should I offer my software for free with paid features, or charge a flat $20/month premium plan?"*
* **Analysis Type:** Pros and Cons List
* **Result:** The AI successfully generated a nuanced breakdown of the freemium vs. premium models.
* **Also gave a final verdict**

### **Freemium Model**
<img width="906" height="614" alt="second ss" src="https://github.com/user-attachments/assets/cf74791d-9b66-4783-9595-3abb6cd29160" />

### **Flat Premium Model**
<img width="915" height="574" alt="third ss" src="https://github.com/user-attachments/assets/9d10be75-d10d-4966-8c95-18db30542d77" />

### **Final Verdict**
<img width="887" height="674" alt="fourth ss " src="https://github.com/user-attachments/assets/6ac0a39b-47d4-4d01-bc83-1728b6bbebf0" />



### 3. Troubleshooting and "Auto-Fix" Implementation
A critical part of modern AI app development is handling edge cases and bugs. During development, the application crashed due to a **React hydration error** caused by invalid HTML structure (specifically, the console flagged a `<form>` element incorrectly nested inside another `<form>`).

Instead of manually digging into the component tree to refactor the code, I utilized Google AI Studio's built-in **Auto-fix** feature to handle the debugging:
* **The Process:** Upon encountering the crash, I triggered the Auto-fix function. The AI model successfully analyzed the error logs and stack trace, identified the DOM conflict, and automatically rewrote the underlying component structure to resolve the nested form issue—all within seconds.

<img width="535" height="589" alt="fifth ss" src="https://github.com/user-attachments/assets/b13d99f8-51ea-415e-9411-65da63497b82" />



### 4. Verification & Format Testing
With the hydration error resolved and the form structure successfully repaired by Auto-fix, it was crucial to verify that the UI was stable and could handle new submissions without crashing. 

I ran a final verification test using an everyday dilemma and a different output format:
* **User Input:** *"What should I eat tonight: Sushi or Chinese food?"*
* **Analysis Type:** Comparison Table
* **Result:** The application handled the form submission flawlessly. It processed the request and successfully formatted the output into a clean, comparative table, proving the Auto-fix patch was completely stable.

<img width="915" height="674" alt="sixth ss" src="https://github.com/user-attachments/assets/88b5fce2-45c4-4f53-9d1f-7fd9bf48aa3f" />



---

## 🧠 Key Takeaways
Building this project reinforced how rapidly functional prototypes can be built using natural language prompts. It also highlighted the importance of built-in AI debugging tools (like Auto-fix) in accelerating the development lifecycle.
