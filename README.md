# Gitlab-PIPELINES
#written by Gaby tal

#this pipeline is used with Gitlab, in AWS environment.
#working with gitlab-runner

#stages:
build - build the dockerfile with nocache
test  - stage for testing. (empty)
deploy__to_ECS_repo - deploy the dockerimage to ECR repo in AWS.
deploy__to_ECS_stage - trigger the ECS stage cluster with our new image.
deploy__to_PROD - trigger the ECS production cluster with our new image.
