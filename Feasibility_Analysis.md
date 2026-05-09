# Clinic Management System: Feasibility Analysis – Cost-Benefit Analysis

This analysis assumes a **Custom Build** approach for an MVP covering Patient Records, Appointment Management, and Billing modules.

## Assumptions
*   **Initial Investment (Year 0):** 500,000 EGP (Development, Discovery, Infrastructure)
*   **Annual Operating Cost (Years 1–5):** 100,000 EGP (Maintenance, Hosting, Support)
*   **Expected Annual Benefits:** Growing as adoption increases.
*   **Discount Rate:** 10% (for Present Value calculations).

## 1. Cash Flow & Break-Even Analysis (Non-discounted)

| Year | Benefits (EGP) | Total Costs (EGP) | Net Cash Flow (EGP) | Cumulative Cash Flow |
| :--- | :--- | :--- | :--- | :--- |
| **0** | 0 | 500,000 | (500,000) | (500,000) |
| **1** | 200,000 | 100,000 | 100,000 | (400,000) |
| **2** | 250,000 | 100,000 | 150,000 | (250,000) |
| **3** | 300,000 | 100,000 | 200,000 | (50,000) |
| **4** | 350,000 | 100,000 | 250,000 | 200,000 |
| **5** | 400,000 | 100,000 | 300,000 | 500,000 |

### Calculations
1.  **Break-Even Year**: Occurs in Year 4.
2.  **Exact Break-Even Point**:
    *   Remaining after Year 3: 50,000
    *   Year 4 inflow: 250,000
    *   Calculation: $3 + (50,000 / 250,000) = 3.2 \text{ years}$.
3.  **Total ROI (after 5 years)**:
    *   Total Benefits: 1,500,000
    *   Total Costs: 1,000,000 (500k dev + 500k op)
    *   Net Profit: 500,000
    *   $ROI = (500,000 / 1,000,000) \times 100 = 50\%$.

## 2. Net Present Value (NPV) Analysis (Discounted)

*Discount Rate = 10%*

| Year | Net Benefit (EGP) | Discount Factor | Present Value (PV) |
| :--- | :--- | :--- | :--- |
| **0** | (500,000) | 1.0000 | (500,000) |
| **1** | 100,000 | 0.9091 | 90,910 |
| **2** | 150,000 | 0.8264 | 123,960 |
| **3** | 200,000 | 0.7513 | 150,260 |
| **4** | 250,000 | 0.6830 | 170,750 |
| **5** | 300,000 | 0.6209 | 186,270 |
| **Total** | | | **222,150** |

### Decision Criterion
*   **NPV**: 222,150 EGP
*   **Decision**: **Accept**. Since the NPV is positive (> 0), the project is financially viable and adds value to the clinic over the 5-year period.

## 3. Summary of Findings

| Metric | Result |
| :--- | :--- |
| **Payback Period** | 3.2 Years |
| **5-Year ROI** | 50% |
| **Net Present Value** | 222,150 EGP |

---

## Appendix: Understanding Cash Flow Analysis
*Example: Inventory Management System breakdown.*

### 1. The Outflow: Investment & Costs
*   **Year 0 (CapEx - Capital Expenditure):** Money spent to create the foundation.
    *   **Hardware/Software:** The physical infrastructure and development costs to launch the system.
    *   **Training:** An essential cost to ensure staff can use the system efficiently.
*   **Years 1–3 (OpEx - Operational Expenditure):** Ongoing costs required to keep the system operational.
    *   **Maintenance:** Hosting, bug fixes, updates, and support to ensure system reliability.

### 2. The Inflow: Operational Benefits
*   **Savings:** Benefits are not always new cash; they are often **savings**.
    *   **Labor Savings:** Automating manual tasks saves employee time, allowing them to focus on revenue-generating activities.
    *   **Loss Reduction:** Tracking inventory automatically prevents theft or waste.
*   **Why Benefits Grow:** As staff adoption increases and system processes are refined over time, the system becomes more efficient, leading to increased annual savings.

### 3. The Flow Logic: Net & Cumulative
*   **Net Cash Flow (NCF):** The profit or loss in a specific year (`Total Benefits - Total Costs`).
*   **Cumulative Net Cash Flow:** The "Running Total" that tracks your initial investment. It tells you exactly when the project has fully paid for itself (the Break-Even Point). If the cumulative figure is negative, you are still recovering the initial investment.
