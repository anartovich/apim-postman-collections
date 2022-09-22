# Postman collections for Axway API Management products (Gateway and Manager)

Axway publishes OpenAPI spec files for API Manager and API Gateway product APIs. In some cases it is convenient to use Postman collections for quick and easy invocation of the APIs. This project offers two Postman collections and one environment:
  - API Manager API v1.4 (OpenAPI v3) collection
  - API Gateway API v1.0 (Swagger v2) collection
  - Axway API Management demo environment

The environment contains several variables that allows you to setup hostname, ports, and instance ID for gateway. 

## Using Postman collections

These are a few simple steps to use this collections (you need to have a running Axway API Management instance to use the APIs):

1. Start your Axway API Management instance
2. Import both collection and environment files located in the `./Postman-files` folder to Postman
3. Select Axway **API Management demo** in the Environment selection box
4. Modify parameters as needed to match your environment. If you don't know your gateway instance ID, you can get it using topology API. After you set it in the environment, it will be used where it is set as path variable.
5. Click each collection in the Collections view and modify **Username** and **Password** on the Authorization tab to match your API Management instance (API Manager and/or API Gateway Manager). All APIs are configured to inherit authentication from the Collection level.
6. Call any API as needed