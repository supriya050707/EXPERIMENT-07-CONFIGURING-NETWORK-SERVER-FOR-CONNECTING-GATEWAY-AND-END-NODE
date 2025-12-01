### EXPERIMENT -07 CONFIGURING NETWORK SERVER FOR CONNECTING GATEWAY AND END NODE 
 
## Aim: 
To  configure the Network server and end device for transferring data on the network
## Components required: 
End node stm 32 development kit , Dragino LPS8, Network server 

## Theory :
When working with sensitive applications or files, saving progress on your local device is a start, but what if you lose access to your device? Network servers address this problem by hosting the files and programs most pertinent to the network and enabling access for consistent, real-time use. 

As a result, personnel or network clients can instantly access important data or tools while also facilitating collaboration between users. Multiple users can make changes to the same program or document for continued development over the course of a project. Via a secure login, remote users can connect to the home network.
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/59db9b76-ddd5-4d6a-9075-8db233f5e479)


In the above graphic, the circle represents an organization network where a network server facilitates collaboration and file sharing between network clients (devices).

 The role of a network server, then, is to provide users with a set of services and access to resources on the network. These features include:

Permissioned access and log-ins for network users Gateway access to the Internet for an organization Centralized location for network resources  Shared access to devices on the network like a printer or a scanner Hosts multi-user apps like email servers, web applications, or CRM

## Procedure :

 1. login to the network server using login link  https://iot.saveetha.in/
 2. Click on the nework server as shown blow
    
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/1bd434ca-1426-4102-8384-94473483543e)
 3. Click on the add gateway 
 
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/47c2e08d-6598-4437-8b07-f213d6f3b8ac)
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/e62ff028-99bc-485e-9808-fbb6e124f8b2)
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/a2e3ae58-6402-49e8-8f96-679059c1842c)
4. Click on the lora options , lora - frequency plan 

5. Click on channels and create a new channel after which you can add a new end device
   
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/1fb72be5-e48d-4cde-a329-0cfb0d29070f)

6. Add the attributes in the end device as  shown below 

 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/00bff30b-42fc-42d5-9540-285d270e41cb)
 
7.Using AT commands configure end device in serial port utility
AT Commands to set initially (Mandatory)
 AT+FDR // To do factory data reset
 AT+NJM=1 // To set OTAA mode
 AT+ADR=1 // To enable the ADR
 AT+TDC=600000 // To set the default sampling interval as 10 minutes
(Should not give below 5 minutes)
 AT+CLASS=C // To set class C
 AT+DEUI=XX XX XX XX XX XX XX XX // To set Device EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX // To set APP EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX //
To set APP Key
 ATZ // To take effective action on below settings (As like saving)



## OUTPUT 

<img width="1919" height="1065" alt="image" src="https://github.com/user-attachments/assets/42e3a2bb-cd4b-4abe-8cd0-b1d4e6495e05" />

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/01363d05-1a23-420c-9e4e-e5d306489590" />

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/fa42d52e-98de-42c3-9641-8f73464e4dbe" />

<img width="1600" height="898" alt="image" src="https://github.com/user-attachments/assets/3d8366a6-bdc1-4831-940f-f1e865614384" />

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/631aebd0-cc5e-4319-b023-8d4620637606" />


<img width="1913" height="1128" alt="Screenshot 2025-12-01 085246" src="https://github.com/user-attachments/assets/76287bea-a01f-430a-9a53-271192597a8f" />

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/cec6ae60-45a8-41cb-9f13-a7ee65b6cfc0" />

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/65e549e9-0613-4a51-8182-6226e05e656c" />

<img width="1913" height="1128" alt="Screenshot 2025-12-01 085246" src="https://github.com/user-attachments/assets/c1542a03-b44d-45fb-bab9-14ec03496115" />

<img width="1914" height="842" alt="image" src="https://github.com/user-attachments/assets/b31497f2-58d8-4dd9-ae0d-d38fbf859662" />

<img width="1908" height="778" alt="image" src="https://github.com/user-attachments/assets/b06b8358-3ea2-40d9-a456-f05bdf245e16" />

<img width="1600" height="998" alt="image" src="https://github.com/user-attachments/assets/53f18137-7e27-44fb-abb4-3f93c62eb503" />

<img width="1600" height="851" alt="image" src="https://github.com/user-attachments/assets/6e808250-0d5e-4169-8c2c-c488a96a28f1" />


![WhatsApp Image 2025-12-01 at 5 26 44 PM](https://github.com/user-attachments/assets/7689f020-c4d9-42e2-9769-f8c4a0c2a961)


<img width="911" height="942" alt="image" src="https://github.com/user-attachments/assets/9327178d-f717-424f-ab79-f301356e5309" />

<img width="932" height="1039" alt="image" src="https://github.com/user-attachments/assets/a2ae07d4-288f-437d-b58b-bad4746334b6" />

<img width="903" height="974" alt="image" src="https://github.com/user-attachments/assets/a6a581d7-5e37-40e0-b5f1-26579b7b1e85" />

![WhatsApp Image 2025-12-01 at 5 28 11 PM](https://github.com/user-attachments/assets/61371766-71f6-488f-9c47-310212cf35e1)


## Result: 

  The Network server and end device for transferring data on the network has been accomplished.
