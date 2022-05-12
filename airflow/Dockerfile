FROM apache/airflow:2.2.4
USER root
RUN apt-get update \
  && apt-get install -y --no-install-recommends \
         libpq-dev python-dev gcc \
  && apt-get autoremove -yqq --purge \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists/*
USER airflow
RUN  pip install --no-cache-dir -i http://pypi.douban.com/simple/ --trusted-host=pypi.douban.com/simple ipython apache-airflow-providers-celery \
apache-airflow-providers-elasticsearch \
apache-airflow-providers-ftp \
apache-airflow-providers-http \
apache-airflow-providers-imap \
apache-airflow-providers-jdbc \
apache-airflow-providers-microsoft-mssql \
apache-airflow-providers-mysql \
apache-airflow-providers-postgres \
apache-airflow-providers-redis \
apache-airflow-providers-sftp \
apache-airflow-providers-sqlite \
apache-airflow-providers-ssh \
beautifulsoup4 \
clickhouse-driver \
dataclasses \
DBUtils \
elasticsearch \ 
fastapi \
graphviz \
mysql-connector-python \
mysqlclient \
openpyxl==3.0.7 \
pandas \
paramiko \
petl \
prettytable \
psycopg2 \
psycopg2-binary \
pymssql \
redis \
requests \
SQLAlchemy \
supervisor \
swagger-ui-bundle \
virtualenv \
virtualenvwrapper \ 
xlrd==1.2.0 \
ibm_db
