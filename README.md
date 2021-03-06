# NextDrop
### Powerful auto-buying bot
Built in Node.js using Electron + React

![NextDrop running on Windows](https://raw.githubusercontent.com/HusnainJaved/nextdrop/main/screenshots/nextdrop-win-1.png)

## Features
- Simple, intuitive GUI
- Run multiple concurrent tasks
- Schedule tasks
- Repeat stock checking
- Cross-platform
- Clean architecture
- Easily extensible scrapers

## Goals
| Description | Status |
|-|-|
| Add more scrapers | *In progress* |
| Implement auto updating | *Not started* |
| Add proxy support | *Not started* |

## Usage

##### Download for Windows
Grab the latest Windows installer from [here](https://github.com/HusnainJaved/nextdrop/releases/latest).

##### NPM
```
npm run start
```

##### Yarn
```
yarn start
```

## Supported retailers
- [x] Currys
- [ ] Game
- [ ] John Lewis
- [ ] ShopTo
- [ ] Smyths

##### Currently only focusing on UK retailers.
*You can contribute by developing a scraper for one of these, I've made it very simple to do so.*

##### Build your own scraper
Add a new retailer by creating a new Scraper class that extends BaseScraper from `infrastructure/scrapers`. The base class contains enough abstract functions to guide you from the home page all the way to order confirmation.

Then just append a new record in `infrastructure/data/retailers.ts` and `infrastructure/services/ScraperService.ts`.

## License
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)