# API-INTEGRATION-AND-DATA-VISUALIZATION

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: ALPHIN KINGSLEY S

*INTERN ID*: CTO4DG37

*DOMAIN*: Python programming

*DURATION* : 4 WEEKS

*MENTOR*: NEELA SANTHOSH

DESCRIPTION: User Interface with Streamlit The app uses streamlit to create an interactive web interface. It sets the page layout and title, displays headers, and allows users to interact through dropdowns and data visualizations.

API Integration (Alpha Vantage) The app fetches hourly stock data using the Alpha Vantage TIME_SERIES_INTRADAY API. Users must provide their own API key. Data is retrieved for selected companies like Apple, Microsoft, Google, Amazon, and Tesla.

Stock Selection A multiselect widget allows users to choose one or more stocks to analyze. By default, Apple and Microsoft are selected.

Caching for Efficiency The @st.cache_data decorator caches the fetched stock data for one hour (ttl=3600), reducing unnecessary API calls and improving performance.

Data Processing with Pandas The raw API response is parsed and converted into a structured DataFrame using pandas. It is sorted by timestamp, and the columns are cleaned and converted to appropriate data types.

Data Display The app displays the latest few records of each selected stock in a clean and scrollable data table using st.dataframe().

Data Visualization with Matplotlib & Seaborn

📉 Line Chart: Shows the closing price trend over time for each selected stock using a multi-line chart.

📦 Box Plot: Displays the distribution of closing prices for all selected stocks, allowing users to compare price volatility and spread.

Error Handling & Feedback The app provides visual feedback using st.warning() if no data is available for a particular stock, and st.error() if no data is returned at all. Once the dashboard is ready, it displays a success message.

OUTPUT:

<img width="769" height="835" alt="Image" src="https://github.com/user-attachments/assets/08b4992e-6d67-41f9-b3f4-e52ece38b0af" />
<img width="803" height="882" alt="Image" src="https://github.com/user-attachments/assets/5dba3747-353f-43fe-bd55-88af1832bdd4" />
