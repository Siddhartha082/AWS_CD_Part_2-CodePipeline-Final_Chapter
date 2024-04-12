
# AWS Continuous Integration 

## Set Up GitHub Repository

The first step in our CI journey is to set up a GitHub repository to store our Python application's source code. If you already have a repository, feel free to skip this step. Otherwise, let's create a new repository on GitHub by following these steps:

- Go to github.com and sign in to your account.
- Click on the "+" button in the top-right corner and select "New repository."
- Give your repository a name and an optional description.
- Choose the appropriate visibility option based on your needs.
- Initialize the repository with a README file.
- Click on the "Create repository" button to create your new GitHub repository.

Great! Now that we have our repository set up, we can move on to the next step.

## Create an AWS CodePipeline
In this step, we'll create an AWS CodePipeline to automate the continuous integration process for our Python application. AWS CodePipeline will orchestrate the flow of changes from our GitHub repository to the deployment of our application. Let's go ahead and set it up:

- Go to the AWS Management Console and navigate to the AWS CodePipeline service.
- Click on the "Create pipeline" button.
- Provide a name for your pipeline and click on the "Next" button.
- For the source stage, select "GitHub" as the source provider.
- Connect your GitHub account to AWS CodePipeline and select your repository.
- Choose the branch you want to use for your pipeline.
- In the build stage, select "AWS CodeBuild" as the build provider.
- Create a new CodeBuild project by clicking on the "Create project" button.
- Configure the CodeBuild project with the necessary settings for your Python application, such as the build environment,  build commands, and artifacts.
- Save the CodeBuild project and go back to CodePipeline.
- Continue configuring the pipeline stages, such as deploying your application using AWS Elastic Beanstalk or any other suitable deployment option.
- Review the pipeline configuration and click on the "Create pipeline" button to create your AWS CodePipeline.

Awesome job! We now have our pipeline ready to roll. Let's move on to the next step to set up AWS CodeBuild.

## Configure AWS CodeBuild

In this step, we'll configure AWS CodeBuild to build our Python application based on the specifications we define. CodeBuild will take care of building and packaging our application for deployment. Follow these steps:

- In the AWS Management Console, navigate to the AWS CodeBuild service.
- Click on the "Create build project" button.
- Provide a name for your build project.
- For the source provider, choose "AWS CodePipeline."
- Select the pipeline you created in the previous step.
- Configure the build environment, such as the operating system, runtime, and compute resources required for your Python application.
- Specify the build commands, such as installing dependencies and running tests. Customize this based on your application's requirements.
- Set up the artifacts configuration to generate the build output required for deployment.
- Review the build project settings and click on the "Create build project" button to create your AWS CodeBuild project.

Fantastic! With AWS CodeBuild all set up, we're now ready to witness the magic of continuous integration in action.

## Trigger the CI Process

In this final step, we'll trigger the CI process by making a change to our GitHub repository. Let's see how it works:

- Go to your GitHub repository and make a change to your Python application's source code. It could be a bug fix, a new feature, or any other change you want to introduce.
- Commit and push your changes to the branch configured in your AWS CodePipeline.
- Head over to the AWS CodePipeline console and navigate to your pipeline.
- You should see the pipeline automatically kick off as soon as it detects the changes in your repository.
- Sit back and relax while AWS CodePipeline takes care of the rest. It will fetch the latest code, trigger the build process with AWS CodeBuild, and deploy the application if you configured the deployment stage.

 ![image](https://github.com/Siddhartha082/aws-zero-to-hero/assets/110781138/d8e6eda0-1e28-4ebc-ad5d-d48a48055804)


![image](https://github.com/Siddhartha082/aws-zero-to-hero/assets/110781138/a6a991fd-20ae-424e-8ce9-1fe2f8c043ba)

# test the Code  change / Commit in  my Repo will Trigger/ update the same in the aws codepipeline

# I commented in the Py – file 

![image](https://github.com/Siddhartha082/aws-zero-to-hero/assets/110781138/980ff5a1-7e35-410b-8eeb-340c3b30a441)

![image](https://github.com/Siddhartha082/aws-zero-to-hero/assets/110781138/a0672b2f-84bd-4700-90f6-864a61fd5482)

# Triggered The Github

![image](https://github.com/Siddhartha082/aws-zero-to-hero/assets/110781138/51acc0a3-518c-47d1-b1ce-15322770d712)

# Testing passed – the CI pipeline  

![image](https://github.com/Siddhartha082/aws-zero-to-hero/assets/110781138/84f2076e-87c6-4e54-98c0-254e6592ac69)

# code Build

![image](https://github.com/Siddhartha082/aws-zero-to-hero/assets/110781138/da691aee-96ed-4809-9b4d-abf89056962f)

![image](https://github.com/Siddhartha082/aws-zero-to-hero/assets/110781138/ddd8ca36-8b02-445f-8919-a367bbdfc09d)

![image](https://github.com/Siddhartha082/aws-zero-to-hero/assets/110781138/bff547e9-3df7-4cdc-a832-baf4be9f4bd7)

# docker hub – changed occurred

![image](https://github.com/Siddhartha082/aws-zero-to-hero/assets/110781138/faf13fad-d9e3-40de-954d-3cfbf74025bf)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/ab91959e-8eda-4f4f-bc21-e513da2808ba)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/24d06db9-d816-4481-abba-24a9ae694784)

# Create Application

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/5688fc77-641b-44ae-92eb-50ded606efaf)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/a0b0f1a0-0952-4188-8846-e194b7044af1)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/43c25293-32df-471f-acfa-6d7d25293bd0)

# now @ EC2 --- Create & Launch it

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/b98771c2-79a1-4db5-af62-1cef39f27896)

# EC2  created

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/4b9f5c3f-88ab-4a5b-9ca7-02524870d871)

# For Every resource you can create a TAG

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/6be31313-0d2b-4fe0-86ec-f5335a1dd1bd)

# Tag

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/086ac84d-9680-442c-acb6-e05d83eb8dec)

# Now install An Agent inside EC2 instance – called as codedeploy- Agent

# Steps to be followed to install Agent inside Ec2 . instance…

# https://docs.aws.amazon.com/codedeploy/latest/userguide/codedeploy-agent-operations-install-ubuntu.html

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/65d4a3d3-355b-49bd-bc87-14474039407d)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/cf2e75e1-30ce-4156-8a41-e1a374e6c5bb)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/bd99fa09-13cf-4945-864a-d3e73d02146b)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/b4253c32-4893-402d-8ddc-53722f91f6f1)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/64ddc5dd-5d5e-455c-865a-04935cd3f25a)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/747ba653-d613-434a-b4dc-f6500856330a)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/0af8e82b-0f4a-45d1-af1c-edd06fb08a76)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/f237f745-c44e-413e-9a7a-190d8d8097cd)

# Agent Created now Give permission to EC2 instance & start Communicating with Codedeploy

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/2c437be2-c509-4ad8-bfab-c568ce148859)

# create Role in IAM .. & select the Service

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/5e94bad8-9759-47bb-b100-74fb05d734b9)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/2fbd190d-75c7-4bfc-bd04-396288d9499f)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/28f933f7-8b94-43f0-907a-8bb3ae5ac5b5)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/37a6d199-7113-4ae4-84d5-444dea7b6050)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/92981e6b-e61d-48d5-aeea-b52c5888be5e)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/a0c129e3-70a1-4439-b778-94a58df34b67)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/3c35abb8-5741-41e6-a838-522c7c5928c5)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/6b8499a9-43a0-43f8-bbc7-f2de9c06f9e3)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/5b926a1b-8c04-412f-9525-47f218f948a5)

# Now Assign the role to EC2 instance 

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/e026bca5-a0d0-405d-afb0-640e2780eaa0)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/ec49f499-877c-4378-a33e-46400332779e)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/5f862256-2d40-47d0-abcd-1b445779fea7)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/67822c74-7baa-4b16-893a-9d3ee43596e2)

# configure Code Deploy

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/9cb8c649-10fb-4304-905d-286580b123e5)

# Create Deployment Groups

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/8787de3c-12aa-4205-881e-10c963721dce)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/cc72ee6d-ff1b-459a-8cdb-54a2841ce9f7)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/79d1f6f9-0af8-42c0-9bda-15e8577cb36a)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/0f01e70c-cf9c-4bdc-8195-6fa121be70dd)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/16c7ff24-1274-42c4-ba29-84031133bdf4)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/552814f1-ac5f-4f29-b2c4-051d2dc339c8)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/43df5653-72c4-41a4-8a92-52b2d1f8a01c)


![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/92640d2a-308b-4849-acc0-48c67fb821e4)

# Go to create Deployments

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/ef2132fd-ae6a-44ce-abcd-26a843bd6daa)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/e46906d4-f731-43b9-886d-ffbfb21164b0)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/237dc9aa-5836-4909-b3ab-d459cafc5cbf)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/7161ea5f-fc25-4460-9cc4-4c9ed1e4de7e)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/16df863a-db0c-44a8-9344-7e3868f606aa)

# ERROR

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/ab3fba61-c9fd-447a-9f83-5493b6059be4)

# Error as appspec.yml should be 2 root of Repository

# ERRO Log- View

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/ac7c4793-124b-4860-b131-4f02fb3d6069)

# go to Git hub Repo – copy yaml file & the map to Root 

#https://github.com/Siddhartha082/aws-devops-zero-to-hero/blob/main/day-14/simple-python-app/appspec.yml

#now Convert GITHUB REPO to Visual Studio setup .. Virtual .. by PRESSIN … DOT(.) in your keypad

#Web-Editor from GIT

# Create a file appspec.yaml

[Uploading image.png…]()

# start & Stop container

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/af2ba568-75bb-4a50-b3ad-c4e425d71cd5)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/169a9ec5-8a0a-41a8-9d04-d9ba481f8b1f)

# Ref  from My Docker hub -- @ CICD part 1 project – ci-pipeline

#GitHUB Link - Part1 - https://github.com/Siddhartha082/AWS_CICD_Part_1_CI_Pipeline_End_to_End

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/7ab8958e-3c44-48ba-ac34-3c08d91e3fed)

# now Commit 

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/9f6eff72-ebff-4de0-afa4-80cbf86227a2)

# Commit & Push

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/a3e3bfcf-fbe3-4d68-b133-c2fd034ef2ee)

# now the error in Deployment File – Delete it  or Re-create it

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/1e21af5b-08b8-4010-8c3f-c18b74f504fa)

# Recreate a new Deployment

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/c87c958b-15f8-4359-8c1e-c9e522e7f5cd)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/72f8daaa-7720-4dae-8158-c1063b3decb4)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/d029060a-3cdc-4db0-b124-c4db003aec86)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/c66042ce-d96d-4703-a557-4ed8b10f9c20)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/bf3058c0-1da2-4685-9dae-7070041acbda)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/32896853-be8b-4e54-938a-c191dc4ab03d)

# Docket install

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/85fc994c-ec2e-4c1b-97f5-42d2f63889d0)

# Retry the  Deployment

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/200a4435-8ec5-401a-8267-ee9df13574d0)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/471cba1d-b437-41c3-abb5-f7fd72571bbc)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/e6ddd5ca-d063-4bf0-a2e5-453c1caacce5)

# view Logs Executions &  ERROR Free

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/865ec996-6787-4fe2-8720-af0819de5823)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/327db69e-a0e4-4269-9d20-22640ae03ebf)

# Final Step .. go to  AWS CodePipeline

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/1ebe72a6-bb3f-481a-9c17-9d0afecd4475)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/c2b556a4-f34d-4549-b796-ee5e6b935a1f)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/9457b498-97c2-4ddf-a3e7-6262ed54ec22)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/9de85928-4573-46b8-8f50-bde9fad05229)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/c32356b4-d52c-453a-8ccf-cda1958a8a05)

# Add one more stage

# click on Edit 

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/a2721af8-9cc7-4a55-a2b1-54bfc20cfe3b)

# @ Build – click on add stage

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/94f8eda7-994d-4eb9-9f76-54c14cb8d090)

# click on Action Group

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/abce080b-2523-4d9b-b310-9907b6f662d3)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/8f3bbacb-1698-443d-9c95-0df315e89f60)

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/729a36a6-b9da-40bc-a136-4ef0eb3ffb3d)

#Click on save Button

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/3e4cbb55-f5ed-4a53-8b3d-31cfbebe7076)

# CICD- details Saved

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/b4e03fbc-e689-4a7b-8bf7-96a635426c92)

# Check the Stages

# 1st Stage- Source

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/f12d9f71-3f9d-45fa-bffb-26558c96d41a)

# 2nd Stage - Build

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/629e48db-d1b7-428d-91e5-2cb9f80c6b89)

# 3rd Stage - Code Deploy

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/711edcf2-597d-4341-959a-b3d673701ed8)

# TEST &  COMMIT IN Github .. See the Changes Below

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/08d51951-f320-469f-a577-0d1a668f7330)

# 1st Stage Success

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/28f4c24d-9fe8-4a31-b615-68701a926b0a)

# 2nd stage success

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/2b2175e9-5292-4c8a-a6b2-ec608c420eca)

# Docker Hub --- updated build stage Successful

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/767a8ef7-ec2e-469b-98b0-97be6ca1320e)

# 3rd stage – code-deploy – Failed

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/c80985e4-1413-475d-b89d-cf6788c9c3e9)


# now check in Ubuntu Terminal Docker image is been Pulled + Docker image Running stage

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/9541cdb5-11fa-462a-aaf1-028196f66c2c)

# Final Stage Deployed 

![image](https://github.com/Siddhartha082/AWS_CICD_Part_2-CodePipeline-Final_Chapter/assets/110781138/d7071dbd-7cf6-46fe-afdd-75fd68031eac)
































































