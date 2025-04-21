# Portfolio Optimization & Performance Analysis 

##Part 1: Portfolio Overview 

**Objective**: Achieve **6% annual return** (10-year Treasury +1%) with **moderate risk** (A=4) over a 5-year horizon.  
**Constraints**: Limited withdrawals, liquidity needs, and sectoral diversification.  
**Tools**: Excel and Python for all calcuations and Refinitiv Eikon for data extraction.  

---

## Part 2: Exploratory Data Analysis & Stock Selection  

### (a) 25-Stock Portfolio Construction: 
  - **S&P 500 stocks** (10-year monthly returns up to Dec 2023).  
  - **Sectoral diversification**: 25 stocks across sectors (e.g., Tech, Healthcare, Consumer Staples).  
  - **Low-correlation pairs**: Mitigated unsystematic risk using correlation matrices (e.g., NeWMon & ERIE INDEMNITY: p=-0.077).  

### (b) 15-Stock Portfolio Construction: 
-** Mispriced Stocks identified using CAPM (e.g., Insulet: annualized return 19:02%, α = +3.2%, β = 0.9).

### (c) Key Metrics:  
  | Metric               | 25-Stock Portfolio |
  |----------------------|--------------------|
  | Avg Annual Return     | 18.16%             | 
  | Standard Deviation    | 15.79%             |  
  | Sharpe Ratio          | 0.833              | 
- **Autocorrelation**: Minimal (<0.1 for 95% of stocks), confirming no serial dependency.  

---

## Part 3: Portfolio Construction & Evaluation  

### **(a) Markowitz & Market-Weighted Portfolios**  
1. **Markowitz Optimal Portfolio** (25 stocks):  
   - Maximized Sharpe Ratio (**1.40**) via Solver.  
   
   - **Performance**:  
     - Expected Return: **29.43%**  
     - Risk (SD): **17.43%**
     - Sharpe Ratio: **1.4**  

2. **Market-Weighted Portfolio**(25 stocks):
   - Calculate portfolio based on the Market cap weight 

    - **Performance**:  
     - Expected Return: **20.60%**  
     - Risk (SD): **14.33%**  
     - Sharpe Ratio: **1.254**  

### **(b) Treynor-Black Portfolio**  
- **15 Mispriced Stocks **:  
  - **Active Portfolio Weight**: 196.43% (leveraged).  
  - **Market Portfolio Weight**: -96.43% (short-sold).  
  - **Complete Portfolio**:  
    - **258.35% in Risky Assets**, **-158.35% in Risk-Free Assets**.  

---

## Part 4: Investor Perspectives & Performance  

### **Active vs. Passive Strategies**  
| **Aspect**          | Active Investor (Markowitz/Treynor-Black)      | Passive Investor (Market-Weighted) |  
|----------------------|-----------------------------------------------|------------------------------------|  
| **Goal**             | Outperform market via alpha                   | Match market returns               |  
| **Risk Tolerance**   | High (SD >17%)                                | Moderate (SD ~14%)                 |  
| **Liquidity**        | Low (leveraged/short positions)               | High (low turnover)                |  

### **Performance Evaluation**  
1. **Sharpe Ratio**:  
   - *Markowitz*: **1.40** (Best risk-adjusted returns).  
   - *Market-Weighted*: **1.254** (Balanced).  
    
---
### **Sample Stocks & Refinitiv Codes**  
| **Company**   | **Refinitiv Code** | **Sector**       |  
|---------------|--------------------|------------------|  
| Newmont       | NEM.N              | Technology       |  
| ...           | ...                | ...              |  


----
## How to Check:   
1. **Master Excel File**:  
   - Download from [Google Drive](https://docs.google.com/spreadsheets/d/1ovhuICCpJpxHxPU1dI223FWGqvEFDIc4/edit?usp=drive_link&ouid=115337222374551152231&rtpof=true&sd=true) Please note that access to the Google Drive link is restricted, and you may need to request permission to view the file.
     
2. **Google Colab**:  
   - Click this link to cross check the calcuation from excel[Google Collab](https://colab.research.google.com/drive/1k_CXgJiOEA30eQyVyKsGujJcLALXvVKZ?usp=sharing). 

