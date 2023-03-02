# Ryanism.org Static APIs

Ryanism.org Static APIs is a collection of static JSON files used for [Ryanism.org](https://ryanism.org).

- [Member Count](members/) - [Minify](members/min/) - [readme.txt](members/readme.txt)
- [Quotes](quotes/) - [Minify](quotes/min/) - [readme.txt](quotes/readme.txt)
- [Legacy Quotes](legacyquotes/) - [Minify](legacyquotes/min/) - [readme.txt](legacyquotes/readme.txt)

## Built with

- [GitHub Actions](https://github.com/features/actions)
  - [styfle/cancel-workflow-action](https://github.com/marketplace/actions/cancel-workflow-action)
  - [actions/checkout](https://github.com/marketplace/actions/checkout)
  - [josStorer/get-current-time](https://github.com/marketplace/actions/get-current-time)
- [benborgers/opensheet](https://github.com/benborgers/opensheet)
- [stedolan/jq](https://github.com/stedolan/jq)
- [compress-json.sh](compress-json.sh)

## How does it work?

The APIs work by making use of these tools to retrieve and process the data, and then storing the data in the form of static JSON files. This makes it possible to access the data easily and efficiently, without the need for a server or a database.

The Member Count file contains the number of members in the organization. The Quotes file contains a list of quotes, while the Legacy Quotes file contains quotes from previous versions. All the files can be minified for faster loading times.

## Getting Started

Getting started with the Ryanism.org Static APIs is simple. You can access the APIs using a web browser or a programming language that supports JSON and retrieve the data as needed. The process is straightforward and can be done without any technical expertise.

### Javascript

```js
fetch("https://staticapi.ryanism.org/members/")
.then(response => response.json())
.then(data => {
  console.log(data);
});
 ```
 
 ### Node
 
 ```js
const https = require('https');

const options = {
  hostname: 'staticapi.ryanism.org',
  path: '/members/',
  method: 'GET'
};

const req = https.request(options, res => {
  let data = '';
  res.on('data', chunk => {  data += chunk; });
  res.on('end', () => { console.log(JSON.parse(data)); });
});

req.on('error', error => { console.error(error); });

req.end();
```

## Authors

- **[RyanistRyan](https://github.com/RyanistRyan)** - *Initial work*
- **[PiSaucer](https://github.com/PiSaucer)** - *Automated process*

See also the list of other [contributors](https://github.com/ryanism-org/staticAPI/contributors) who participated in this project.

## Contributing

Submit any issues or problems found in the static API on GitHub to notify the developers. This can be anything from security vulnerabilities to typos. If the you know how to fix the issue, they are encouraged to make a pull request to resolve it. If a you have a suggestion for a new feature or change, they can also submit it as an issue or reach out to the developers on [discord](https://ryanism.org/discord/) for further discussion. We welcome feedback and discussions about major changes.

## License ![badge](https://badgen.net/github/license/ryanism-org/staticAPI)

Distributed under the [MIT License](https://choosealicense.com/licenses/mit/). See [`LICENSE`](LICENSE) for more information.
