### **Annex A**

**Computational Thinking Exercise: "Smart School Canteen Queue"**

**Section: 9-Lithium 	Score:**  
**C# / Name: Jose Marco S. Bassig	Date: 8/6/2026**

**Scenario**

The PSHS school canteen is small and often gets crowded during lunch break. Students line up to buy food, but the process is slow because:

* Some students take too long to decide what to order.  
* The cashier has to manually calculate totals and give change.  
* There is no system to track which food items are running out.

Your group’s task is to **decompose this problem** into smaller, manageable parts that could be solved with computational thinking (CT) Skills.

**Step 1: Identify the Big Problem**

Main Problem: *The main problem is that there are no preparedness for both the staff and students. The students dont know what is on the menu beforehand, nor do the staff have an established POS system.*



**Step 2: Identify three to four Sub-Problems**

Please list possible sub-problems:

1. The cashiers are missing a Point Of Sale (POS) system, making fast lines sluggish and complex orders hard to read.

   

2. The students dont know what are on menu before the line, so they are left to choose on the spot.

   

3. The staff dont have a centralized supply management system, and therefore, cant foresee the input and output of food supplies.

   

**Step 3: Define Computational Thinking Approaches**

For each sub-problem, apply CT skills:

| Sub-Problem | CT Skill | Example Solution |
| ----- | ----- | ----- |
| 1 | Algorithm Design | Design a step-by-step ordering process for a simple POS system: cashier selects item(s) from a pre-loaded menu, the system automatically computes the total and change, then prints or displays the receipt. |
| 2 | Abstraction | Strip away unnecessary details of the full kitchen inventory and show students only what matters to them, a simple digital or printed menu board with item names, prices, and availability, posted before they reach the cashier. |
| 3 | Pattern Recognition | Track daily sales data to notice recurring patterns (e.g., rice runs out fastest during Monday lunches) and use these patterns to predict restocking needs and flag low-supply items automatically. |

 

**Step 4: Draw a flowchart or write a pseudocode for the identified sub-problem**

**Pseudocode for Sub-Problem 1: Point of Sale (POS) System**

```
START
DISPLAY menu items with prices
SET total = 0

WHILE student is still ordering DO
    CASHIER selects item from menu
    IF item is available THEN
        ADD item price to total
        DECREASE item stock by 1
        DISPLAY item added to order
    ELSE
        DISPLAY "Item out of stock"
    END IF
    ASK "Add another item? (Y/N)"
END WHILE

DISPLAY total amount due
CASHIER enters amount paid by student
CALCULATE change = amount paid - total

IF amount paid < total THEN
    DISPLAY "Insufficient payment, please add more"
ELSE
    DISPLAY change due
    PRINT receipt
    IF any item stock <= low-stock threshold THEN
        FLAG item for restocking
    END IF
END IF

END
```

**Flowchart (described in steps, corresponding to the pseudocode above):**

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