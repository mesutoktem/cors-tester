# CORS Error Simulation

This project demonstrates how to simulate and debug a CORS (Cross-Origin Resource Sharing) issue using a simple HTML file and an API request from `localhost`.

## Prerequisites

- Ensure you have `Node.js` installed on your system.
- The `http-server` npm package will be used to serve the HTML file.

## Steps to Run the Test

### 1. Clone or Download the Project

Ensure the `cors_test.html` file is in your project directory.

### 2. Install `http-server`

Open your terminal and run the following command to install `http-server` globally if you don't already have it:

```bash
npm install -g http-server
```

### 3. Navigate to the directory where cors_test.html is located and start the http-server:

```bash
npx http-server .
```

Once the server is running, open your browser and visit one of the following URLs:

http://127.0.0.1:8081/cors_test.html
http://192.168.1.103:8081/cors_test.html

### 4. Simulate the CORS Request
In the opened HTML page, you will see a button labeled "Make Request". Click the button to initiate a request to the API endpoint (http://localhost:8080/api/v1/test/application).

### 5. Handling CORS Error
If CORS is not correctly configured on your API server (http://localhost:8080), you should see a CORS error in the browser's console. The error will look something like this:

### 6. Modifying the API Endpoint
If you're testing with a different API, replace the URL in the axios.get call in the cors_test.html file:

```bash
axios.get('http://your-api-url/api/endpoint')
```




