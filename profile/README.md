# ControlHub ![MIT License](https://img.shields.io/badge/License-MIT-blue.svg) [![SaaS](https://img.shields.io/badge/SaaS-Live-blueviolet)](https://control-hub.org)


**ControlHub** is a SaaS platform for centralized management of multiple computers using customizable Python scripts.

## Main Repositories

- **[Web Application](https://github.com/control-hub/controlhub-app)** — SvelteKit frontend → [control-hub.org](https://control-hub.org)  
- **[PocketBase Backend](https://github.com/control-hub/controlhub-pb)** — Extended PocketBase (Go)  
- **[Client Program](https://github.com/control-hub/controlhub-client)** — Python-based installer for each computer  
- **[Python Library](https://github.com/control-hub/controlhub-lib)** — Python library to control Windows PCs  

## Get Started

As option watch this [playlist on russian](https://www.youtube.com/watch?v=tOdoN6NBIOk&list=PLBQcTLwZqeGRtCOc6nBVxaPdsLouO8aU_&index=3)

### 1. Create a Computer

1. Go to [control-hub.org](https://control-hub.org)  
2. Register a new account (Google login supported)  
3. Create a new **team** (e.g. `My School` or `John's Team`)  
4. Create a **region** (e.g. `Room 47`, `Lab`, `Office`)  
5. Create a **computer** (name it as you wish)

### 2. Install the Client

1. Download the latest version of the [client program](https://github.com/control-hub/controlhub-client/releases)  
2. Install it on the computer you want to connect  
3. When asked for an access token:  
   - Go to the **Tokens** section  
   - Find and copy the token for your computer  
4. Go to your region and execute the `lixelv/Спать` script  
5. After ~1 second, a message will confirm successful execution

## Team Management

### Invite a New Member

1. Open your **team** → go to the **Links** tab  
2. Create a new link with required permissions (e.g. `edit_computer` to allow running scripts)  
3. Send this link to the person you want to invite

> [!CAUTION]
> Access and team permissions are very dangerous, becouse they allow user to see links, manage access and other admin stuff.

## Audit Executions

### By Computer

1. Go to the **Computers** dashboard  
2. Click on the desired computer to view its execution history  

### By User

1. Go to your **team** → open the **Members** tab  
2. Click the `...` menu for a user → select **Browse actions**

## Create Your Own Scripts

1. Go to the **Scripts** section in the sidebar  
2. Create a new script (you can make it public or keep it private)  
3. Write your Python code and save it  
4. Test it by executing it on any computer in your team

> [!NOTE]
> You may use `{{VAR}}` syntax in python code and any `{{VAR}}` code fragment will be replaced with what you like there to be,
> Also if you use `{{VARIABLE or Default value}}`, then on execution `Default value` will be placed in field `VARIABLE`

## Architecture
![image](https://github.com/user-attachments/assets/5f7a5ff1-3521-410e-916f-c8497a7c018c)

## License

This project is licensed under the MIT License.
