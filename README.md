#  Network-Diagram

# 1) Setup Wazuh in VirtualBox Tutorial 
https://www.youtube.com/watch?v=Ldm9hv7Tki8

  - Install GPG key as root for Linux devices cmd: curl -s https://packages.wazuh.com/key/GPG-KEY-WAZUH | sudo gpg --no-default-keyring --keyring gnupg-ring:/usr/share/keyrings/wazuh.gpg --import
sudo chmod 644 /usr/share/keyrings/wazuh.gpg

<img width="616" height="192" alt="image" src="https://github.com/user-attachments/assets/c4485f19-a233-4fbc-a03d-bd0f00d62fe8" />


 
  
  - Add repository: echo "deb [signed-by=/usr/share/keyrings/wazuh.gpg] https://packages.wazuh.com/4.x/apt/ stable main" \
| sudo tee /etc/apt/sources.list.d/wazuh.list
<img width="622" height="126" alt="image" src="https://github.com/user-attachments/assets/cd642653-b26b-475a-8da1-835d94dbf1f6" />



 
 - Run the Wazuh Agent installer command on the device you are installing the agent onto and replace the IP address with the IP address of the Wazuh Server: WAZUH_MANAGER="10.0.0.2" sudo apt install wazuh-agent
<img width="623" height="330" alt="image" src="https://github.com/user-attachments/assets/2fcda7c0-6796-4582-bc21-73a5e630a33f" />
