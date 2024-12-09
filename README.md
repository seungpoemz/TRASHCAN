# Cloud-Computing  
Backend API for the TRASCAN application  

# Members
Allgiant O'Neill Feltony Asywal - C133B4KY0404    
Antonieta Aryuka Paskalia Nggotu - C269B4KX0591  

# Cloud Architecture
![Copy of cloud-architecture-trascan drawio](https://github.com/user-attachments/assets/3266cfde-6513-4309-ac99-0dc848559732)

# API ENDPOINT
[TRASCAN API Documentation](https://lacy-sting-8e9.notion.site/TRASCAN-API-15328cfc24d580c8a8a2f44c637b7e00)

# **Setup and Deploy Using Google Cloud Services**

## **1. Setup Cloud Storage**
1. Open [Google Cloud Console](https://console.cloud.google.com/).
2. Go to **Cloud Storage** and click **CREATE**.
3. Set a unique bucket name and choose your region.
4. Set **Storage class** to **Standard** and **Access Control** to **Fine-grained**.
5. Click **CREATE**.
6. In the bucket settings, click the **three dots**, select **Edit Access**, and **Add Principal**.
7. In the **New Principal** field, enter `allUsers`, and select **Storage Object Viewer** as the role.
8. Click **Save**.

## **2. Setup Service Account**
1. Go to **IAM & Admin > Service Accounts** or [click here](https://console.cloud.google.com/iam-admin/serviceaccounts).
2. Select your project and click **Create Service Account**.
3. Name the account and select the **Storage Admin** role.
4. Go to **Keys**, click **Add Key**, then **Create new key**, and select **JSON**.
5. Download and save the **credentials.json** file.

## **3. Setup Firestore**
1. Go to **Firestore** in Google Cloud Console.
2. Click **Create Database**.
3. Choose a **Firestore mode** (Native or Datastore).
4. Select your region and click **Create Database**.

---

## **4. Deploy to Cloud Run Using Cloud Build**

### Enable Required Services
Enable Cloud Build and Container Registry services:
```bash
gcloud services enable cloudbuild.googleapis.com containerregistry.googleapis.com




