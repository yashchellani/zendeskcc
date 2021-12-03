## Prerequisite Installations
- [NodeJS](https://nodejs.org/en/) v16.10.0 or greater
- NPM v7.24.0no

## How to run (MacOS/Windows)

1. Navigate to the directory of this README file in your CLI
2. Install all npm modules with the following code.

```
$ npm install
```

3. Run the program with the following code.

```
$ npm start
```

## Credential Management

- This app uses basic HTTP authentication to authenticate requests.

- In the same directory as src, create a .env file and add in the following line:

```
TOKEN={base64-encoded-string}
```
{base64-encoded-string} is a placeholder the encoded credentials of your account.

To obtain this string: 
- Combine your email address and password with a colon. Example: jdoe@example.com:pa$$w0rd.
- Base64-encode the resulting string. Example: amRvZUBleGFtcGxlLmNvbTpwYSQkdzByZA==.


#### Run Tests

1. Navigate to the repository directory in your MacOS Terminal or equivalent command line application.
2. Run the tests with the following code

```
$ npm test
```


### Main Component Description

- ```index.js``` : Program entry point, communicates data between components.
- ```Ticket.js``` : Data model for tickets.
- ```TicketFetcher.js``` : Makes requests to the Zendesk API and returns tickets.
- ```Display.js``` : Prints output and takes user input.
- ```Message.js``` : Contains general text for output, prompts, warnings, etc.

