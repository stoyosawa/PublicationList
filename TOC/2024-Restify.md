# Building REST Servers

<!--- 200 x 258 -->
<img src="https://www.cutt.co.jp/book/images/978-4-87783-549-1.png" width="200">

Satoshi Toyosawa  
Cutt System, Tokyo, Japan. 2024.

## Table of Contents

- **Part I: REST Servers**
	- Chapter 1　Restify Basics
    - Chapter 2　Access Control
    - Chapter 3　Backend Database - MongoDB Atlas
    - Chapter 4　Neat features
- **Part II: Fundamentals**
    - Chapter 5　Node.js
    - Chapter 6　Restify
    - Chapter 7　Node.js HTTP/HTTPS/HTTP2 modules
    - Chapter 8　MongoDB Atlas
    - Chapter 9　curl
    - Chapter 10　OpenSSL ... Generating self-signed certificates for HTTPS servers
    - Appendix A　References
    - Appendix B　List of scripts (see below)
    - Appendix C　JSON

## List of scripts

The scripts discussed in this book (in alphabetical order).

Filename | Section | Description
---|---|---
`access-accept.js` | 2.4 | Handles the `Accept` header.
`access-basicauth.js` | 2.1 | Authenticates using `Authentication: Basic`.
`access-control.js` | 2.2 | Authorizes per user, per method, per endpoint (RBAC).
`access-jwt.js` | 2.5 | Authenticates using JWT（JSON Web Token).
`access-throttle.js` | 2.3 | Throttles traffics based on the request frequency.
`mongo-admin.js` | 3.6 | Administers endpoint for managing table and user names.
`mongo-auth.js` | 3.7 | Endpoint for changing the user password.
`mongo-delete.js` | 3.5 | `DELETE` resources that matches the query options (OData style).
`mongo-get.js` | 3.2 | `GET` resources.
`mongo-post.js` | 3.4 | `POST` resource.
`mongo-query.js` | 3.3 | `GET` method with the `count`、`select`、`orderBy`、`top` query options (ODATA style).
`node-client.js` | 7.5 | Node.js native HTTP/HTTPS client.
`node-http.js` | 7.2 | Node.js native HTTP client.
`node-http2.js` | 7.4 | Node.js native HTTP/2 server (`https://`).
`node-https.js` | 7.3 | Node.js native HTTPS server (use self-signed cert).
`others-client.js` | 4.5 | Restify's own HTTP client.
`others-formatter.js` | 4.4 | Transforms input to `text/html` and `text/markdown` formats in response to the `Accept` request header.
`others-gzip.js` | 4.3 | Compresses response body (`Accept-Encoding` request and `Content-Encoding` response headers).
`others-redirect.js` | 4.2 | Redirects (301) from the old `/old/xxx` request to `/new/xxx`.
`others-static.js` | 4.1 | Serves static HTML files (not REST).
`rest-endpoint.js` | 1.2 | Demonstrates a various endpoint formats.
`rest-http.js` | 1.1 | A simple HTTP/1.1 REST server.
`rest-http2.js` | 1.7 | A simple HTTP/2 REST server (self-signed cert).
`rest-https.js` | 1.6 | A simple HTTPS/1.1 server (self-signed cert).
`rest-post.js` | 1.5 | `POST`resource (file-base).
`rest-query.js` | 1.4 | Parses the query string and returns the matching resources (file-base).
`rest-sanitize.js` | 1.3 | Sanitizes the URL path.
`restify-chain.js` | 6.4 | Demonstrates the order of handler execution.
`util-ab.js` | 2.3 | A utility to bombard a HTTP server (in case you don't have `apache ab`).
`util-hash.js` | 2.2 | A utility to generate SHA-256 from input string.
