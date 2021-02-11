# task.json-server

Sync server for [task.json](https://github.com/DCsunset/task.json).
It supports automatic conflicts handling and merging.

## Installation

### npm

```
npm i -g task.json-server
```

### Docker

```
docker pull dcsunset/task.json-server
```

## Usage

If installed from npm:

```
NODE_ENV=production DATA_PATH=$PWD/task.json task.json-server
```

If installed from docker:

```
docker run -d --name task.json-server -p 3000:3000 -v $PWD/task.json:/task.json dcsunset/task.json-server
```

Configurations can be set via environment variables.
Available configurations are listed below:

| Variables   | Default   | Description                           |
| ----------- | --------- | ------------------------------------- |
| ADDR        | `0.0.0.0` | Address to listen at                  |
| PORT        | `3000`    | Port to listen at                     |
| ROOT_PATH   | `/data`   | Absolute directory to store task.json |
| PASSWORD    | `admin`   | Login password                        |
| MAX_CLIENTS | `3`       | Max number of concurrent logins       |

## License

GPL-3.0
