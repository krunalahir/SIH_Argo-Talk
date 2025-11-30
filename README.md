🌀 FloatChat – ARGO Ocean Data Discovery & Visualization

AI-Powered Conversational Interface for Oceanographic Insights

FloatChat is an AI-driven system that lets users query, explore, and visualize ARGO float data through natural language.
Ask anything — “Plot salinity at 200m in the Indian Ocean” — and FloatChat handles the data pipeline, retrieval, and visualization automatically.

🚀 Features

	 •	Natural Language Querying of ARGO float datasets
	 •	Automatic NetCDF → SQL / Parquet conversion
	 •	Metadata indexing using FAISS / Chroma
	 •	MCP-based RAG pipeline to transform user queries into executable SQL
	 •	Interactive Streamlit Dashboard with geospatial visualizations
	 •	Chatbot Interface for quick, conversational data exploration
	 •	Supports Indian Ocean ARGO Float Data (extendable globally)

🧠 Tech Stack

	•	Backend: Python, FastAPI (optional), SQL
	•	AI Layer: MCP, LLM-based RAG (FAISS/Chroma), Query Translator
	•	Data Processing: xarray, NetCDF4, Pandas
	•	Dashboard: Streamlit
	•	Visualization: Plotly, Folium, Matplotlib
	•	Storage: SQL / Parquet Format

🧭 System Architecture


User Query → Retrieval → SQL Generation → Data Fetch → Visualization → Response


Pipeline

	1.	User query in plain English
	2.	RAG pipeline embeds query → retrieves the right float metadata
	3.	LLM converts query → SQL
	4.	SQL fetches dataset from processed ARGO storage
	5.	Visualization rendered in Streamlit
	6.	Chatbot returns results + graphs


🌍 Visualizations Supported

	•	Temperature profiles
	•	Salinity profiles
	•	Depth-time cross sections
	•	Float trajectories
	•	Parameter distributions
	•	Region-specific ARGO queries
	•	Custom SQL-to-plot transformation

📈 Future Improvements

	•	Global ARGO dataset integration
	•	On-device ML models for prediction
	•	Drift pattern forecasting
	•	Live float data streaming
	•	Temporal anomaly detection


