# Horizon News Hub (News Aggregator Application) - [![Netlify Status](https://api.netlify.com/api/v1/badges/992d1de3-06ae-4bdb-a95b-e7a5a8cc7d10/deploy-status)](https://app.netlify.com/sites/latestnewsaggregator/deploys)

# 

## Brief Description
**Horizon News Hub** is a modern and responsive news aggregator web application built with **React.js**. It pulls news articles from multiple trusted sources, providing a seamless experience for users to explore, search, and personalize their news feed. With robust filtering options and a clean interface, the application focuses on delivering news efficiently and intuitively. The project is containerized using **Docker** and deployable on various platforms.

## Index
1. [Features](#features)  
2. [Technologies Used](#technologies-used)  
3. [Setup and Installation](#setup-and-installation)  
4. [Usage and Examples](#usage-and-examples)  
5. [Code Organization and Structure](#code-organization-and-structure)  
6. [Contributions and Feedback](#contributions-and-feedback)  
7. [Acknowledgements and Credits](#acknowledgements-and-credits)  
8. [License](#license)  

## Features
- **Article Search and Filtering:**
  - Search for articles using keywords.
  - Filter results by date, category, and source.
- **Personalized News Feed:**
  - Create a custom feed by selecting preferred news sources, categories, and authors.
- **Mobile-Responsive Design:**
  - Fully optimized for desktop and mobile viewing.
- **API Integration:**
  - Leverages multiple APIs (NewsAPI, The Guardian API, New York Times API) to gather diverse and up-to-date articles.

## Technologies Used
- **Frontend:**
  - [React.js](https://react.dev): Library for building user interfaces.
  - [React Bootstrap](https://react-bootstrap.github.io/): Pre-styled UI components.
- **State Management:**
  - [Redux Toolkit](https://redux-toolkit.js.org/): Simplified state management.
- **HTTP Requests:**
  - [Axios](https://axios-http.com/): For fetching data from APIs.
- **Backend Deployment:**
  - [Docker](https://www.docker.com/): For containerization and deployment.
- **APIs for News Data:**
  - [NewsAPI](https://newsapi.org/), [The Guardian API](https://open-platform.theguardian.com/), [New York Times API](https://developer.nytimes.com/).

## Setup and Installation
To run the application locally or in a Dockerized environment, follow these steps:

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/horizon-news-hub.git
   cd horizon-news-hub
   ```
2. **Install Dependencies:** Ensure you have Node.js installed. Run:
   ```bash
   npm install
   ```
3. **Install Dependencies:** Ensure you have Node.jsinstalled. Run:
   ```bash
   REACT_APP_NEWS_API_KEY=your_newsapi_key
   REACT_APP_GUARDIAN_API_KEY=your_guardian_key
   REACT_APP_NYT_API_KEY=your_nyt_key
   ```
4. **Run the Application:** Start the development server with:
   ```
   npm start
   ```
   The application will be available at http://localhost:3000.
5. **Docker Deployment (Optional):** Build and run the Docker container:
   ```
   docker build -t horizon-news-hub .
   docker run -p 80:80 horizon-news-hub
   ```
   Or, using Docker Compose:
   ```
   docker-compose up --build
   ```

## Code Organization and Structure
```
horizon-news-hub/
│
├── public/
│   ├── index.html
│   └── ...
│
├── src/
│   ├── components/              # Reusable components
│   │   ├── Error/
│   │   ├── Loading/
│   │   ├── NavBar/
│   │   ├── News/
│   │   ├── NewsCard/
│   │   ├── NoDataFound/
│   │   ├── NoRouteFound/
│   │   ├── ScrollToTop/
│   │   └── ...
│   │
│   ├── config/                  # API configurations and constants
│   ├── images/                  # Static assets
│   ├── pages/                   # Page-level components
│   │   ├── HomePage/
│   │   ├── PersonalizedPage/
│   │   └── ...
│   │
│   ├── router/                  # Routing configuration
│   ├── store/                   # Redux state management
│   ├── App.css                  # Global styles
│   ├── App.js                   # Main component
│   ├── index.css                # Index styles
│   ├── index.js                 # Entry point
│   └── ...
│
├── .dockerignore
├── .env
├── .gitignore
├── docker-compose.yml
├── Dockerfile
├── package.json
└── ...
```

## Contributions and Feedback
This project is no longer accepting contributions. However, I would love to hear your feedback to improve my future projects. Feel free to reach out through GitHub Issues.

## Acknowledgements and Credits

- **APIs:**  
  - [NewsAPI](https://newsapi.org/) 
  - [The Guardian API](https://open-platform.theguardian.com/)
  - [New York Times API](https://developer.nytimes.com/)
 
## License
This project is licensed under the MIT License. For more details, see the [LICENSE](URL) file.

