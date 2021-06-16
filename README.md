# eva-instagram

This connector has been created using Instagram API, it shows how to incorporate eva conversational flow.

This application is a Spring Boot app and uses the Azure Kubernetes Service (AKS) to deploy to Azure.

## 1. Requeriments
- Facebook developers account
- Instagram enterprise account
- eva bot

## 2. Configuration

1. First of all, it is necessary to have a business app created at https://developers.facebook.com/ and click the option **My Apps**.
![](https://i.ibb.co/khcb12V/01.png=100x)

![drawing](https://i.ibb.co/khcb12V/01.png){ width=50% }

2. Once the app is open, inside the panel, look for the Instagram Grap API and select Configure. In the left bar, select the option Messenger and then, Instagram setup. 
![](https://i.ibb.co/swHLBRK/02.png)

3. In Token access, select the facebook page and instagram channel you want to connect. The Instagram account must be previously linked to a Facebook page. You can only link Instagram accounts that are business. 
![](https://i.ibb.co/Kht7GQ2/03.png)
![](https://i.ibb.co/DKZyBPP/04.png)

4. Once selected the facebook page, instagram channel and have given corresponding permissions, you must click on Generate token. 
5. After generate the token, scroll down to add the webhook. This webhook allows you to send and receive the messages between eva and instagram. Webhook should have two services: Get and post. Both of services must have the same name. 
![](https://i.ibb.co/yqYp4zF/05.png)

6. The Get service is used to answer the validation of the service, doing a two-factor authentication with a token generated by a keyword. As for the post method, it is a way to send messages to Instagram
7. Once you add webhook services (get and post) you can see the facebook pages asociated, like this: 
![](https://i.ibb.co/yqYp4zF/05.png)

9. At the end of the associated Facebook page, you will find the edit button, click and select the permissions "messages" and "messaging_postbacks": 
![](https://i.ibb.co/X7VTxt0/06.png)
