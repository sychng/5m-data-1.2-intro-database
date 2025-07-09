# Assignment

## Brief

Create an ERD for each of the following case study question.

## Instructions

Paste the answer as DBML in the answer code section below each question.

### Question 1

Construct an ERD for a social media company whose database includes information about users, their followers, and the posts that they make. Users can follow multiple users and create multiple posts.

Each entity has the following attributes:

- User: id, username, email, created_at
- Post: id, title, body, user_id, status, created_at
- Follows: following_user_id, followed_user_id, created_at

Answer:

<iframe width="560" height="315" src='https://dbdiagram.io/e/686e6ac3f413ba35080e15c7/686e6f6df413ba35080f19dd'> </iframe>

Table User {
  id int [pk, increment]
  username varchar
  email varchar
  created_at datetime
}

Table Post {
  id int [pk, increment]
  title varchar
  body varchar
  user_id varchar
  status varchar
  created_at datetime
}

Table Follows {
  following_user_id varchar
  followed_user_id varchar
  created_at datetime
}

Ref: Post.user_id > User.id // many-to-one
Ref: Follows.following_user_id > User.id // many-to-one
Ref: Follows.followed_user_id > User.id // many-to-one


### Question 2

Construct an ERD for a company that sells books online. The company has a website where customers can browse available books and add them to their shopping carts. Each cart can contain multiple books.

There are 4 entities, think of what attributes each entity should have.

- Customer
- Book
- Cart
- CartItem

Answer:

```dbml

```

## Submission

- Submit the URL of the GitHub Repository that contains your work to NTU black board.
- Should you reference the work of your classmate(s) or online resources, give them credit by adding either the name of your classmate or URL.
