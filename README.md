# **SMB Folder Sharing App – PS2 & Home Network**

## **📌 Overview**  
This **Windows-based VB.NET application** simplifies **file sharing over SMB1**, enabling **PlayStation 2 (PS2) consoles**, **other Windows PCs**, and **legacy devices** to access shared folders on your home network.  

It provides an easy way to **configure SMB1, set up user permissions, and share files** using either **IP address or NetBIOS name**, ensuring full compatibility with devices like **Open PS2 Loader (OPL)** and **Windows network clients**.

---

## **🔹 Features**  
- ✅ **Dynamically Share Any Folder** – Choose any folder and share it over the network.  
- ✅ **Works for PS2 & Other Devices** – Supports **PS2 (OPL), Windows PCs, and legacy SMB1 clients**.  
- ✅ **Access via IP or NetBIOS Name** – Connect using **`\\192.168.1.X\SHARE`** or **`\\PC-NAME\SHARE`**.  
- ✅ **Uses Standard SMB Ports** – Works on **Port 445 (Direct SMB) & Port 139 (NetBIOS over TCP/IP)**.  
- ✅ **One-Click SMB1 Setup** – Enables **SMB1 protocol**, adjusts **Windows Firewall**, and **configures registry settings**.  
- ✅ **PS2 Compatibility Fix** – Automatically applies **required SMB1 & security settings** for OPL.  
- ✅ **Live User & Share Management** – Dynamically **add, remove, and manage users and shares**.  
- ✅ **Change NetBIOS Name** – Customize your PC's network name for easier access.  
- ✅ **Custom UI & EXE Icon** – A user-friendly **Windows Forms interface** with a modern feel.  

---

## **🔧 How to Use**  
1️⃣ **Download & Run the App** (Run as Administrator).  
2️⃣ **Select a Folder** to share and assign access to a **specific user**.  
3️⃣ **Enable SMB1** (if it’s not already enabled).  
4️⃣ **Click "Fix for PS2"** to apply compatibility settings (also works for legacy SMB clients).  
5️⃣ **Access Your Shared Folder:**  
   - **Windows PCs**: Use `\\192.168.1.X\SHARE` or `\\PC-NAME\SHARE`  
   - **PS2 (OPL)**: Enter **your PC's IP or NetBIOS name** in OPL Network Settings:  
     - **Server IP**: Example: `192.168.1.100`  
     - **Share Name**: Your selected folder name.  
     - **Username**: The account assigned to the share.  
     - **Password**: Set in the app (or leave blank if guest access is enabled).  
6️⃣ **Restart your PC** (if required) and test the connection from your **PS2 or another Windows PC**.  

---

## **🌐 Connection & Ports**  
- **Port 445 (SMB over TCP/IP)** – Direct SMB connections without NetBIOS.  
- **Port 139 (NetBIOS over TCP/IP)** – Used for older devices that rely on NetBIOS.  
- Can connect using either **IP address** (`\\192.168.1.100\SHARE`) or **NetBIOS name** (`\\MY-PC\SHARE`).  

---

## **⚠️ Important Notes**  
- **Run the application as Administrator** to apply system settings.
- **SMB1 is disabled by default in modern Windows** – Enable it using **this app** or run:
  ```
  dism /online /enable-feature /featurename:SMB1Protocol
  ```
  
## **❓ Support & Feedback**
- **💬 Found a bug or need help? Open an Issue
- **🌟 If you found this useful, star the repo and share it!
