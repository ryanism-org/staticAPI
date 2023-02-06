# Ryanism.org Static APIs

Ryanism.org Static APIs is a collection of static JSON files used for [Ryanism.org](https://ryanism.org). The files contain information such as member count, quotes, and legacy quotes.

* [Member Count](members/) - [Minify](members/min/) - [Readme.txt](members/readme.txt)
* [Quotes](quotes/) - [Minify](quotes/min/) - [Readme.txt](quotes/readme.txt)
* [Legacy Quotes](legacyquotes/) - [Minify](legacyquotes/min/) - [Readme.txt](legacyquotes/readme.txt)

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

Getting started with the Ryanism.org Static APIs is simple. All you need to do is access the APIs using a web browser or a programming language that supports JSON. The data can then be retrieved and used as needed.

## Authors

- **[RyanistRyan](https://github.com/RyanistRyan)** - *Initial work*
- **[PiSaucer](https://github.com/PiSaucer)** - *Automated process*

See also the list of other [contributors](https://github.com/ryanism-org/staticAPI/contributors) who participated in this project.

## Contributing

Pull requests are welcome. If you find any problem(s) in the staticAPI, feel free to submit an issue. This includes stuff like vulnerabilities, or even the most trivial issues (such as typoes.) If you know how to fix an issue, feel free to make a pull request for the issue. If you would like to suggest a feature or change, submit it as an issue as well or message us on [discord](https://ryanism.org/discord/); it will be given the appropriate tag once we have seen it. We love to discuss any major changes with you.

## License ![badge](https://badgen.net/github/license/ryanism-org/staticAPI)

Distributed under the [MIT License](https://choosealicense.com/licenses/mit/). See [`LICENSE`](LICENSE) for more information.
