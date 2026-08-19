### **Annex A**

**Computational Thinking Exercise: "Smart School Canteen Queue"**

**Section: 9-Lithium 	Score:**  
**C# / Name: Jose Marco S. Bassig	Date: 8/6/2026**

**Scenario**

The PSHS school canteen is small and often gets crowded during lunch break. Students line up to buy food, but the process is slow because:

* Some students take too long to decide what to order.  
* The cashier has to manually calculate totals and give change.  
* There is no system to track which food items are running out.

Your group's task is to **decompose this problem** into smaller, manageable parts that could be solved with computational thinking (CT) Skills.

**Step 1: Identify the Big Problem**

Main Problem: *The primary issue pertains to the lack of a POS system. Consequently, students remain uninformed about the menu in advance, and the staff lacks an established procedure for managing these operations effectively.*



**Step 2: Identify three to four Sub-Problems**

Please list possible sub-problems:

1. The absence of a Point Of Sale (POS) system for cashiers results in slow-moving lines and difficulty in processing complex orders.

   

2. Students face the challenge of making quick decisions as they are unaware of the menu options prior to queuing.

   

3. The staff lacks a centralized supply management system, which consequently hinders their ability to anticipate food supplies' input and output.

   

**Step 3: Define Computational Thinking Approaches**

For each sub-problem, apply CT skills:

| Sub-Problem | CT Skill | Example Solution |
| ----- | ----- | ----- |
| 1 | Algorithm Design | In designing a step-by-step ordering process for a simple POS system, the cashier first selects the item(s) from a pre-loaded menu. Subsequently, the system automatically computes the total and change, and finally, it prints or displays the receipt. |
| 2 | Abstraction | Present students with an efficient digital or printed menu board, displaying only essential information such as item names, prices, and availability. This should be showcased before they approach the cashier, removing extraneous kitchen inventory details. |
| 3 | Pattern Recognition | Monitoring daily sales data meticulously can reveal recurring patterns, such as rice depleting most swiftly during Monday lunches. These insights are invaluable for forecasting restocking requirements and automatically identifying items with low supply. |

 

**Step 4: Draw a flowchart or write a pseudocode for the identified sub-problem**

**Flowchart for Sub-Problem 1: Point of Sale (POS) System**

1. **Start**
2. Display menu with prices → 
3. Decision: Is the student still ordering? 
   - **Yes** → Cashier selects an item → Decision: Is item in stock? 
     - **Yes** → Add price to total, reduce stock, show item added → loop back to step 3 
     - **No** → Display "Out of stock" → loop back to step 3 
   - **No** → proceed to step 4
4. Display total amount due
5. Cashier enters payment
6. Decision: Is payment enough? 
   - **No** → Display "Insufficient payment" → return to step 5 
   - **Yes** → Calculate and display change, print receipt
7. Decision: Is stock low for any item? 
   - **Yes** → Flag item for restocking 
   - **No** → skip
8. **End**

**Rubrics For Grading**

**Total Points: 20pts**

Criteria & Levels of Performance

| Criteria | Excellent (4) | Good (3) | Fair (2) | N.I. (1) |
| ----- | ----- | ----- | ----- | ----- |
| **Identification of Sub-Problems** | Identifies 3+ clear, relevant sub-problems that directly connect to the scenario. | Identifies 2–3 mostly relevant sub-problems. | Identifies 1–2 vague or partially relevant sub-problems. | Struggles to identify sub-problems or lists unrelated issues. |
| **Application of CT Strategies** | Correctly applies appropriate CT strategies (abstraction, decomposition, pattern recognition, algorithm design) to each sub-problem with clear reasoning. | Applies CT strategies to most sub-problems, with minor errors or limited explanation. | Applies CT strategies inconsistently, with weak or unclear reasoning. | Rarely applies CT strategies or misuses them. |
| **Flowchart / Pseudocode** X 2 | Flowchart / Pseudocode is complete, logical, and easy to follow; shows clear steps and decision points. | Flowchart / Pseudocode is mostly complete and logical, with minor gaps or unclear steps. | Flowchart / Pseudo Code is partially complete, missing key steps or connections. | Flowchart / Pseudocode is incomplete, confusing, or missing entirely. |
| **Reflection / Explanation** | Provides thoughtful reflection on how decomposition helps problem-solving and identifies CT skills used with strong justification. | Provides adequate reflection with some justification of CT skills. | Provides limited reflection with weak or generic justification. | Provides minimal or no reflection. |
