## The following use case necessitates the development of a solution utilizing appropriate Azure services.

# Use Case 1: Remote Work Solution
## Background:
Contoso has 50 employees working remotely. They need a way to provide secure access to corporate applications without requiring employees to have high-end hardware.
## Use Case Objective:
Design and implement a solution that provides secure and cost-effective access to virtual desktops for employees working from different locations. The solution must be scalable.

# How I Deployed an Azure Virtual Desktop environment to address the aforementioned use case.

## Prerequisites

- An active Azure subscription
- Administrator permissions
- 
## I Created resource Group
- Select my subscription
- Name my resources group 'Lorchez_resource'
- Selected a region where i want to host my virtual machine
- ![Resource_group](https://github.com/user-attachments/assets/d6643fac-3cbe-4d30-b141-777077506727)

## I Created a Virtual network
- Select my subscription
- Select my resource group
- Name the vnet
- Selected a region where i want to host my virtual machine
- Configure security and Ip addressed
- Tagged the Vnet
  ![Create vnet](https://github.com/user-attachments/assets/2575316c-3e8a-4801-baec-35db41205c37)
![Vnet](https://github.com/user-attachments/assets/8024f77e-f2a9-4318-99b6-eb02642ec780)

## I Created a Host Pool
- Navigate to the Azure portal.
- Search for 'Azure Virtual Desktop' and select 'Host pools'.
- Click on 'Create' and provide details: 
- Subscription and resource group(which you must have previously created)
- Host pool name
- Location and validation environment
- Select the host pool type (Personal or Pooled) and the load balancing algorithm.

- Click 'Review + Create' to finalize. 
![Host pool](https://github.com/user-attachments/assets/6929733f-3d11-45f0-b76b-8f72dc2e7e18)
## I Created Session Hosts
Session hosts are virtual machines that users connect to. 
![session 1](https://github.com/user-attachments/assets/bff67c06-e557-4e3e-9e0f-3fa705c80c4e)
![Session 2](https://github.com/user-attachments/assets/4ba09874-47a2-4ae7-9fda-c8a6d24b5b7c)
![Session 3](https://github.com/user-attachments/assets/4256df99-a297-4cb9-891b-9f4d3932f4e0)
![Session host](https://github.com/user-attachments/assets/51e808c3-04ae-4662-b417-797db1bc1f16)

## I Created an Application Group
An application group contains applications that users can access.
![AVDSession 1](https://github.com/user-attachments/assets/ce62ddc0-bc41-4639-843a-60b2a0659bab)

## I Created a Workspace
A workspace is a logical container for application groups. 

## I Assigned Users to the Application Group
![Application group in workspace](https://github.com/user-attachments/assets/64960eb2-cc29-40ab-be0f-f3d4122f6deb)

## I Registered the Application Group with the Workspace
![Application group in workspace](https://github.com/user-attachments/assets/bb8053a3-f184-4333-a5d0-1a6ab5905b47)

## Testing and Verification
- Launch the Remote Desktop client or web client '(https://client.wvd.microsoft.com/arm/webclient/index.html)/'and sign in.
- Verify access to the assigned virtual desktop
![AVDSession 1](https://github.com/user-attachments/assets/17ce5ebd-de07-44a5-84ec-b536777e5db6)
![AVDSession 1](https://github.com/user-attachments/assets/53979bee-7677-4991-adac-8c7ec449bab2)
## Azure Virtual Desktop has been successfully created
![Voila](https://github.com/user-attachments/assets/65bc7ccb-9357-4b35-9ad2-463c31b246b5)
![voila2](https://github.com/user-attachments/assets/67dcbe46-7b9f-4eed-9d52-fe17a7299ffd)

# THANK YOU!
