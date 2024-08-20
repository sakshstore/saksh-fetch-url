
# Saksh Fetch URL Package

A Node.js package to fetch the contents of a given URL  .

## Installation

To install the package, run:

```bash
npm install saksh-fetch-url

```


### Usage
 
You can use the package as a library in your Node.js application.

```
const file_get_contents = require('saksh-fetch-url');

async function fetchContent(url) {
try {
const data = await file_get_contents(url);
console.log(data);
} catch (error) {
console.error('Failed to fetch content:', error);
}
}


// Example usage
const url = 'https://example.com';
fetchContent(url);

```
### more examples


Here's an example of how you can use the file_get_contents function to read both a local file and a remote file:


#### Local File Example:

- First, create a local file named example.txt with some content:

- This is a sample text file.

- Then, use the file_get_contents function to read this file:

```

const file_get_contents = require('saksh-fetch-url');

async function readLocalFile() {
try {
const data = await file_get_contents('example.txt');
console.log('Local file content:', data);
} catch (error) {
console.error('Error:', error);
}
}

readLocalFile();
```


####  1. Remote File Example:

- Use the file_get_contents function to fetch data from a remote URL:


```
const file_get_contents = require('saksh-fetch-url');

async function readRemoteFile() {
try {
const data = await file_get_contents('https://jsonplaceholder.typicode.com/posts/1');
console.log('Remote file content:', data);
} catch (error) {
console.error('Error:', error);
}
}

readRemoteFile();
```


In these examples, readLocalFile reads the content of a local file named example.txt, and readRemoteFile fetches data from a remote URL. Make sure to replace './file_get_contents' with the correct path to your file_get_contents module.

 


  
### License
This project is licensed under the MIT License. See the LICENSE file for details.

### Contributing
Contributions are welcome! Please open an issue or submit a pull request.

 

### Contact
For any questions or feedback, please contact susheel2339 @ gmail.com

