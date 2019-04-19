# snips-action-timer
#### Snips action code for the Timer app

## Setup

```sh
# Install the dependencies, builds the action and creates the config.ini file.
sh setup.sh
```

## Run

- Dev mode:

```sh
# Dev mode watches for file changes and restarts the action.
npm run dev
```

- Prod mode:

```sh
# 1) Lint, transpile and test.
npm start
# 2) Run the action.
node action-timer.js
```

## Debug

In the `action-timer.js` file:

```js
// Uncomment this line to print everything
// debug.enable(name + ':*')
```

## Test

*Requires [mosquitto](https://mosquitto.org/download/) to be installed.*

```sh
npm run test
```

**In test mode, i18n output is mocked.**

- **i18n**: see `src/factories/i18nFactory.ts`