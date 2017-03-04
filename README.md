# dojo-data
EPFL dojo data for events, announcements, archives and maybe more...

## Infos
We use [https://hjson.org](https://hjson.org) to have a human writable/readable format for data. Then, `*.json` files are generated into the ./src folder.

## Usage
1. install https://hjson.org
2. generate JSON files with hjson:
`for i in *.hjson; do hjson -j $i > src/"${i%.*}".json; done`
or `hjson -j links.hjson > src/links.json`
