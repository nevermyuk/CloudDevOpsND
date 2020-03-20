## [URL of LoadBalancer](http://final-serve-orjl82hz5198-1793070846.ap-southeast-1.elb.amazonaws.com/)

## Overview

![Architecture](C:\Users\zequa\Desktop\Projects\Udacity-CloudDevOps-Nanodegree\Portfolio Projects\Project 2 - Deploy a highly-available web app using CloudFormation\Architecture.png)

`Bastion Host access is hardcoded to home IP.`

`All EC2 instances are in the same ASG, 2 instances in each PRIVATE Subnet`

`Connection to S3 is through NAT Gateway not Gateway Endpoint `

## Create Stack

```bash
./create.sh stackname final-project-starter.yml serverParams.json 
```

## Update Stack

```bash
./create.sh stackname final-project-starter.yml serverParams.json 
```

## Delete Stack

```bash
./delete.sh stackname
```

