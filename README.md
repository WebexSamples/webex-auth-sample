# webex-auth-sample

## Description

A simple application demonstrating how to retrieve a Cisco Webex OAuth2 token for use with the Cisco Webex APIs.

  - **Technology stack**: HTML/JavaScript

  - **Status**:  v1.0 [CHANGELOG](CHANGELOG.md)

## Installation

* From a terminal, clone this repo to your local PC:

    ```bash
    git clone https://github.com/WebexSamples/webex-auth-sample.git
    ```

* The HTML page must be served from a web server (not just opened from the local file system).  

    If you have Node.js and NPM v5.2+, you can run the following from the root of this repo to start a simple web server serving everything in the current directory:

    ```bash
    cd webex-auth-sample
    npx http-server
    ```

    ```bash
    #Example response
    npx: installed 23 in 3.334s
    Starting up http-server, serving ./
    Available on:
    http://127.0.0.1:8080
    http://10.99.58.21:8080
    http://172.16.255.1:8080
    http://192.168.52.1:8080
    Hit CTRL-C to stop the server
    ```

## Usage

- Register a Webex 'integration' application at [https://developer.webex.com/my-apps](https://developer.webex.com/my-apps)

- The **Redirect URI** provided during registration should be the URL where this sample app page will be hosted, which can be a 'localhost' URL, e.g.:

    ```
    http://127.0.0.1:8080/webex-auth.html
    ```

- **Scopes** should include, at minimum, `spark:rooms_read` (note `spark:all` will not work)

- The application **Client ID** and **Client Secret** generated during registration are required to run the app - the secret will only be displayed once.  Make a note of these two values to run the sample

## Getting help

* Webex developer support: [https://developer.webex.com/support](https://developer.webex.com/support)

## Getting involved

Suggestions and enhancements welcome, see [CONTRIBUTING](CONTRIBUTING.md).

----

## Open source licensing info
[LICENSE](LICENSE)
