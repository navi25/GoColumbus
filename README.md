# GoColumbus
A RESTFul API using GoLang for Online Food Ordering System
The project aims at Migrating https://github.com/navi25/RestaurantAPI from Python Based Framework to Go Based Framework

Development Goals
------------------

- No change in terms of functionality from end user's perspective
- Use of [Buffalo](https://gobuffalo.io/en) framework for the development.
- Using Redis for caching layer to improve performance of the REST API

Installation
------------

Before we begin, kindly install following on your system:-

-   [Go](https://golang.org/)

How to Run the App?
-------------------

-   mkdir $GOPATH/github.com/yourUserName/
-   cd $GOPATH/github.com/yourUserName/
-   git clone <https://github.com/navi25/GoColumbus>
-   cd GoColumbus
-   go build
-   ./GoColumbus

Everything should be ready. In your browser open
<http://127.0.0.1:4646/>


REST Endpoints
--------------

There is currently only one major object in the app:-

-   **Restaurants** 
-   Menu (To be added soon)
-   Food Items (Menu Items) (To be added soon)

The endpoints and the corresponding REST operations are defined as
follows:-

-   **RESTAURANTS**
    -   <http://127.0.0.1:5000/api/v1.0/restaurants/>
        -   **GET** : This method on above URL returns all the
            restaurants available in the database in json format
        -   **POST** : This method posts a new restaurant and accept
            *application/JSON* format for the operation with "name" as
            the only and the required parameter for the JSON.
        -   **Delete** : This method deletes the given restaurant if the
            *restaurant\_id* exists.
