CONTAINER_ID= bcc1e133d8cf7532217902646b9b132df92c088a861cd63ac66f24514f5675bf

build_airflow:
	docker build -t airflow .

run_airflow:
	docker run --rm -d -p 8080:8080 $(CONTAINER_ID)

stop_airflow:
	docker stop $(CONTAINER_ID)

airflow_cli:
	docker exec -it $(CONTAINER_ID) /bin/bash

airflow_webserver:
	docker exec -it $(CONTAINER_ID) airflow webserver

airflow_list_dags:
	docker exec -it $(CONTAINER_ID) airflow list_dags
