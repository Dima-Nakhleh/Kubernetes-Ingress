# Kubernetes-Ingress
## **The Purpose Of The Apps:**
this repository contains two apps:
1. Ynet-App: This app reads the news from the Ynet new service: http://www.ynet.co.il/Integration/StoryRss2.xml .
Using the spring boot, The App parses and Presents the Breaking News XML in an HTML Table Format.

1. Bitcoin-App: 
- This App Presents the Current BitCoin Price.
- Stores the price in a Redis Database.
- Presents the Average Price for the last 10 minutes

Both apps were dockerized and published on dockerhub :

[![https://github.com/Dima-Nakhleh/Kubernetes-Ingress/blob/main/images/dockerhub.GIF](https://github.com/Dima-Nakhleh/Kubernetes-Ingress/blob/main/images/dockerhub.GIF "https://github.com/Dima-Nakhleh/Kubernetes-Ingress/blob/main/images/dockerhub.GIF")](https://github.com/Dima-Nakhleh/Kubernetes-Ingress/blob/main/images/dockerhub.GIF "https://github.com/Dima-Nakhleh/Kubernetes-Ingress/blob/main/images/dockerhub.GIF")

## **Steps To Running The Apps on Minikube:**

1. **Clone This Repository.**
- git clone https://github.com/Dima-Nakhleh/Kubernetes-Ingress.git
2. **Go to the project directory:**
- cd Kubernetes-Ingress
3. **Start Minikube:**
- minikube start
4. **apply deployment:**
- kubectl apply -f .
5. **Enable ingress addon:**
- minikube addons enable ingress
6. **Start minikube tunnel:**
- minikube tunnel

-  **You can now access the apps from you browser at :** 
- http://localhost/bitcoin
- http://localhost/ynet
