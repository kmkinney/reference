# How to pull a docker image from ECR

* Make sure you have docker installed
* Run `aws sso login` to get aws cli credentials
* Navigate to ECR on the AWS console and find the repository you want
* Click on the tag of the image you want to pull
* Copy the image URI
* Run `aws ecr get-login-password --region us-west-2 | docker login --username AWS --password-stdin <paste-URI-here>`
* It should say "login successful"
* To pull the docker image, run `docker pull <paste-URI-here>`
* Next, it's easiest to create a copy with a more managable tag to run.
	* Do this by running `docker image tag <paste-URI-here> <new-tag>
* Now you can run docker containers using the image tag
	* e.g. `docker run -it <tag> bash` for a terminal inside the container
