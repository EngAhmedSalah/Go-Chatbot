# Go-Chatbot
a console chat bot using java and AB API for making java AI Agent
![app](images/app.jpg?raw=true "Title")
![app2](images/app2.jpg?raw=true "Title")


# this is the private repo of WASET Project
## Contributers
salah - shimaa- 2andel - eldeeb - fero - samah

#  #
##### To run docker container for mongodb with default user and password:##
#### `$ docker run -d -p 27017:27017 --name mongodb mongo` ##
Waset Documentation
=================
   * [APIs endpoints for user service](APIs-endpoints-for-user-service)
      * [Linked List](https://github.com/EngAhmedSalah/Coding-Interview-Preparing/tree/master/Topics%20to%20Study/Linked%20List)
            
            
##APIs endpoints for user service:
#Real Cool Heading
## POST `/user/create` ##
    {
        "id": "11111",
        "phone": "0100023423",
        "userName": "Mostafa",
        "nationalIdPhoto": "photo3232.png",
        "....": "....",
        "....": "...."
    }
## GET `/user/{id}` ##

**User Service**
----
  Returns json data about a single user.

* **URLs**

  * /user/{id}
  * /user/create

* **Method:**

  `GET` , `POST`
  
*  **URL Params**

   **Required:**
 
   `id=[int]`

* **Data Params**

        id=[int] , phone=[string] , userName=[string] , nationalIdPhoto=[img]

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** `true / false`
 
* **Error Response:**

  * **Code:** 404 NOT FOUND <br />
    **Content:** `{ error : "User doesn't exist" }`

  OR

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** `{ error : "You are unauthorized to make this request." }`

* **Sample Call:**

  ```plain
    localhost:8080/user/1
  ```
  
  [Go to Real Cool Heading section](#real-cool-heading)
