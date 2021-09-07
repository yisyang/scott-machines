# scott-machines
CasC storage space of new and migrated personal projects.

# Initial project

## Plan for stock project
- Bootstrap with https://github.com/fluxcd/flux2-kustomize-helm-example
- Start locally with K8s w/ robotrade namespace
- Add container with TSDB
- Add container with Couchbase
- Start new repo for new REST API
  - Adding/removing symbols to monitor (CB)
  - Ingesting 365 days of data from Alpaca into TSDB for given symbol
  - Predict 1, 2, 3, 5 days trends from historic data and actions to take
  - Evaluate predicted actions
- Add testing
- Move secrets into kubeseal
- Publish relevant containers and helm chart
- Add Flux for CD

## Plan for moving to production
- Start with Terraform w/ Linode w/ 3 nodes
- Set up Flux

# Next steps
- Move over simple nginx static sites
- Move over CO EOS
  - Add health checks
- Move over everything else?
- Apply machine learning?
- Work on new game?

