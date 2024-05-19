How to run :

to run install libraries in directory :pip install pandas matplotlib openai yfinance streamlit
pip install pandas matplotlib openai yfinance streamlit
just insert your openai api key in the API_KEY file

Financial Virtual Assistant does following tasks for you :

Functionalities:

Stock Price Retrieval:

Fetches and returns the closing stock price for a specified ticker symbol over the past year by  Calculating Simple Moving Average (SMA)
Computes and returns the Simple Moving Average of a stock's closing price over a specified window of days by Calculating Exponential Moving Average (EMA).
Computes and returns the Exponential Moving Average of a stock's closing price over a specified window of days by Calculating Relative Strength Index (RSI).
Calculates and returns the Relative Strength Index, which measures the speed and change of price movements by Calculating Moving Average Convergence Divergence (MACD).
Computes and returns the MACD, signal line, and MACD histogram, which are used to identify potential buy and sell signals.

Stock Price Plotting:

Plots the closing stock price over the past year and saves the plot as an image file (stock.png).

Streamlit Chatbot Interface:

User Input Handling: Accepts user input via a text input box.
OpenAI ChatCompletion API: Interacts with the OpenAI GPT-3.5-turbo model to process user input and call the appropriate financial function.
Dynamic Image Display: Displays the generated stock price plot image within the Streamlit app.

Financial Data Retrieval and Analysis:

Uses the yfinance library to retrieve historical stock data and perform various financial analyses.

Data Visualization:

Utilizes matplotlib to create and save visual representations of stock prices, which are dynamically displayed in the Streamlit interface.
Chatbot Integration:
Leverages OpenAI's GPT-3.5-turbo model to provide an interactive chatbot experience, responding to user queries with relevant financial data and visualizations.
Session Management:
Maintains a session state to keep track of user messages and responses, ensuring a coherent conversational flow.

Dynamic Function Execution:

Automatically determines and executes the appropriate financial function based on user input, providing real-time financial analysis and insights.

Example Code Flow:

User Input: User enters a query such as "What is the SMA of AAPL for 20 days?".
Message Processing: The user input is appended to the session messages and sent to the OpenAI API.
Function Call Determination: Based on the response from the OpenAI API, the relevant function (e.g., calculate_SMA) is called with the necessary arguments (e.g., ticker symbol and window).
Function Execution: The function computes the requested financial indicator.
Result Display: The result is displayed in the Streamlit app. If a plot is requested, the generated plot image is shown.
