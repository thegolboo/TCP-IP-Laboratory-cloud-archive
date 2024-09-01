# PNETLab

# Installation

### Step 1: Download and Deploy
[Download](https://pnetlab.com/pages/download) the `.ova` file and deploy it on virtualization platforms such as VMWare.

#### 1.
<img src="https://github.com/user-attachments/assets/fd5ef2b9-ca5a-4da7-96a4-0c0a52aae15f" length="800" width="600"/>

#### 2.
<img src="https://github.com/user-attachments/assets/59843ef2-ce5f-4e95-90d8-d47dcb00b3bd"/>

#### 3.
<img src="https://github.com/user-attachments/assets/4fdd2e9e-2021-4ae1-a0f4-941b56dfffd5" length="600" width="500"/>

#### 4.
<img src="https://github.com/user-attachments/assets/b1c38994-d404-4428-99ac-f920bfb8a491" length="1000" width="800"/>

#### 5.
<img src="https://github.com/user-attachments/assets/c6110652-e354-43df-a8df-11719e3eaaa2" length="1000" width="800"/>

#### 6.
<img src="https://github.com/user-attachments/assets/18018e6d-6956-4d56-8fb3-d278cd399016"/>

#### 7.
<img src="https://github.com/user-attachments/assets/1dbec741-2c5c-4df4-a31b-e01a06f2df88" length="600" width="500"/>

#### 8.
<img src="https://github.com/user-attachments/assets/7054fdc1-b6b4-45a9-b443-74fcde06a470" length="600" width="500"/>
<br/><br/>

Then turn on the PNETLab machine and wait until you see a screen with the IP address. 
- **Username**: `root`
- **Password**: `pnet`

<img src="https://github.com/user-attachments/assets/e04b459f-2aba-494a-9d84-40ae32ce7610"/>

### Step 2: Register and Login
Use the IP address to access the PNETLab from the browser.  
Login to the PNETLab using the following credentials:
- **Username**: `root`
- **Password**: `pnet`

<img src="https://github.com/user-attachments/assets/c1f83889-2cc9-4b9e-bc8c-66cd8696204f"/>
<br/>
<img src="https://github.com/user-attachments/assets/db900365-8f53-4b25-92da-b6764d7e093c"/>

# How to Upgrade PNETLab?

#### 1. 
Access [link](https://pnetlab.com/pages/releases) to download the upgrade package. <br/>
For all of the versions till version **4.2.10**, you have to upgrade step by step from your current version to the latest version. (E.g you can upgrade **4.2.0** > **4.2.1** > **4.2.2** . But you can not upgrade from **4.2.0** > **4.2.2** it may be get the error.) However from version **5.2.7**, you can update directly to the latest version. <br/>
After Download the upgrade patch package. Copy it to **/tmp** folder of PNETLab.
<br/><br/>
<img src="https://github.com/user-attachments/assets/662e1019-29bb-4b23-9f9d-7a2eacbb156d"/>

#### 2.
SSH to PNETLab with root account and run command to check:
- `cd /tmp`
- `ls -l`

<img src="https://github.com/user-attachments/assets/489ce234-07a0-46f3-9e6e-ce44dc57a1d6"/>

#### 3.
Unzip upgrade package by command:
- delete old upgrade folder if exist by command: `rm -rf upgrade`
- `unzip [package] -d ./upgrade` (Eg: `unzip 4.0.1.zip -d ./upgrade`)
- Check again by command : `ls -l` . You should see the upgrade folder

<img src="https://github.com/user-attachments/assets/273a909e-7c42-4a4b-8486-a47750f08089"/>
<br/>
<img src="https://github.com/user-attachments/assets/817681bd-8ab7-48e5-b7d6-1e64ea3a923c"/>

#### 4.
Run below commands to upgrade:
- `chmod 755 -R upgrade`
- `find upgrade -type f -print0 | xargs -0 dos2unix`
- `./upgrade/upgrade`

<img src="https://github.com/user-attachments/assets/5854b9ab-f3b2-4c3a-874f-c7c45b5c1e63"/>
<br/>
<img src="https://github.com/user-attachments/assets/84c2f208-bc78-48e6-8957-70d258261847"/>

#### 5.
Login to Web Guide and check again.
<br/><br/>
<img src="https://github.com/user-attachments/assets/cf458e4c-fa13-4051-8eb4-5b15470840e6"/>

