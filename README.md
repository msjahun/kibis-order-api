# API plugin for KibrisOrder

This plugin provides a RESTful API for managing resources in KibrisOrder.

## What is a RESTful API?


HTTP requests are often the way that you interact with a RESTful API.
A client makes an HTTP request to a server and the server responds with an HTTP response.

In a HTTP request, you need to define the type of action that you want to perform against a resource. There are four primary actions associated with any HTTP request (commonly referred to as CRUD):

**POST** (Create)

**GET** (Retrieve)

**PUT** (Update)

**DELETE** (Delete)

A resource is a data object that can be accessed via an HTTP request. The API allows you to “access your KibrisOrder site’s data (resources) through an easy-to-use HTTP REST API”. In the case of the most recent version of the API (KibrisOrder version 3.80), the resources include the following 7 KibrisOrder objects:

[**Customers**](Customers.md)

[**Products**](Products.md)

[**Categories**](Categories.md)

[**ProductCategoryMappings**](ProductCategoryMappings.md)

[**Orders**](Orders.md)

[**OrderItems**](OrderItems.md)

[**ShoppingCartItems**](ShoppingCartItems.md)

With the KibrisOrder API, you can perform any of the four CRUD actions against any of your KibrisOrder site’s resources listed above. For example, you can use the API to create a product, retrieve a product, update a product or delete a product associated with your KibrisOrder website.

## What about security?

The API plugin currently supports OAuth 2.0 Authorization Code grant type flow. So in order to access the resource endpoints you need to provide a valid AccessToken. To understand how the authorization code grant flow works . Ensure you get valid AccessToken from an Administrator in Kibrisorder.

In Order to get authorized while requesting for resources you should include an the following in the request header: <strong>Authorization: Bearer {Access Token from administrator}</strong>