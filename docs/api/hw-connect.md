---
title: Homewizard API
summary: How to add your own device to your ETOZ dashboard
authors: Os773
date: 20-26-2025
---

# Setting up your own device with the Homewizard API

> A guide on how to connect your own device to read your live data on our website.

Please follow this guide on a Laptop or Personal Computer.

## Step 1

Navigate to [hwenergy.app](https://hwenergy.app/) 

![The hwenergy.app website](./../assets/api/api-connect/1.png)

## Step 2

Log in on the website. This is what we call a "web app", the web variant for an existing app. It should look similar- or the same as the homewizard app on your phone.

![The Login page for hwenergy.app](./../assets/api/api-connect/2.png)  
![The dashboard for hwenergy.app](./../assets/api/api-connect/3.png)  

## Step 3

Press your right mouse button to bring up the context menu, then navigate and click to the button that reads "inspect". It will usually be the lowest button on the menu.

![The context menu on the hwenergy.app dashboard](./../assets/api/api-connect/4.png)  
![Please click inspect within the context menu](./../assets/api/api-connect/5.png)

After clicking inspect, a bigger menu should pop up on the right hand side of your screen. Depending on wether or not you've used this before- it might appear elsewhere.

![The inspection menu opens up](./../assets/api/api-connect/6.png)

## Step 4

Within the inspect menu, navigate to the "Network" tab.

![Navigating to the network tab within the inspection menu](./../assets/api/api-connect/7.png)

The site might prompt you to reload, please do if it asks.

![The network tab requests to reload the page. Click the button.](./../assets/api/api-connect/8.png)  
![The page has been reloaded and new information has appeared](./../assets/api/api-connect/9.png)

## Step 5

I have made my inspection tab wider- in order to make it easier to read.

What you see now is a table with rows, like an excel sheet. If you click a row, you will see another field pop up with more informaiton.

![The network tab displays information about the related row on the table within it.](./../assets/api/api-connect/10.png)

## Step 6

Please navigate to the tab within this new field that reads "Payload", this is where we will take the first value for your own device from.

![Navigating to the tab which reads "payload"](./../assets/api/api-connect/11.png)

Within this tab, you will see even more information. We are looking for the one which has "main_connection" as type.

![This one reads "overvoltage" as type, we need another one](./../assets/api/api-connect/12.png)
![This one does read "main_connection" as type](./../assets/api/api-connect/13.png)

Please make sure if you can also see the name "main_connection" above, within the "devices" group. Sometimes there are more "main_connection"s to a house. If both names match, you have the right one!

Right click the line below "Request Payload" and click "copy object"

![Right clicking the line below request payload brings up another context menu](./../assets/api/api-connect/14.png)
![Within this context menu, we will click copy object](./../assets/api/api-connect/15.png)

The object you have just copied is the "Device Header", head over to your ETOZ dashboard, paste the value into the "Update Header" text field, and click the save button.

![Enter the Device Header into the Update Header field.](./../assets/api/api-connect/etoz1.png)
![Do not forget to click save, in order to save the new value.](./../assets/api/api-connect/etoz2.png)

The new Device Header will be saved and you can see it in the "current header" field above the "update header" field. 

## Step 7

Next, we will get the "Device Token".  

Please head back to the [hwenergy.app](https://www.hwenergy.app) website and the network tab within the inspect menu, just as before. We will now head to the "headers" tab.

![hwenergy.app inspect network tab payload menu](./../assets/api/api-connect/16.png)
![The header tab within the network menu](./../assets/api/api-connect/17.png)

## Step 8

Please scroll down until you find the "authorization" tab

![Please scroll down](./../assets/api/api-connect/18.png)

Here you will copy the immense string of text and numbers you see. This is the authorization token. it expires every so often, and then you have to grab the new one in order for the graph to work again.

![Copy the authorization token](./../assets/api/api-connect/19.png)

This value is your "Device Token", head back to the ETOZ website and paste your device token into the "update token" field.

![Head back to the etoz dashboard and click on the update token field](./../assets/api/api-connect/etoz3.png)
![Do not forget to save this new value, too](./../assets/api/api-connect/etoz4.png)

## Result

If you have followed the steps correctly, a graph should now appear!

Well done :)

![The graph displays correctly with the correct information](./../assets/api/api-connect/etoz5.png)

Features to further implement this API may be created in the future.

