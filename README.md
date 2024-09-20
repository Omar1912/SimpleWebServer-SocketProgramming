# Tiny Web Server
This repository contains the code for a **Tiny Web Server** built for the **ENCS3320 Computer Networks** course. The project demonstrates the implementation of a basic web server using socket programming, with support for serving HTML pages, CSS, images, and handling HTTP requests for sorting laptop data. It also supports requests in both **English** and **Arabic**.

### Project Overview
The goal of this project is to build a simple web server using socket programming in Python that listens to HTTP requests on a specified port and responds with the appropriate content. The server can serve static files such as HTML pages, images, and CSS, while also handling more complex requests like sorting data and redirecting users to external websites.

Key objectives include:

- Learning socket programming and understanding the fundamentals of HTTP communication.

- Serving both English and Arabic versions of a web page, along with handling various file types.

- Implementing dynamic responses based on the request URL, such as sorting laptops by name or price.

- Demonstrating redirection for certain requests to external websites.

### Features
- Serve static HTML pages and images.
- Handle HTTP requests for specific files (HTML, CSS, PNG, JPG).
- Display dynamic content (sorting laptops by name or price).
- Redirect requests to external websites (Amazon, Stack Overflow, etc.).
- Serve both an English and Arabic version of the main page.
- Error handling for invalid requests with a 404 response page.
  
### Files
  ####  Server Code
- `web-server.py` : This is the core Python server code. It listens for HTTP requests and serves the corresponding files or handles specific requests (e.g., sorting laptop data, redirects, etc.)​(web-server).
- `server.py`: An additional server implementation to handle TCP connections and lock the workstation based on valid user IDs​(server).
- `client.py`: The client-side code that sends a request to the server and prints the server’s response​(client).
#### HTML Files
- `main_en.html`: The English version of the main web page. It includes links to other resources and displays information about the project members​(main_en).
- `main_ar.html`: The Arabic version of the main web page. It mirrors the content of the English page but in Arabic​(main_ar).
- `secondary.html`: A secondary web page used for testing the server's ability to serve multiple HTML pages​(secondary).
#### CSS Files
- `main.css` : Stylesheet for the English and Arabic pages, providing layout, typography, and styling for the web content​(main).
- `second.css` : Additional styling for the secondary page, featuring background images and custom shapes​(second).

### Key Functionalities
1. Dynamic Content Handling:

      - Sort laptops by name or price when requested via /SortByName or /SortByPrice routes. It displays the sorted names and prices directly in the browser.
   
2. Multilingual Support:
      - The server responds with either an English (/en) or Arabic (/ar) version of the main web page based on the user's request.

3. File Handling:
      - Serves HTML, CSS, and image files based on the requested resource (e.g., /main_en.html, /main_ar.html, /image.png, etc.).

 4. Redirection:  
      -  Redirect specific requests (/azn, /so, /bzu) to external websites such as Amazon, Stack Overflow, and Birzeit University.

5. Error Handling:
      - Responds with a custom 404 page if the requested file or resource is not found.

