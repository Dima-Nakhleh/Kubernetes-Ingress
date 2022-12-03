# Kubernetes-Ingress
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
