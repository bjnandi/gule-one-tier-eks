# README #

1) Install AWS cli
2) Install Eksctl 
3) Install Kubectl

4) Create Cluster
  eksctl create cluster -f cluster.yaml

5) Run
  create_iam_role.sh
  
6) Run
  eksctl create iamidentitymapping --cluster basic-cluster --arn arn:aws:iam::888276918709:role/CodeBuildKubectlRole --group system:masters --username CodeBuildKubectlRole

7) Run for View  IAM 
  kubectl get configmaps aws-auth -n kube-system -o yaml > aws-auth.yaml
  
8) Create Build 

9) Create Pipeline

################################################################################

This README would normally document this Docker Build veriables

AWS_DEFAULT_REGION

AWS_ACCOUNT_ID

IMAGE_REPO_NAME

AWS_CLUSTER_NAME

DEPLOYMENT_NAME

IMAGE_TAG

------------------------------------------------------------------------

This README would normally document how to deploy this Dockerfile

DEMO VALUES<br />

ENV APP_DB=laravel<br />
ENV APP_DB_USER=laraveluser<br />
ENV APP_DB_PASS=laravelpass<br />
ENV DB_FILE=bahonbdc_ticket.sql<br />
ENV WEB_SERVER=127.0.0.1<br />
ENV GIT_REPO=https://github.com/bjnandi/glue-one-tier.git<br />
ENV GIT_BRANCH=main<br />
ENV GIT_APP_FOLDER=.<br />
