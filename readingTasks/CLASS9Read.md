# Reading Class 09

## Five Steps in the HTTP Request Lifecycle:

1- DNS Resolution: The client needs to resolve the domain name of the server to an IP address using the Domain Name System (DNS).

2- TCP Connection: The client establishes a TCP connection with the server on the specified port.

3- HTTP Request: The client sends an HTTP request to the server, including the request method (GET, POST, etc.), headers, and any optional data.

4- Server Processing: The server processes the request, performs the necessary actions, and generates an HTTP response.

5- HTTP Response: The server sends an HTTP response back to the client, which includes response headers, status code, and response data.

## Two Things the Client Needs Before Making an HTTP Request:

1- URL (Uniform Resource Locator): The URL specifies the address of the resource the client wants to request.

2- HTTP Method: The client needs to determine the appropriate HTTP method for the request (e.g., GET, POST, PUT, DELETE) to indicate the desired action to be performed on the resource.

## Four-Way Handshake:
The term "four-way handshake" is often associated with TCP connection establishment and termination. It's used to establish and release a connection between a client and a server. The steps are as follows:

1- Client sends a SYN (Synchronize) packet: Initiates the connection request.

2- Server responds with SYN-ACK (Synchronize-Acknowledge) packet: Acknowledges the client's request and sends its own synchronization request.

3- Client sends an ACK (Acknowledge) packet: Acknowledges the server's synchronization request, and the connection is established.

4- Connection termination: To terminate the connection, one party sends a FIN (Finish) packet, and the other responds with an ACK. Then, the roles are reversed, and the other party sends a FIN followed by an ACK. This process ensures a graceful connection closure.

## Java HTTP Request Example:
Here's a simple Java example using the built-in HttpURLConnection class to make an HTTP GET request:

---
import java.io.BufferedReader;
import java.io.InputStreamReader;
import java.net.HttpURLConnection;
import java.net.URL;

public class HttpRequestExample {
    public static void main(String[] args) {
        try {
            URL url = new URL("https://example.com");
            HttpURLConnection connection = (HttpURLConnection) url.openConnection();

            int responseCode = connection.getResponseCode();
            if (responseCode == HttpURLConnection.HTTP_OK) {
                BufferedReader reader = new BufferedReader(new InputStreamReader(connection.getInputStream()));
                String line;
                StringBuilder response = new StringBuilder();

                while ((line = reader.readLine()) != null) {
                    response.append(line);
                }
                reader.close();

                System.out.println("Response: " + response.toString());
            } else {
                System.out.println("HTTP Request failed with response code: " + responseCode);
            }

        } catch (Exception e) {
            e.printStackTrace();
        }
    }
}

---

## Following Redirects:
By default, most HTTP client libraries follow redirects (3xx status codes) automatically. However, clients may provide options to disable automatic redirect following. It's generally a good practice to follow redirects as they often indicate a resource has been moved or the client should access a different URL.

## HTTP Status Codes:

Successful Response (2xx): 200 OK is the most common success code.
Redirect (3xx): Examples include 301 Moved Permanently, 302 Found (temporarily moved), and 307 Temporary Redirect.
Client Error (4xx): Examples include 400 Bad Request, 404 Not Found.
Please note that the information provided is based on the state of knowledge up to September 2021, and there might have been developments or changes beyond that date.
