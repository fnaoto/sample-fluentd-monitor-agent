# fluentd-monitor-agent-sample

This repo is sample for gathering log with Fluentd,
and monitor itself on NewRelic.

```sh
<Nginx> --> `/var/log/nginx` <-- <Fluentd> --> `0.0.0.0:24220` <-- <NewRelic>
```

## Usage

- Settings for NewRelic

```
$ cp .env.sample .env
$ vim .env

NRIA_LICENSE_KEY=<Enter NewRelic license key>
```

- Run

```
$ docker-compose up -d --build
```

- UI for Fluentd

```
$ open localhost:9292

Enter:
  user: admin
  pass: changeme
```
