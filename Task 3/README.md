**Apple Stock Analysis**  
Simple analysis of AAPL historical data. Calculates daily price movements and returns to spot the biggest days.  
**What it does**  
- Loads Apple stock CSV data  
- Calculates daily price change (Close - Open)  
- Calculates daily return percentage  
- Shows top 8 biggest movement days  
**Requirements**  
pip install pandas  
   
**Setup**  
Place your AAPL.csv file in the same directory. Expected format:  
- Date  
- Open  
- Close  
- High  
- Low  
- Volume  
**How to run**  
Just execute the notebook top to bottom. Each cell builds on the last.  
**What you get**  
1. **Dataset load** - checks your data loaded correctly  
2. **Daily Delta** - price difference from open to close  
3. **Top movers** - biggest absolute price swings (in dollars)  
4. **Daily Return %** - percentage change from open to close  
5. **Best performers** - top 8 days by return percentage  
**Output**  
Two tables showing:  
- Biggest dollar moves  
- Biggest percentage moves  
