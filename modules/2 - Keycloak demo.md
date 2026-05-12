# Keycloak and OAuth2 in Practice

## Keycloak

In the previous chapter we introduced the theoretical foundations of OAuth2, its authentication flows, and the concepts of access and refresh tokens.

We will now put these concepts into practice using Keycloak.

Keycloak is an OAuth2-compliant Identity Provider (IDP) developed and maintained by RedHat. It provides authentication and authorization functionalities and can be self-hosted inside distributed systems and microservice architectures.

For simplicity and reproducibility, we will run Keycloak through Docker and Docker Compose and use it to simulate real OAuth2 authentication flows.