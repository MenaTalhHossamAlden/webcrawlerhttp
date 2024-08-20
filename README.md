# webcrawlerhttp
A simple web crawler implemented in JavaScript that recursively crawls web pages and extracts URLS from HTML pages. This project demonstrates how to fetch, parse, ad handle HTML documents using `fetch API`, `JSDOM Package`, `URL Constructor`, and recursive algorithms.

## Features
- Recursively crawls web pages within the same domain by using the URL Constructor to parse each URL found in an HTML document and verify if the domain name matches the domain of the URL provided by the user.
- Extracts URLs from HTML pages using the JSDOM package, which generates an object representation of the HTML tree structure, allowing access to \<a> elements and their href attributes to retrieve URLs.
- Handles both relative and absolute URLs and normalizes them to prevent crawling the same page multiple times when accessed via different URLs.
- Logs errors for non-HTML responses, invalid URLs, and HTTP errors.
- Supports asynchronous crawling with concurrent fetch HTML documents requests to improve performance and efficiency.

## <img  align= center width=50px height=50px src="https://c.tenor.com/HgX89Yku5V4AAAAi/to-the-moon.gif"> Get Started <a id = "started"></a>

### Prerequisites
 - Node.js (check .nvmrc file for the version)

### Setup
<ol>
<li>Clone the repository

<br>

```bash
git clone https://github.com/MenaTahaHossamAlden/webcrawlerhttp.git
cd webcrawlerhttp
```
</li>
<li>Install dependencies

<br>

```
npm install
```

</li>

### Usage
To start the web crawler, use the following command:
````bash
npm start <websiteURL>
````

### Output:
The crawler logs the current page being crawled along with any errors it encounters, such as:

 - Non-HTML content responses.
 - Invalid URLs.
 - HTTP status codes > 399.

<br>

After crawling the specified website, the script generates a report that:
 - Lists all the URLs found within the website.
 - Sort URL by the count of how many times each URL was encountered during the crawl.