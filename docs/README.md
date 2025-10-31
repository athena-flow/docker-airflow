```shell
docker run --rm "debian:bookworm-slim" bash -c 'numfmt --to iec $(echo $(($(getconf _PHYS_PAGES) * $(getconf PAGE_SIZE))))'

curl -LfO 'https://airflow.apache.org/docs/apache-airflow/3.1.1/docker-compose.yaml'

mkdir -p ./dags ./logs ./plugins ./config
echo -e "AIRFLOW_UID=$(id -u)" > .env

sudo docker compose run airflow-cli airflow config list
sudo docker compose up airflow-init
sudo docker compose up -d

http://49.232.232.231:8080/
admin
admin

sudo docker exec -it 2f2ad0105ad9 bash
airflow users  create --role Admin --username admin --email admin --firstname admin --lastname admin --password admin

sudo docker compose up airflow-init
sudo docker compose down --volumes --remove-orphans
sudo docker compose up
sudo docker compose run airflow-worker airflow info

curl -LfO 'https://airflow.apache.org/docs/apache-airflow/3.1.1/airflow.sh'
chmod +x airflow.sh
./airflow.sh info
./airflow.sh bash
./airflow.sh python

ENDPOINT_URL="http://localhost:8080"
curl -X GET  \
    --user "airflow:airflow" \
    "${ENDPOINT_URL}/api/v1/pools"

sudo docker compose down --volumes --rmi all
```