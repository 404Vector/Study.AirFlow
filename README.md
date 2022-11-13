# Study.AirFlow

## Requirement

- poetry

## initialize

- install package

```shell
poetry install
```

- set homepath

```shell
export AIRFLOW_HOME={SOMEWHERE_YOU_WANT_TO_USE}

# 현재 경로를 Airflow 프로젝트의 루트 경로로 설정
export AIRFLOW_HOME=.
```

- init airflow db

```shell
export AIRFLOW_HOME=.
airflow db init
```

- create admin account

```shell
airflow users create -u admin -p admin -f [이름] -l [성] -r Admin -e admin@admin.com
```

## Run Airflow service

### Run WebServer

```shell
airflow webserver -p [port]
```

### Run scheduler

```shell
airflow scheduler
```
