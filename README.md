# 🎧 Spotify Data Pipeline: End-to-End with AWS

This project demonstrates the creation of a complete data engineering pipeline using Spotify's API and AWS technologies. The pipeline extracts music-related data, transforms it, and loads it into an AWS-based data warehouse for analysis and insights. This project showcases how modern data engineering practices can be applied to build scalable and efficient data pipelines.

## 🌟 Project Overview

The primary goal of this project is to create an automated pipeline that fetches data from Spotify’s API, processes it, and stores it in an AWS data warehouse for analysis. By leveraging cloud technologies, the project demonstrates how data from a music streaming platform can be efficiently ingested, transformed, and visualized for actionable insights.

## 🛠️ Key Features

- **Data Extraction**: Uses Spotify’s API to fetch real-time data on music tracks, albums, artists, and user activity.
- **Data Transformation**: Python scripts are employed to clean, process, and structure the raw data.
- **Data Loading**: Transformed data is loaded into AWS S3 as a staging area and then processed further using AWS Glue.
- **Data Warehouse**: Final data is stored in AWS Athena for efficient querying and analysis.
- **Dashboarding**: Insights and visualizations are generated using popular BI tools.

## 🧰 Technology Stack

- **Programming Language**: Python  
- **Cloud Platform**: AWS
  - **S3**: Data storage for raw and processed data
  - **Lambda**: Serverless functions to automate data extraction and processing
  - **Glue**: Managed ETL service for data transformation
  - **Athena**: Data warehouse for querying processed data
- **API**: Spotify API for data retrieval
- **Data Pipeline Orchestration**: Scheduled using AWS Lambda and Glue

## 🗂️ Project Architecture

<p align="center">
  <img src="https://github.com/Prajwal0105/spotify-end-to-end-data-engineering-project/blob/main/architecture.png" alt="Project Architecture" width="80%" />
</p>

The project follows a simple yet scalable architecture:

1. **Data Ingestion**: Spotify API data is ingested and stored in AWS S3 (raw format).
2. **Data Transformation**: Python scripts running on AWS Lambda clean and process the raw data.
3. **ETL Processing**: AWS Glue is used to further transform the data and load it into a structured format.
4. **Data Warehousing**: Processed data is stored in AWS Athena, where it can be queried and analyzed.
5. **Visualization**: Insights are visualized through BI tools connected to Athena.

## 📊 Dataset and Data Sources

Data is fetched directly from Spotify’s public API, which provides comprehensive information about:

- **Tracks**: Song metadata, popularity, and streaming metrics.
- **Artists**: Artist details, follower count, and genres.
- **Albums**: Album releases, tracks, and related metadata.
- **User Activity**: Streaming habits, playlists, and interactions.

## 🚀 Setup Instructions

Follow these steps to set up and run the project:

### 1. Clone the Repository

```bash
git clone https://github.com/Prajwal0105/spotify-end-to-end-data-engineering-project.git
cd spotify-end-to-end-data-engineering-project
```

### 2. Set Up AWS

- Create an S3 bucket to store raw and processed data.
- Set up AWS Glue for ETL jobs.
- Configure AWS Lambda for automated data extraction.

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure API Access

- Create a Spotify Developer account and generate API keys.
- Store your Spotify API keys in a `.env` file:

```bash
SPOTIFY_CLIENT_ID=your_client_id
SPOTIFY_CLIENT_SECRET=your_client_secret
```

### 5. Run the Pipeline

- Extract data from the Spotify API:

```bash
python extract_data.py
```

- Transform the data and load it into AWS S3:

```bash
python transform_data.py
```

- Use AWS Glue for further processing and querying in Athena.

## 📈 Data Analysis and Insights

After loading the data into AWS Athena, you can perform queries to gain insights such as:

- **Top Artists**: Which artists have the most streams over time.
- **Popular Tracks**: Which songs are trending globally.
- **User Behavior**: Patterns in streaming behavior, such as most active times for listening.

These insights can be visualized in a BI tool like **Tableau**, **Power BI**, or **Amazon QuickSight**, providing rich, interactive reports.

## 🏆 Key Learnings

- Building a scalable data pipeline using modern cloud technologies.
- Automating data extraction from APIs using serverless architectures.
- Efficiently processing and transforming large datasets for analysis.
- Storing and querying data in a cloud data warehouse for real-time analytics.

## 👨‍💻 Future Enhancements

- **Real-time Processing**: Implement real-time data streaming with AWS Kinesis.
- **Machine Learning**: Apply machine learning models to predict song popularity trends.
- **Advanced Dashboards**: Create more advanced dashboards for deeper insights using Power BI or Looker Studio.

## 📬 Contact

If you have any questions or feedback, feel free to reach out:

- **LinkedIn**: [Prajwal KP](https://www.linkedin.com/in/prajwal-kibbanahalli-prabhuswamy/)
- **Email**: prajwal.prabhu0105@gmail.com
