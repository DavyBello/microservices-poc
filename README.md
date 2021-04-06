# Hooli - Microservices Proof of concept

This Repo contains a demo microservices application I am currently building as I learn about microservices.

It is built with Typescript, React, Kubernetes, Skaffold and uses FusionAuth for Authentication.

**Local Setup**

- Make sure your kubernetes cluster is up and running 
- Install Nginx Ingress [here](https://kubernetes.github.io/ingress-nginx/deploy/)
- Install Skaffold [here](https://skaffold.dev/docs/install/)
- create kubernetes namespace matching the namespace in line 9 of ./skaffold.yaml - `kubectl create namespace hooli-poc`
- map the hosts defined in the ./infra/k8s/ingress-srv.yaml file to your localhost - `127.0.0.1 hooli.devl` and `127.0.0.1 auth.hooli.devl` to your hosts file
- Run `skaffold dev`
- Application is available at `http://hooli.devl`
