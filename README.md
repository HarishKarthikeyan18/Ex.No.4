
# **Ex.No.4 – Scenario-Based Report Development Utilizing Diverse Prompting Techniques**


### **Aim**

To design an AI-powered chatbot that assists customers in resolving issues related to product troubleshooting, order tracking, and general inquiries. The chatbot should handle various customer queries efficiently while maintaining a conversational and user-friendly tone. In this experiment, we will employ different prompt patterns to guide the development process of the chatbot, ranging from basic task-oriented prompts to more complex, persona-driven prompts.

**Case Study 2** will be analyzed using **Comparative Analysis Prompt, Universal Prompt Structures, Prompt Refinements, and Prompt Size Limitations.**

---

### **Explanation**

Any one use case from **Unit 5** is chosen, and the report is generated using **Unit 2 Prompt Types.**

---

### **Procedure**

1. **Understanding Chatbot Requirements**

   * The chatbot must answer customer FAQs, track orders, provide product recommendations, and handle complaints politely.

2. **Selection of Prompting Techniques**

   * We selected a wide range of prompting techniques — including Zero-shot, Few-shot, Chain-of-Thought, Role Prompting, and others — to cover different aspects of chatbot development.

3. **Prompt Design**

   * For each technique, prompts were specifically designed to handle real-world customer scenarios such as order tracking, damaged item reporting, and delayed delivery.

4. **Experimentation**

   * Each prompting technique was applied to the same scenario to evaluate how the chatbot responded.

5. **Observation and Analysis**

   * The quality, tone, and accuracy of the chatbot’s responses were compared to determine which techniques produced the best customer experience.

6. **Identify Prompt Patterns for Each Design Aspect**

   **Idea Generation Prompts**

   * Prompt: *“What features can be incorporated into the automation system to optimize production and reduce downtime?”*

   **Generated Ideas:**

   * Sensors for real-time monitoring of equipment performance.
   * Predictive maintenance alerts to anticipate equipment failures.
   * Energy usage optimization by automating switching of machines on/off based on demand.
   * Cloud-based dashboards for remote monitoring and control of machinery.

   **Persona and Context Prompts**

   * Prompt: *“What should the user interface and control system convey to the operators and managers?”*

   **Generated Context:**

   * The user interface should be intuitive and provide real-time data on machine performance, energy usage, and alerts.
   * The system should convey reliability and ease of use, with minimal training required for operators.

   **Main Objectives:**

   * Improve production efficiency by 30%.
   * Minimize machinery downtime with predictive maintenance.
   * Enable real-time monitoring and remote control of manufacturing systems.
   * Reduce energy consumption by optimizing processes.

---

### **Prompt Design and Techniques**

1. **Zero-Shot Prompting**

   * Prompt: *“Where is my order #12345?”*
   * **Observation:** The chatbot responded but tone consistency varied. Sometimes the reply was generic or robotic.

2. **One-Shot Prompting**

   * Prompt Example:
     *“Example: Customer asks: Where is my order #98765? → Bot: Your order is out for delivery and will arrive tomorrow. Now answer: Where is my order #12345?”*
   * **Observation:** The chatbot’s response became more aligned with the expected format and tone.

3. **Few-Shot Prompting**

   * Multiple examples were given to set a clear pattern.
   * **Observation:** Improved tone and consistency. Maintained a polite, professional style.

4. **Chain-of-Thought Prompting**

   * Prompt Example:
     *“The customer says they received a damaged item. Think step by step: Apologize, Ask for details, Offer a replacement.”*
   * **Observation:** Responses became structured, covering all steps systematically.

5. **ReAct Prompting**

   * Prompt Example:
     *“Decide if a refund or replacement is more appropriate. Think first, then respond to the customer.”*
   * **Observation:** Worked best for decision-making tasks like returns/refunds.

6. **Self-Consistency Prompting**

   * Generated multiple possible responses, selecting the best.
   * **Observation:** Final response was more balanced and customer-friendly.

7. **Role Prompting**

   * Prompt Example:
     *“You are a polite and empathetic customer service agent. Help the customer track their order.”*
   * **Observation:** Natural, professional, and empathetic replies.

8. **Tree-of-Thought Prompting**

   * Prompt Example:
     *“Generate three ways to resolve a delayed shipment: (1) Apologize and offer a discount, (2) Offer a replacement, (3) Give updated ETA. Choose the best option.”*
   * **Observation:** Creative and customer-focused decision-making.

9. **Reflection Prompting**

   * Prompt Example:
     *“Here’s your answer: . Make it more polite and professional.”*
   * **Observation:** Improved wording and professionalism.

10. **Multimodal Prompting**

    * Example: Uploading a product image and asking: *“Is this available in blue?”*
    * **Observation:** Effective for product-related queries but requires image database.

---

### **Scenario Application**

**Situation:**
A customer reports a **damaged item** and wants a resolution.
We apply two techniques for comparison:

---

#### **Technique 1: Few-Shot Prompting**

**Prompt:**
Classify and respond to customer complaints in a polite, solution-oriented way.

**Examples:**

* Customer: *My order was late.*
  Bot: *I'm really sorry your order was delayed. I have checked and it will reach you today. Thank you for your patience!*

* Customer: *I received the wrong item.*
  Bot: *I apologize for the mix-up! I have initiated a replacement request. You will receive the correct item within 3-4 working days.*

**New Case:**
Customer: *I received a damaged item.*

**Output:**
Bot: *I’m very sorry to hear that your product arrived damaged. I have initiated a replacement request at no extra cost. You will receive the new item within 3-4 working days. Would you like me to arrange a pickup for the damaged product?*

**Observation:**

* Polite, structured, aligned with examples.
* Maintains consistency and professional tone.
* Anticipates customer needs without extra clarification.

---

#### **Technique 2: ReAct Prompting**

**Prompt:**
Customer: *I received a damaged item.*

*Reason step by step:*

1. Identify complaint type (damaged product).
2. Decide refund or replacement (replacement better for customer satisfaction).
3. Respond politely and take action.

**Reasoning:**

* Complaint: Damaged item.
* Resolution: Replacement retains sale & ensures satisfaction.
* Action: Apologize, confirm replacement, arrange pickup.

**Final Response:**
Bot: *I’m sorry to hear your item was damaged. I have arranged a replacement for you at no cost. It will arrive within 3-4 business days. Could you confirm your address for the pickup of the damaged item?*

**Observation:**

* Explains reasoning before answering.
* Provides empathetic, actionable response.
* Balances business needs with customer care.

---

### **Comparative Analysis of Techniques**

| Technique          | Strengths                                 | Weaknesses                            | Best Use Case                        |
| ------------------ | ----------------------------------------- | ------------------------------------- | ------------------------------------ |
| Few-Shot Prompting | Consistent tone, structured replies       | Limited creativity, fixed to examples | FAQs, routine queries                |
| ReAct Prompting    | Adaptive, reasoning-based, customer-first | Slightly longer processing            | Complaints, refunds, decision-making |

---

### **Universal Prompt Structures, Refinements & Size Limitations**

* **Universal Prompt Example:**
  *“You are a polite and empathetic chatbot. A customer reports: \[issue]. Respond with empathy, suggest the best solution, and confirm next steps.”*

* **Refinements:**

  * Few-Shot prompts improved tone consistency.
  * ReAct prompts enhanced reasoning and adaptability.

* **Prompt Size Limitations:**

  * Excessive examples → longer processing times.
  * Concise, well-structured prompts yielded best performance.

---

### **Result**

* Both techniques enhanced chatbot performance compared to Zero-Shot.
* **Few-Shot Prompting**: Best for FAQs and structured, routine queries.
* **ReAct Prompting**: Best for complaints, refunds, or reasoning-heavy queries.
