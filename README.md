# Dags Covid Pipline
Python 3.8.10

## Install Apache Airflow

1. Install Virtual Enviroment
```sh
pyenv install 3.8.10
```

2. Create Directory for Project
 ```sh
mkdir airflow-setup
cd airflow-setup
```

3. Create Virtual Enviroment
```sh
python3 -m venv ENV
```

4. Activate Enviroment
```sh
source ENV/bin/activate
```

5. Install and run test Apache Airflow
```sh
pip3 install apache-airflow
airflow db init
airflow webserver -p 8080
```
หมายเตุ
Add user
```sh
airflow users create --username admin --firstname FIRST_NAME --lastname  LAST_NAME --role Admin --email admin@example.org
```

Add Repo สำหรับ Install Driver ODBC
```sh
curl -sSL https://packages.microsoft.com/keys/microsoft.asc | sudo tee /etc/apt/trusted.gpg.d/microsoft.asc

sudo apt-add-repository https://packages.microsoft.com/ubuntu/20.04/prod

sudo apt-get update

sudo apt-get install msodbcsql17
```
