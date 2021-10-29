# Praktikum Sistem Administrasi Server

**Kelompok 9**
# Modul 1 Virtualisasi

## Case Study
---
- vm.local
  - berisi landing page
- vm.local/blog
  - berisi blog
- vm.local/app
  - berisi aplikasi perusahaan

## Scheme
---
- Virtual Box Ubuntu Server IP : 192.168.1.100

- LXC Debian Server 9 php5.6 IP : 10.0.3.102

- LXC Ubuntu Server 18.04 php7.4 IP : 10.0.3.101

- LXC Ubuntu Server 16.04 IP : 10.0.3.103

## Problem Solving
---
- **Make sure set to bridge adapter and set ip static**

![1](https://user-images.githubusercontent.com/80197844/138592804-fee25f34-a18f-4ca9-bba2-2d0fc034a57e.png)

- **Check lxc on ubuntu in the previous practicum practice**

![2](https://user-images.githubusercontent.com/80197844/138593056-2167ed34-44d7-449b-b336-8f1514d53efa.png)

**1. Change ubuntu 5.6 to ubuntu landing**

![3](https://user-images.githubusercontent.com/80197844/138593617-06001710-9c9b-429a-a799-eb99f5d939c2.png)

- **Start lxc php landing and php 7**

![4](https://user-images.githubusercontent.com/80197844/138594052-b4c162d8-dd1a-4de1-bb2f-8437545e1c17.png)

- **Login to ubuntu landing**

![5](https://user-images.githubusercontent.com/80197844/138594072-a043f239-6127-42b0-9ccc-bf934f6a71d6.png)

- **Change ip ubuntu landing**

![6](https://user-images.githubusercontent.com/80197844/138594123-460a504a-9007-44d4-b3c8-cafb5917e00b.png)

- **Restart ip, then check ip using ifconfig**

![7](https://user-images.githubusercontent.com/80197844/138594167-6efca5d3-c8d4-41ed-8067-dc96b7cb19a6.png)

- **Exit ubuntu landing**

![9](https://user-images.githubusercontent.com/80197844/138594251-b342ef8d-d6d9-4958-8e96-c90b8dedebd4.png)

**2. Check internet connection by ping google.com / 8.8.8.8 / 1.1.1.1**

![10](https://user-images.githubusercontent.com/80197844/138594474-2de9fe63-8012-4d45-87e0-eebb2f33b46f.png)

- **Install LXC debian**

![11](https://user-images.githubusercontent.com/80197844/138594504-ceb3c85e-8b8a-437a-bc10-b93286df210a.png)
![12](https://user-images.githubusercontent.com/80197844/138594507-55ed8d36-0c65-4bc7-9a47-16af7c4341be.png)

- **Check debian LXC**

![13](https://user-images.githubusercontent.com/80197844/138594596-f9e6f681-1d67-4b60-901c-8f1ed5882e56.png)

**3. Start LXC debian**

![14](https://user-images.githubusercontent.com/80197844/138594642-a8ade8a8-f0cb-4a7b-8eae-966ba413d0f1.png)

- **Install nginx dan nginx-extras**

![15](https://user-images.githubusercontent.com/80197844/138594688-f407c07d-6bb5-4339-9c90-e0298fa214cb.png)

- **Set ip static debian php**

![16](https://user-images.githubusercontent.com/80197844/138594713-2735ab8d-326e-4342-860b-01d008e7c606.png)

- **Restart settings and check ip**

![17](https://user-images.githubusercontent.com/80197844/138594745-3e95b26d-57e6-498a-b79d-3cfb3981123f.png)

- **Setting nginx**

![18](https://user-images.githubusercontent.com/80197844/138594779-09c4ee98-18cc-4948-b80b-2828b1da9d4c.png)
![19](https://user-images.githubusercontent.com/80197844/138594801-17aeddb4-2406-407a-9c09-944fd28e0c44.png)
![20](https://user-images.githubusercontent.com/80197844/138594924-99997aa8-e8c2-45d7-8317-f01be0fccb9e.png)
![21](https://user-images.githubusercontent.com/80197844/138594928-2f6857d6-7e1b-472d-a525-8be97720a7dd.png)
![22](https://user-images.githubusercontent.com/80197844/138594933-67e1e583-fc6e-4c61-b484-a8100c464e4f.png)
![22](https://user-images.githubusercontent.com/80197844/138594941-306011bd-94ee-4d5b-b0a7-8ae051f259b7.png)

- **Test with curl**

![23](https://user-images.githubusercontent.com/80197844/138595011-3c8b12e6-bf5a-4a7b-92c7-a11b7e7a006a.png)
- **Exit from Debian PHP**

**4. Enter ubuntu landing and setting nginx**

![24](https://user-images.githubusercontent.com/80197844/138595085-fa18df8b-e66c-4413-9dfc-0ad1c8a89dd0.png)
![25](https://user-images.githubusercontent.com/80197844/138595110-3db17013-c91a-4f4c-9a6c-d644b8ca7860.png)
![26](https://user-images.githubusercontent.com/80197844/138595113-1ec33a82-eda5-4942-a392-383b75205240.png)
![27](https://user-images.githubusercontent.com/80197844/138595117-3dbecab9-378f-4334-bb81-bb63607a7788.png)

- **Change lxc_php5.6 to lxc_landing**

![28](https://user-images.githubusercontent.com/80197844/138595218-ff07cdf9-4c83-4174-9630-a33e919f3ef6.png)
![29](https://user-images.githubusercontent.com/80197844/138595223-810098e2-0500-4c50-bbb3-8275a700c667.png)
![30](https://user-images.githubusercontent.com/80197844/138595242-db301887-0555-4ab3-b3c1-93eaace3601e.png)

- **Test with curl**

![31](https://user-images.githubusercontent.com/80197844/138595258-d9fd7056-38b8-4a7a-af92-31c4fe896f38.png)
- **Exit from ubuntu landing**

**5. Stop ubuntu landing and check**

![32](https://user-images.githubusercontent.com/80197844/138595306-ff3602d9-1da5-4c84-b3ba-c13d16f50144.png)

- **Go to the /var/lib/lxc directory and check if there are any directories**

![33](https://user-images.githubusercontent.com/80197844/138595336-2a5606d7-a763-4d04-b6b6-71c6cf424fcb.png)

- **Because it will use auto start on ubuntu landing, add config like below**

![34](https://user-images.githubusercontent.com/80197844/138595400-ad7336ea-e210-49b1-8c95-abad30b45577.png)

- **Check auto start by rebooting**

![35](https://user-images.githubusercontent.com/80197844/138595456-ead51e7a-a373-4e3e-85aa-ce67f277cc4f.png)

**6. Setup nginx on local vm**

![35](https://user-images.githubusercontent.com/80197844/138595682-ad97ac69-3d4c-4763-bbdc-37d4b6834a51.png)
![36](https://user-images.githubusercontent.com/80197844/138595699-5665ba56-fc60-43b5-83df-23732bb9ad26.png)
![37](https://user-images.githubusercontent.com/80197844/138595700-046eaf93-4f86-4676-bce6-04b10c7356c4.png)
![38](https://user-images.githubusercontent.com/80197844/138595702-d4ee5e8a-44b8-4f57-bd63-7ef01930534a.png)

**7. a. Accessing http://vm.local will be redirected to http://lxc_landing.dev** 
![40](https://user-images.githubusercontent.com/80197844/138595710-1ac197c5-8a17-4762-9c72-eb0f45648516.png)
![41](https://user-images.githubusercontent.com/80197844/138595714-5ae8a473-ae94-47fa-8218-aa478c312e97.png)

b. **Accessing http://vm.local/blog will be redirected to http://lxc_php7.dev**
![42](https://user-images.githubusercontent.com/80197844/138595718-8eecfd96-cef7-4a8d-b1f1-75bb45121210.png)
![43](https://user-images.githubusercontent.com/80197844/138595721-58e13f4b-2d68-4df2-824c-d3622ecb006a.png)

c. **Accessing http://vm.local/app will redirect to http://lxc_php5.dev**
![44](https://user-images.githubusercontent.com/80197844/138595724-c3478b05-7929-447f-8e56-001f8b774ec3.png)
![45](https://user-images.githubusercontent.com/80197844/138595727-9ce73154-0eca-4ddf-b650-5bd227852c54.png)

# **Analysis**
1. Why we can't use ubuntu 16.04 for php5.6 needs, and we have to change the OS to debian 9?
2. Why we have to use LXC Virtualization for website scheme that will be developed?
3. What is a proxy server? Why we think of vm.local as a proxy server?

# **Answer Question**
1. on ubuntu 16.04 it is no longer supported by the support system or because of software like security, php5.6 etc which expires in april 2021 so need to replace debian 9 which will be supported until 2022.
2. Because the use of lxc virtualization is more resource efficient, makes it easier to manage servers, and can run various other types of operating systems.
3. The proxy server is an intermediary system for network access, because vm.local has been configured to bypass the virtual machine network to connect to the virtualization os or container that has been created so that when we can directly access the website that has been created through a local computer browser.

# Create By 
- 1202199005  Difa Taufiqurahman
- 1202190035  Alvyano Rizqilla R

