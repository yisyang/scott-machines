# scott-machines
CasC storage space of new and migrated personal projects.

# Initial project

## Plan for stock project
- [x] Bootstrap with Flux to enable CD (https://github.com/fluxcd/flux2-kustomize-helm-example)
- [x] Start locally with K8s w/ robotrade namespace
- [x] Add TSDB
- [x] Add Redis
- [] Add CouchBase
- Create robotrader REST API
  - [] Start new repo w/ Python on FastAPI
  - [] Endpoint for adding/removing symbols to monitor (CouchBase)
  - [] Ingesting 365 days of data from Alpaca for given symbol (TSDB)
- [] Optional: Add Pub/Sub w/ persistence (Kafka or RabbitMQ)
- [] Add Task Queue (RQ or Celery)
- [] Add Grafana
- Update API to handle predictions
  - [] Predict 1, 2, 3, 5 days trends from historic data and actions to take (CouchBase)
  - [] Evaluate past predicted actions (CouchBase)
  - [] Add relevant dashboards for actual/predicted, accuracy, etc.
- [] Move secrets into kubeseal
- Update API to handle trading
  - [] Configure
  - [] Start with Alpaca
- [] Add testing and CI w/ Jenkins or Gitlab
- [] Publish relevant containers and helm charts

## Plan for moving to production
- Start with Terraform w/ Linode w/ 3 nodes
- Bootstrap Flux prod cluster

# Next steps
- Move over simple nginx static sites
- Move over CO EOS
  - Add health checks
- Move over everything else?
- Apply machine learning?
- Work on new game?
