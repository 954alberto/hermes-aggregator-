# hermes-aggregator-
Hermes is a lightweight Rust-based Swagger/OpenAPI aggregator designed for Kubernetes. 
It automatically discovers microservices exposing Swagger specs, aggregates their API documentation into a unified Swagger UI endpoint, and simplifies API exploration for your teams.

# Features
Kubernetes native: discovers services labeled with expose-swagger=true

Dynamically generates Swagger UI configuration with all APIs in the cluster

Optionally proxies Swagger JSON to avoid CORS and mTLS complications

Lightweight and fast, built with Rust and actix-web

Easy to deploy alongside your microservices


# Getting Started
Label your microservices with expose-swagger=true and ensure they expose Swagger/OpenAPI JSON at /openapi.json.

Deploy hermes-aggregator in your Kubernetes cluster.

Deploy Swagger UI Helm chart configured to use hermes-aggregator’s /swagger-config.json as the configUrl.

Access the unified Swagger UI to explore all your APIs in one place.
