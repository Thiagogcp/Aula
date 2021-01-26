# Guestbook with Cloud Code


The Guestbook sample demonstrates how to deploy a Kubernetes application with a front end service and a back end service using the Cloud Code extension for Visual Studio Code.

### Table of Contents
* [Getting Started](#getting-started)
    1. [Run the app locally with minikube](#run-the-app-locally-with-minikube)
    2. [Run the app remotely with Google Kubernetes Engine](#run-the-app-remotely-with-google-kubernetes-engine)
        * [Set up a GKE cluster](#set-up-a-gke-cluster)
        * [Deploy app to GKE](#deploy-app-to-gke)
* [Next steps](#next-steps)
* [Sign up for User Research](#sign-up-for-user-research)
* [Kubernetes Architecture Diagram](#kubernetes-architecture-diagram)

---

## Getting Started

### Run the app locally with minikube

1. To run your application, click on the Cloud Code status bar and select ‘Run on Kubernetes’.  

![image](./img/status-bar.png)

2. Select ‘Run locally using minikube’ when prompted. Cloud Code runs your app in a local Kubernetes cluster created using [minikube](https://minikube.sigs.k8s.io/docs/start/).

![image](./img/create-k8s-cluster.png)

3. View the build progress in the OUTPUT window. Once the build has finished, click on the front end service's URL in the OUTPUT window to view your live application.

![image](./img/kubernetes-guestbook-url.png)

4.  To stop the application, click the stop icon on the Debug Toolbar.

### Run the app remotely on Google Kubernetes Engine

#### Set up a GKE cluster

1. Navigate to the Cloud Code - Kubernetes explorer using the left side taskbar.

2. In the Google Kubernetes Engine Explorer, click '+' to create a new Google Kubernetes Engine cluster. If prompted, follow the instructions to log in to Google Cloud Platform.

![image](./img/kubernetes-explorer.png)

3. Follow the steps to configure your cluster and click "Create Cluster".

4. Once your GKE cluster has been created, it will be displayed in the Google Kubernetes Engine Explorer.

5. Your new cluster will be set as the active cluster by default. To switch clusters, right click on a different cluster in the GKE Explorer and select “Set Active Cluster”. 

![image](./img/kubernetes-explorer-new-cluster.png)

#### Deploy app to GKE

1. Click on the Cloud Code status bar and select ‘Run on Kubernetes’.
2. If prompted, confirm the current context and image registry.
3. View the build’s progress in the OUTPUT window. Once the build has finished, you can visit your deployed app by clicking the URL in the OUTPUT window.

---
## Next steps
* Try [debugging your app](https://cloud.google.com/code/docs/vscode/debug) using Cloud Code
* Navigate the [Kubernetes Engine Explorer](https://cloud.google.com/code/docs/vscode/using-the-gke-explorer)
* Learn how to [edit YAML files](https://cloud.google.com/code/docs/vscode/yaml-editing) to deploy your Kubernetes app
* [Configure an existing app](https://cloud.google.com/code/docs/vscode/setting-up-an-existing-app) to run on Cloud Code
* Enable [Cloud APIs and client libraries](https://cloud.google.com/code/docs/vscode/client-libraries)
* Manage secrets with [Secret Manager](https://cloud.google.com/code/docs/vscode/secret-manager)

For more Cloud Code tutorials and resources, check out [Awesome Cloud Code](https://github.com/russwolf/awesome-cloudclode)!

---
## Sign up for User Research

We want to hear your feedback!

The Cloud Code team is inviting our user community to sign-up to participate in Google User Experience Research. 

If you’re invited to join a study, you may try out a new product or tell us what you think about the products you use every day. At this time, Google is only sending invitations for upcoming remote studies. Once a study is complete, you’ll receive a token of thanks for your participation such as a gift card or some Google swag. 

[Sign up using this link](https://google.qualtrics.com/jfe/form/SV_4Me7SiMewdvVYhL?reserved=1&utm_source=In-product&Q_Language=en&utm_medium=own_prd&utm_campaign=Q1&productTag=clou&campaignDate=January2021&referral_code=UXbT481079) and answer a few questions about yourself, as this will help our research team match you to studies that are a great fit.

---
## Kubernetes Architecture Diagram
![Architecture Diagram](./img/diagram.png)

----