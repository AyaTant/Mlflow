# Mlflow project

import dagshub
dagshub.init(repo_owner='AyaTant', repo_name='Mlflow', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)