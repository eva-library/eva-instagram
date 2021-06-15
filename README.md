# eva-instagram

This connector has been created using Instagram API, it shows how to incorporate eva conversational flow.

This application is a Spring Boot app and uses the Azure Kubernetes Service (AKS) to deploy to Azure.

## Steps

1. First of all, it is necessary to have a business app created at https://developers.facebook.com/ 
2. Once the app is open, inside the panel, look for the Instagram Grap API and select Configure. In the left bar, select the option Messenger and then, Instagram setup. 
3. In Token access, select the facebook page and instagram channel you want to connect. The Instagram account must be previously linked to a Facebook page. You can only link Instagram accounts that are business. 
4. Once selected the facebook page, instagram channel and have given corresponding permissions, you must click on Generate token. 
5. After generate the token, scroll down to add the webhook. This webhook allows you to send and receive the messages between eva and instagram. Webhook should have two services: Get and post. Both of services must have the same name. 
6. The Get service is used to answer the validation of the service, doing a two-factor authentication with a token generated by a keyword. As for the post method, it is a way to send messages to Instagram
7. Once you add webhook services (get and post) you can see the facebook pages asociated, like this: 
<a href="https://ibb.co/N76WTMp"><img src="https://i.ibb.co/1bfRzkK/webhook-v2.jpg" alt="webhook-v2" border="0"></a>
9. At the end of the associated Facebook page, you will find the edit button, click and select the permissions "messages" and "messaging_postbacks": 
<a href="https://ibb.co/RNgC0sR"><img src="https://i.ibb.co/G9dV28z/suscription-webhook.jpg" alt="suscription-webhook" border="0"></a>
