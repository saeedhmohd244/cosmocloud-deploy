# cosmocloud-deploy

This Helm chart deploys a backend, frontend, and Redis instance with the following configurations:

## Deployment Configuration

- **Backend**
  - Image: `shreybatra/sample-backend`
  - Environment Variable: `REDIS_URI=redis://redis-svc:6379`
  - Service Type: `ClusterIP`
  - Port: `8000`

- **Frontend**
  - Image: `shreybatra/sample-frontend`
  - Environment Variable: `BACKEND_URL=http://backend-svc:8000`
  - Service Type: `NodePort`
  - Port: `5175`
  - NodePort: `31000`

- **Redis**
  - Image: `redis`
  - Service Type: `ClusterIP`
  - Port: `6379`

## Installation

To install the chart, use the following command:

```sh
helm install testapp cosmocloud-deploy --atomic 

I have deployed redis as statefulset as well as simple deployment if you want to try as deployment please use the master branch
