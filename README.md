#weather-cli

[![Coverage Status](https://github.com/92bondstreet/rdd-cdd-tdd/tree/master/weather/tests)](https://github.com/92bondstreet/rdd-cdd-tdd/tree/master/weather/tests)

Weather give weather of the city of your choice, more precisely condition and temperature.

Check the weather for your city from your terminal

*Se [pageres-cli](https://github.com/92bondstreet/rdd-cdd-tdd/tree/master/weather) for the command-line tool.*


## Install

```
$ npm install yql
$ npm install meow
$ npm install chalk
$ npm install updateNotifier
$ npm install request

```


## Usage

```js
const weather = require('./');

```

## Version

1.0.0


## Scripts

To start the application, you need to start like this:"node cli.js",

To start test, you need to start like this: "mocha -t 10000 tests/tests.js"

To have coverage, tou need to start like this: "istanbul cover ./node_modules/mocha/bin/_mocha --report lcovonly -- -R spec tests/tests.js -t 100000 && cat ./coverage/lcov.info | ./node_modules/coveralls/bin/coveralls.js && rm -rf ./coverage"

### Weather([options])

#### options

##### city

Type: `string` *()*<br>
Default: `Dhaka`

City given by user which is the city where the wheather must be given.


##### country

Type: `string` *()*<br>
Default: `Bangladesh`

Country given by user which is the country where wheather must be given.

##### scale

Type: `number`*(C/F)*<br>
Default: `Celsius`

Temperature of city, it's given in Celsius or Farenheit.

###### Examples

Examples of how use Weather and what result it give.

Apply like this:  
$ weather London UK C', ($ weather [City] [Country] [Scale])

Result:
'  London, UK', 
'  Condition: Partly Cloudy',
'  Temperature: 32C'

## License

MIT © [weather-cli](https://github.com/92bondstreet/rdd-cdd-tdd)
