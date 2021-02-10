# task.json-server

Sync server for [task.json](https://github.com/DCsunset/task.json).
It supports automatic conflicts handling and merging.

## Installation

```
npm i -g task.json-server
```

## Usage

```
DATA_PATH=$PWD/task.json task.json-server
```

Configurations can be set via environment variables.
Available configurations are listed below:

| Variables   | Default      | Description                      |
| ----------- | ------------ | -------------------------------- |
| ADDR        | `0.0.0.0`    | Address to listen at             |
| PORT        | `3000`       | Port to listen at                |
| DATA_PATH   | `/task.json` | Absolute path to store task.json |
| PASSWORD    | `admin`      | Login password                   |
| MAX_CLIENTS | `3`          | Max number of concurrent logins  |

## License

GPL-3.0