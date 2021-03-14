## Posts application backend

### This application serves to fetch data from public API [JSON Placeholder](https://jsonplaceholder.typicode.com).

### Application is created using `Java` and `Spring Boot`

- Application fetches data from the API and redirects the results to the frontend part.
- Application has 2 controllers with corresponding endpoints:
1. `CommentController` - in method `getComments` uses `ApiService`  to fetch `Comment` data.
2. `PostController` - identically to `CommentController` uses `ApiService` to fetch `Post` data from external API.

- `ApiService` class is using `HttpClient` to execute `GET` request by endpoint `https://jsonplaceholder.typicode.com/comments` and `https://jsonplaceholder.typicode.com/posts` for `CommentController` and `PostController` respectively.

### In order to run the application complete the following steps
1. Download and Install [Maven](https://maven.apache.org)
2. Download the [source code](https://github.com/Likh-Alex/posts-backend)
3. Open the source code in your IDE and run `PostsApplication` class which is located in `src/main/java/com/dev/postsapp/`

### Now application is able to fetch data from external API and redirect in to frontend
In order to use the data and render it on the frontend part - please proceed with [Frontend part](https://github.com/Likh-Alex/posts-frontend) setup, if you did not finish it yet.



