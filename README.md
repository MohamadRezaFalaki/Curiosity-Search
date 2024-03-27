
## Curiosity-Search 

### A Laravel API for Dynamic Web Content Retrieval

This project provides a Laravel-based API that enables front-end applications to retrieve information about specified categories and details from the web. This retrieved data can be used to dynamically populate web pages with relevant content.

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)

![Logo](https://th.bing.com/th/id/OIG2.TOLJXErdMkwTFiFQKlhH?w=1024&h=1024&rs=1&pid=ImgDetMain)


## Features:

* Accepts search requests with category and detail parameters.

* Leverages web scraping or web search APIs to retrieve information from the web.

* Web Scraping: Parses HTML content of target websites to extract title, body, and image URL.

* Web Search API: Integrates with a web search API (e.g., Google Custom Search) to retrieve curated search results.

* Returns retrieved information (title, body, image URL) as a JSON response.
## Benefits:

* Simplifies front-end development by providing a centralized API for retrieving dynamic content.

* Offers flexibility for choosing between web scraping or web search APIs based on your needs.

* Allows for building custom search functionalities for your front-end applications.
## Getting Started:

1. Clone the repository:

```Bash
git clone https://github.com/your-username/your-repo-name.git
```

2. Install dependencies:


```Bash
composer install
```

3. Configure environment variables (if using web search API):

* Create a .env file in the project root directory.
* Set up necessary API keys or credentials for the chosen web search API.

4. Run database migrations (if applicable):

```Bash
php artisan migrate
```

5. Start the development server:

```Bash
php artisan serve
```
## Usage:

1. Send a GET request to the API endpoint with category and detail parameters:

```
GET /search?category={category}&detail={detail}
```
Example:

```
GET /search?category=game&detail=pubg
```

2. The API will respond with a JSON object containing the retrieved information:

```JSON
{
    "title": "PUBG Mobile: Battlegrounds Royale Game",
    "body": "PUBG Mobile is a...",
    "image_url": "https://...",
}
```
## Technologies Used:

* Laravel (PHP framework)
* Guzzle (HTTP client for web requests)
* Goutte (optional, for web scraping)

## License:
MIT License
## Further Considerations:

* Web scraping has ethical and technical limitations. Respect robots.txt guidelines and consider using web search APIs for better reliability.

* Implement caching mechanisms in your Laravel API to improve performance and reduce unnecessary web requests.
## Contribution:

I welcome contributions to this project. Feel free to submit pull requests!

This comprehensive description provides a clear overview of your project's purpose, functionalities, usage instructions, and technical details. It also encourages potential contributors to engage with your project.
