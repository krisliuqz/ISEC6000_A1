# ISEC6000_Assignment1_Task1
 ISEC6000_Assignment1_Task1
# Task_1. Set Up Initial Infrastructure
## Part_1. Create a Kubernetes Cluster on GKE
### Using Command Console
1. Create a Kubernetes Cluster on GKE\
First you will need to have a Google Cloud account, after you created an account you need to create a new project\
![9881726367e47006fbe35530d0d6908](https://github.com/krisliuqz/isec6000-assignment1-task1/assets/54123573/d95add82-b02b-43bd-9fd0-81718dcd448e)\
 Then you need to enable k8s API\
![645e33e1781cb8970c2572600f324ad](https://github.com/krisliuqz/isec6000-assignment1-task1/assets/54123573/6b7922f8-2ce5-4e69-8e7a-e5dd370e1770)\
  Step 1.log in to Google Cloud console on the top right\
 ![113abd6474c4d7fc2bfac1cc4fa23fc](https://github.com/krisliuqz/isec6000-assignment1-task1/assets/54123573/1877119b-c253-4ef6-bf8a-1e78a9fdacee)
  Step 2. make sure you are on the right project\
if not, using "gcloud config set project PROJECT_ID"\
```shell
gcloud config set project PROJECT_ID
```
![f76848d645515c444a7d81ca5a39f9e](https://github.com/krisliuqz/isec6000-assignment1-task1/assets/54123573/256ec3a5-6d58-4f96-970f-ee7bec6e4d35)\
  Step 3. Select a Default Compute Zone\
using "gcloud config set compute/zone us-central1-a ", alternatively you can choose whatever time zone you like\
 ```shell
gcloud config set compute/zone us-central1-a 
```
![8e3666e2070523ea6e7b89f1da524e7](https://github.com/krisliuqz/isec6000-assignment1-task1/assets/54123573/ce9cb0fa-749f-4a33-8c27-9b82954e8661)\
  Step 4. create a GKE cluster by using "gcloud container clusters create-auto isec-6000-assignment1-task1 --location=us-central1 "\
 ```shell
gcloud container clusters create-auto isec-6000-assignment1-task1 --location=us-central1 
```
![2dd611b24623601f391f8a87598188d](https://github.com/krisliuqz/isec6000-assignment1-task1/assets/54123573/be2e85af-f419-4358-8b21-e0e6a85c41d5)
It may take up for few minutes\
![bf0d781365e023cd1d9582cbf09e765](https://github.com/krisliuqz/isec6000-assignment1-task1/assets/54123573/298f1661-5572-48b1-a5fb-d85878740a9b)
Step 5. Get authentication credentials for the cluster\
![95e69160a335dca5f53191808178a9a](https://github.com/krisliuqz/isec6000-assignment1-task1/assets/54123573/72d38b5a-0f71-4bba-bae0-a048c9fcaadd)
### Using GUI
Step1. Click create to create a new GKE\
![97b8beb45bb8d42ab58ff7670e33cae](https://github.com/krisliuqz/isec6000-assignment1-task1/assets/54123573/75b3b4d8-285e-446f-8b40-8d217faffa5c)
Step2. check the configration and create.\
![d5324609276101ad47c3a39a54f58b7](https://github.com/krisliuqz/isec6000-assignment1-task1/assets/54123573/9eb767b7-af1c-4653-a669-c68ebe9a4923)
## Part_2. Install and configure kubectl to manage your Kubernetes cluster
Step 1.  navigate to the "Kubernetes Engine" > "Clusters" section and click the "Connect" button next to your cluster
![32a479bc7bc85e0056ff3a25db93579](https://github.com/krisliuqz/isec6000-assignment1-task1/assets/54123573/509d58f8-7970-4890-99f3-c56554915447)
Step 2. paste the command line into cloud console
![578ef75d5fb697c7e52b2eac35f2ce7](https://github.com/krisliuqz/isec6000-assignment1-task1/assets/54123573/53a73b9f-2ce0-4d3d-b13b-07fee11c956a)
![4ad82fd020abc9f0b08dca0fc9e5775](https://github.com/krisliuqz/isec6000-assignment1-task1/assets/54123573/19411e43-0583-46d8-be77-5a71ca315dca)
# Task_3. Set up a private GitHub repository to store your project files
Step 1. sign in to github (create one if you don't have it)
![0fe420abe09fce5758600654b3cc6f7](https://github.com/krisliuqz/isec6000-assignment1-task1/assets/54123573/062606b9-d7b6-4ea1-87ea-2d3d76f2ffe5)
Step 2. Click on the '+' icon at the top right corner of the GitHub dashboard and select "New repository."
![b2d05ff74a20f06df66fa69b9a3e5cf](https://github.com/krisliuqz/isec6000-assignment1-task1/assets/54123573/8c061aa7-8eb8-4366-b446-13f571ce9de6)
Step 3. Choose a meaningful repository name and set it to public and add a Readme file
![517ae6e68590dd88e695423872e0c7b](https://github.com/krisliuqz/isec6000-assignment1-task1/assets/54123573/c6872ae5-6959-4890-909f-065a9df71633)
