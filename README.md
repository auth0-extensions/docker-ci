# CI Containers

Contains docker containers used to build public Auth0 extensions related projects.

# Why

Many of our build pipelines uses docker. There are common tools that are required in our build process such as `FOSSA`, `Code Climate` and `auth0-extensions-cli` in the case of building extensions.

These containers will have these tools baked in.

# Variants

## `ci-node:latest`

This is the defacto image. It is used to build any nodejs projects.

## `ci-node:extensions`

This image has the `auth0-extensions-cli` baked in and is used in building and deploying extensions.

# Development

Checkout and modify the Dockerfiles.

## Publishing

Building and publishing is handled by docker hub's automated builds.
