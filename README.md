# Cloud-Computing  
Backend API for the TRASCAN application  

# Members
Allgiant O'Neill Feltony Asywal - C133B4KY0404    
Antonieta Aryuka Paskalia Nggotu - C269B4KX0591  

# Cloud Architecture
![Copy of cloud-architecture-trascan drawio](https://github.com/user-attachments/assets/3266cfde-6513-4309-ac99-0dc848559732)

# API ENDPOINT
[TRASCAN API Documentation](https://lacy-sting-8e9.notion.site/TRASCAN-API-15328cfc24d580c8a8a2f44c637b7e00)

## **Running the classification and articles API Locally**

- Clone the repository to your local machine and change the directory to trascan-be
```bash
git clone https://github.com/TRASCAN-app/Cloud-Computing.git
cd Cloud-Computing/trascan-be/
```

- Install All Dependencies

```bash
pip install -r requirements.txt
```

- Set Up Service Account Credentials  
  Upload the credentials.json file (downloaded from your Google Cloud Service Account) into the project directory.

- Run the server

```bash
uvicorn main:app --reload
```




