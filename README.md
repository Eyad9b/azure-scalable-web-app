# azure-scalable-web-app
Azure project demonstrating how to deploy and secure a scalable web application using Azure services

# 🚀 Azure Virtual Machine Setup Guide  

## 📝 Overview  
This guide provides step-by-step instructions on how to create a Virtual Machine on **Microsoft Azure**.

---

## 🔹 Step 1: Log in to Azure  
1. Go to **[Azure Portal](https://portal.azure.com/)**  
2. Sign in with your credentials.  
3. Navigate to **Virtual Machines**.

---

## 🔹 Step 2: Create a Virtual Machine  
1. Click **Create → Virtual Machine**.  
2. Enter the following details:  
   - **Name**: `MyWebServer`  
   - **Image**: `Windows Server 2022` / `Ubuntu 22.04`  
   - **Size**: `Standard_B2s` (for testing)  
   - **Authentication**: `SSH (for Linux) / RDP (for Windows)`  
   - **VNet**: `MyProject-VNet`  
   - **Subnet**: `WebSubnet`  
3. Click **Review + Create** → **Create**  



---

## 🔹 Step 3: Configure Networking  
1. Open the **Networking** tab.  
2. Ensure **RDP (3389)** for Windows or **SSH (22)** for Linux is **allowed**.  
3. Click **Next: Disks** → **Select SSD**.  
4. Click **Review + Create**.  

![Networking Screenshot](screenshots/networking-config.png)

---

## 🔹 Step 4: Access the VM  
1. Once the VM is deployed, go to **Virtual Machines**.  
2. Select `MyWebServer`.  
3. Click **Connect**.  
4. Choose **SSH** (for Linux) or **RDP** (for Windows).  
5. Follow the instructions to connect.  



---

## 📌 Conclusion  
You have successfully created a Virtual Machine on Azure! 🎉  

