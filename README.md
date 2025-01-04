# ed-colonisation-planner
A colonisation planner for Elite: Dangerous

There's no specific goal for this project. It'll likely just be a collection of personal-use scripts for
various tasks relating to the upcoming colonisation feature in Elite. The features/scripts are listed below.
The same information can also be found at the top of each script file.

# Pre-requisites
Running the scripts requires:
- [Node.js and (optionally) NPM](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)

# Running scripts
The scripts can be run in two ways. These instructions are written with consideration for those who may not be familiar with Node or coding in general.

#### 1. Run files using NPM

The `scripts` list in [package.json](package.json) contains a list of all available scripts for easy access. To run scripts through NPM,
simply run `npm run script` where `script` is the name of the appropriate script, like below:
```sh
npm run elw-finder
```

#### 2. Run files directly using Node
Node can also be used to run the files directly, like below:
```sh
node src/elw-finder
```

# Scripts list
## Unpopulated ELW Finder
The `elw-finder` script finds unpopulated systems with Earth-like Worlds (ELWs) within a given radius of a specified system.
The minimum and maximum radius are configurable, as well as the origin system.

Because the EDSM API is limited in the functionality it exposes, this script first gets all systems in the radius and
then filters down to unpopulated systems with ELWs. Because of this approach, the script may take a long time to run
if the search radius is large.
