# WhatNext-Vision-Motors Salesforce Project

**WhatNext Vision Motors** — Shaping the Future of Mobility with Innovation and Excellence.

---

## Custom Objects
Custom objects are objects that can be created and modified by developers and users to meet specific project needs.

We have successfully created the following six custom objects and enabled optional features like **Allow Reports** and **Allow Search**:

1. Vehicle  
2. Vehicle Dealer  
3. Vehicle Customer  
4. Vehicle Order  
5. Vehicle Test Drive  
6. Vehicle Service Request  

---

## Data Management — Tab Creation
We created tabs for each of the above custom objects:

1. Vehicle  
2. Vehicle Dealer  
3. Vehicle Customer  
4. Vehicle Order  
5. Vehicle Test Drive  
6. Vehicle Service Request  

<img width="917" height="697" alt="image" src="https://github.com/user-attachments/assets/103a59b8-1648-459d-9b58-d22c0b0affd4" />

---

## App Management
Using **App Manager**, we created a new Lightning App.

<img width="928" height="350" alt="image" src="https://github.com/user-attachments/assets/582cd0e2-e161-4672-8b07-89eab673ec2e" />

---

## Navigation Items
We selected and arranged items to be included in the app’s navigation bar.  
Users can personalize the navigation by adding or moving items, but they **cannot remove or rename** the ones we add.  
Some items are only available for mobile or desktop and are hidden when unsupported.

<img width="867" height="706" alt="image" src="https://github.com/user-attachments/assets/6c079f82-22f3-4d49-85ce-d4a8db56f722" />

After adding the **System Administrator** profile and completing the setup, the app was successfully created.

<img width="825" height="421" alt="image" src="https://github.com/user-attachments/assets/f5e9121b-32d5-45d5-971b-bea5d95d30cc" />

---

## Data Management — Field Creation
We created custom fields for each of the previously created objects.

### 1. Vehicle Object
<img width="951" height="631" alt="image" src="https://github.com/user-attachments/assets/72da3128-0a2c-43c2-9683-843e524ac2df" />  
**Final View:**  
<img width="662" height="608" alt="image" src="https://github.com/user-attachments/assets/cdf3cc90-5d1f-4a69-afe7-4ab78b24ad4c" />

---

### 2. Vehicle Customer
<img width="952" height="637" alt="image" src="https://github.com/user-attachments/assets/72ef94a8-d70f-469c-9154-ab9b49299f03" />  
**Final View:**  
<img width="675" height="553" alt="image" src="https://github.com/user-attachments/assets/95c30287-caf2-4504-bda6-088c159fe036" />

---

### 3. Vehicle Dealer
<img width="935" height="577" alt="image" src="https://github.com/user-attachments/assets/47827d33-c6b4-4ce6-b4b2-8b5d3c1303fd" />  
**Final View:**  
<img width="651" height="542" alt="image" src="https://github.com/user-attachments/assets/67341cd7-1a5e-4ea9-bb8f-739a1b5a446f" />

---

### 4. Vehicle Order
<img width="942" height="584" alt="image" src="https://github.com/user-attachments/assets/29609151-abde-4c66-a84e-03529ca0eb68" />

---

### 5. Vehicle Service Request
<img width="940" height="560" alt="image" src="https://github.com/user-attachments/assets/b2b144ef-bbfd-4fe1-8e1b-273529624be4" />

---

### 6. Vehicle Test Drive
<img width="933" height="606" alt="image" src="https://github.com/user-attachments/assets/b306b35b-9a90-48a8-af0c-6b37ed0857be" />

---

## Automation — Record Triggered Flow

### Assign Nearest Dealer to Customer
We created and activated a **Record-Triggered Flow** that automatically assigns the nearest dealer based on the customer’s location.

<img width="950" height="723" alt="image" src="https://github.com/user-attachments/assets/0b5a8006-bd01-440b-9568-6acadc29ddd4" />  
<img width="943" height="729" alt="image" src="https://github.com/user-attachments/assets/3149ec92-bcee-4137-9d6e-7b87603f25e3" />  

**Verification:**  
<img width="769" height="522" alt="image" src="https://github.com/user-attachments/assets/0a57374a-ebf6-4e2a-a32a-58ba5c7575a5" />  
After saving, the dealer is automatically assigned:  
<img width="930" height="498" alt="image" src="https://github.com/user-attachments/assets/f7e7e817-0790-4101-9299-53f2279cff53" />

---

### Email Reminder for Test Drive
We also created a **Record-Triggered Flow** to send customers an email reminder about their scheduled test drive.

<img width="802" height="259" alt="image" src="https://github.com/user-attachments/assets/0bf44cf2-3b20-44e3-a2ec-ca60354a17d5" />

---

## Apex Classes

We developed Apex classes to automate key business processes.  

<img width="693" height="528" alt="image" src="https://github.com/user-attachments/assets/5bcbf227-20da-424e-a102-af769bbba9f5" />  

**Outcome:**  
- Vehicle status is confirmed:  
<img width="647" height="415" alt="image" src="https://github.com/user-attachments/assets/8d759f9b-f7fc-40f9-b22b-880989e4399b" />  
- Stock quantity is reduced from 300 to 299:  
<img width="668" height="504" alt="image" src="https://github.com/user-attachments/assets/dd892dbc-31cc-482d-b836-cc9021c5beb7" />  

If stock quantity reaches **zero**, this condition is also handled via Apex triggers.

---

## Batch Class
We created a batch job to fetch pending vehicle orders.  
Sorting can be added using `ORDER BY` in the query:  
- Newest first (by creation date descending)  
- Oldest first (by creation date ascending)  
- By priority or other custom fields  

Sorting ensures consistent and predictable processing in batches.

---

## Live Link
[Salesforce Org Link](https://orgfarm-0ad87e357b-dev-ed.develop.lightning.force.com/lightning/o/Vehicle_Customer__c/list?filterName=__Recent)
