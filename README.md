# Simple Go Web Server

This project is a basic web server written in Go. It demonstrates handling HTTP requests with different routes and parsing form data. The server responds to simple GET and POST requests.

## Features

- Serves static files from a `static/` directory.
- Handles GET requests on the `/hello` route.
- Handles POST requests on the `/form` route, extracting and displaying form data.

## Prerequisites

- [Go](https://golang.org/doc/install) (version 1.16 or higher)

## Getting Started

1. **Clone the Repository**:

   ```bash
   git clone <repository-url>
   cd <repository-directory>

2. Create a static/ directory:

This directory will be used to store your static HTML or other files that you want to serve through the root endpoint (/).

Write an HTML Form:

Create a file named static/form.html with the following content:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Form Submission</title>
</head>
<body>
    <h2>Submit Your Info</h2>
    <form action="/form" method="post">
        <label for="name">Name:</label><br>
        <input type="text" id="name" name="name"><br><br>
        <label for="address">Address:</label><br>
        <input type="text" id="address" name="address"><br><br>
        <input type="submit" value="Submit">
    </form>
</body>
</html>

Usage
- Access the Homepage: Open your browser and go to http://localhost:8080/. It will display the files from the static/ directory.

- Access the Form Page: Navigate to http://localhost:8080/form.html. Fill in the form and click "Submit" to see your form data displayed.

- Access the /hello Endpoint: Go to http://localhost:8080/hello to get a simple "hello!" response.


Project Structure
.
├── main.go           # Main Go server file
└── static            # Directory to serve static files
    └── form.html     # Example HTML form for testing POST requests

If you want to contribute, please feel free to create a pull request or submit an issue.
