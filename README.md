<h1 align="center">
  api_tweetero
</h1>

<div align="center">

  <h3>Built With</h3>

  ![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=java&logoColor=white)
  ![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)
</div>

<br/>

## Description

Tweetero is a simple API for a Twitter-like app, where you can post and read messages from users.

## Features

-   Log in with name and picture url
-   Post a message
-   Get all the messages
-   Get messages from specific user


## API Reference

### User

* Sign Up
  
  ```http
  POST api/auth/sign-up
  ```

  ##### Request:

  | Body       | Type     | Description                     |
  | :--------- | :------- | :------------------------------ |
  | `username` | `string` | **Required**. valid username    |
  | `avatar`   | `string` | **Required**. valid picture url |

### Tweets

* Post a new tweet

  ```http
  POST api/tweets
  ```

  #### Request body:

  ```json
  {
    "tweet": "string"
  }
  ```


* Get all tweets

  ```http
  GET api/tweets
  ```

  #### Query strings:

  | Parameter | description              |
  | :-------- | :----------------------- |
  | `page`    | **Required** page number |

  #### Response:

  ```json
  [
    {
      "username": "string",
      "avatar": "string",
      "tweet": "string"
    },
    {
      "username": "string",
      "avatar": "string",
      "tweet": "string"
    }
  ]
  ```

* Get tweets from specific user

  ```http
  GET api/tweets/:username
  ```

  #### Path parameters:

  | Parameter  | description |
  | :--------- | :---------- |
  | `username` | username    |

  #### Response:

  ```json
  [
    {
      "username": "string",
      "avatar": "string",
      "tweet": "string"
    },
    {
      "username": "string",
      "avatar": "string",
      "tweet": "string"
    }
  ]
  ```

## Run Locally - VS code

Clone the project

```bash
  git clone https://github.com/rudarabello/api_tweetero
```

Go to the project directory

```bash
  cd tweetero-api
```

OPen vs-code 

```bash
 code .
```

Start the server clicking on Run at file ApitweeteroApplication.java in:

```bash
 /api_tweetero/src/main/java/com/api/apitweetero
```


## Made by:

<table>
  <tr>
    <td align="center"><a href="https://www.linkedin.com/in/ruda-rabello-da-silva/"><img src="https://avatars.githubusercontent.com/u/95311365?s=96&v=4" width="80px;" alt="Rudá Rabello"/><br /><sub><b>Rudá Rabello</b></sub></a><br /><a href="https://www.linkedin.com/in/ruda-rabello-da-silva/"title="Code">💻</a></td></td>
</table>

