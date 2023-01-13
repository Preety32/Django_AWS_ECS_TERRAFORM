# Django_AWS_ECS_TERRAFORM

This Project is inspired by this [Blog](https://testdriven.io/blog/deploying-django-to-ecs-with-terraform/#ecs)

all the codes & steps are given in the blog.

There are following steps in this project which you have to follow:

### 1. Create a new project directory along with a new Django project:
![Screenshot from 2023-01-13 23-28-47](https://user-images.githubusercontent.com/115537106/212388378-8e71e0eb-4ff5-4143-bcb0-2ea3189e32da.png)

Now at the web-browser you will see django page at http://127.0.0.1:8000/

![Screenshot from 2023-01-13 23-34-19](https://user-images.githubusercontent.com/115537106/212389407-93f77371-17cc-4201-9ccc-2fb791949fba.png)

### 2. Now you have to create some files & codes are give in the blog of this project.

### 3. build and tag the image and spin up a new container which is django-app all the codes are given in the blog.

![Screenshot from 2023-01-13 23-43-17](https://user-images.githubusercontent.com/115537106/212390671-3741698a-4140-4123-a411-5d2cf9992111.png)

## ECR

### 4. now you have to push the image in django-app container.
![Screenshot from 2023-01-13 23-45-49](https://user-images.githubusercontent.com/115537106/212391048-840230dd-ac8a-44ad-8c2f-a6750a16abf6.png)

## Terraform setup

### 5. you have to create many .tf files as given in the blog. after that you have to do terraform plan & terraform init.
![Screenshot from 2023-01-12 15-10-06](https://user-images.githubusercontent.com/115537106/212391925-6c168862-faa2-4031-83f8-c1f94a4185f7.png)

## Django Check

### 6. update the code as given. & at the http://localhost:8007/ping/ you will see "pong" in the screen:
![Screenshot from 2023-01-13 23-55-42](https://user-images.githubusercontent.com/115537106/212392774-c3846c02-b864-4dae-96b9-7253e39fd191.png)

### 7. use all the steps one by one, then at the end to apply all the changes you have to do "terraform apply"
![Screenshot from 2023-01-14 00-00-39](https://user-images.githubusercontent.com/115537106/212393351-e736354b-1a7c-4007-8ac5-ea557b55c311.png)

## RDS
### 8. now update all the codes one by one.

## Domain and SSL Certificate

### 9. You have to create a hosted zone in Route 53. & give access to your NS & SOA.
![Screenshot from 2023-01-14 00-04-00](https://user-images.githubusercontent.com/115537106/212393923-e67cbad4-4bc8-4800-a4b0-81e153b39251.png)
![Screenshot from 2023-01-14 00-04-13](https://user-images.githubusercontent.com/115537106/212393975-4c4848e2-36c5-4bb1-943e-6755070ddded.png)

### 10. The you have create a request for AWS Certificate:
![Screenshot from 2023-01-14 00-05-55](https://user-images.githubusercontent.com/115537106/212394264-1051252a-2828-4e71-9c37-7350b43c8b64.png)
![Screenshot from 2023-01-14 00-06-27](https://user-images.githubusercontent.com/115537106/212394273-70f4e81c-4e29-46ad-ad7e-bf8c80101a78.png)

### 10. Make some changes in code the do "Terraform apply"
![Screenshot from 2023-01-14 00-08-52](https://user-images.githubusercontent.com/115537106/212394625-3dc46fed-2b37-43f5-810b-3a74a5faec31.png)

## Nginx

### 11. Again make some changes in code as given in blog & to apply these changs use "terraform apply"
![Screenshot from 2023-01-14 00-17-10](https://user-images.githubusercontent.com/115537106/212396060-6e1eabd7-9005-45b7-b3bf-2a02bca24531.png)
![Screenshot from 2023-01-14 00-19-05](https://user-images.githubusercontent.com/115537106/212396451-7ce25773-8c58-41f4-bb9d-e0d175f2ead1.png)
![Screenshot from 2023-01-14 00-19-11](https://user-images.githubusercontent.com/115537106/212396471-3e36d51f-dfad-4060-b23f-4bac98623674.png)


## Static Files

### 12. Again you have to update or add some codes in your files & the use "terraform apply"
![Screenshot from 2023-01-14 00-11-03](https://user-images.githubusercontent.com/115537106/212395900-732562c6-8407-4d0b-8cc4-5a3a463f2f38.png)


## Allowed Hosts

### 13. Again you have to update or add some codes in your files & the use "terraform apply"
![Screenshot from 2023-01-14 00-13-14](https://user-images.githubusercontent.com/115537106/212395741-db1b5a58-1b5a-415d-a722-9f9ad88c7ec6.png)

### 14. at the end destroy your terraform infra using "terraform destroy"











