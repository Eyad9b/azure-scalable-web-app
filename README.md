# 🚀 Deploy and Secure a Scalable Web Application on Azure  

## 📝 Overview  
This project demonstrates how to deploy a **scalable** and **secure** web application using **Azure App Services, Load Balancer, and Auto-scaling**.

---

## 🔹 Step 1: Create a Resource Group  
1. Go to **[Azure Portal](https://portal.azure.com/)**.  
2. Navigate to **Resource Groups** → Click **Create**.  
3. Enter the following details:  
   - **Name**: `MyWebApp-RG`  
   - **Region**: Select a nearby region  
4. Click **Review + Create** → **Create**.  

![Resource Group Screenshot]

---

## 🔹 Step 2: Deploy an Azure App Service (Web App)  
1. Go to **Azure Portal** → **App Services** → **Create App Service**.  
2. Enter the following details:  
   - **Subscription**: Select your subscription  
   - **Resource Group**: `MyWebApp-RG`  
   - **App Name**: `my-scalable-app`  
   - **Runtime Stack**: `Node.js / .NET / Python / PHP`  
   - **Region**: Same as Resource Group  
3. Select **Linux** as the OS.  
4. Click **Review + Create** → **Create**.  

![App Service Screenshot]

---

## 🔹 Step 3: Set Up a Load Balancer  
1. Navigate to **Load Balancers** → Click **Create Load Balancer**.  
2. Enter the following details:  
   - **Name**: `MyWebApp-LB`  
   - **Type**: Public  
   - **Resource Group**: `MyWebApp-RG`  
   - **Region**: Same as previous resources  
3. Click **Review + Create** → **Create**.  

![Load Balancer Screenshot]

---

## 🔹 Step 4: Enable Auto-Scaling  
1. Go to **App Service** → Select `my-scalable-app`.  
2. Navigate to **Scale out (App Service Plan)**.  
3. Click **Enable Auto-scaling**.  
4. Set the following values:  
   - **Min Instances**: 1  
   - **Max Instances**: 3  
   - **CPU Threshold**: 70%  
5. Click **Apply**.  

![Auto-Scaling Screenshot]

---

## 🔹 Step 5: Configure Security (HTTPS & Firewall)  
1. Go to **App Service** → `my-scalable-app`.  
2. Navigate to **TLS/SSL settings** → **Enable HTTPS Only**.  
3. Set up **Web Application Firewall (WAF)** in Azure Front Door:  
   - Go to **Azure Front Door** → **Create**.  
   - Select **WAF Policy** and enable **Prevention Mode**.  
4. Click **Save**.  

![WAF Screenshot]

---

## 🔹 Step 6: Deploy the Web App  
1. Navigate to **App Services** → Select `my-scalable-app`.  
2. Click **Deployment Center** → Choose **GitHub Actions**.  
3. Select your repository and branch for automatic deployment.  
4. Click **Save** and **Deploy**.  

![Deployment Screenshot]

---

## 📌 Conclusion  
You have successfully deployed a **scalable** and **secure** web application on Azure using:  
✅ **Azure App Service**  
✅ **Azure Load Balancer**  
✅ **Auto-scaling**  
✅ **Security Enhancements (HTTPS, WAF)**  

🎉 Your web app is now live and scalable! 🚀  

