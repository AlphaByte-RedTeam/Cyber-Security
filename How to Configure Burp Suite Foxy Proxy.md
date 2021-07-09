# How to Configure Burp Suite Foxy Proxy
Foxy Proxy is Firefox extension which automatically switches an internet connection across one or more **proxy** servers based on URL patterns. And it is a tool often use by a pentester. If you want to see the complete tutorial, click on this [link](https://null-byte.wonderhowto.com/how-to/use-burp-foxyproxy-easily-switch-between-proxy-settings-0196630/)

Here is how to install and configure Firefox correctly:

### Step 1
Go to this [Link](https://addons.mozilla.org/en-US/firefox/addon/foxyproxy-standard/) to download the Foxy Proxy extensions. 
</br>

### Step 2
Click "Add to Firefox" button
![[Pasted image 20210709130950.png]]
And then click "Add"
![[Pasted image 20210709131107.png]]
After it completely installed, it'll be directed to FoxyProxy's page, which includes a changelog and a bit information.
</br>

### Step 3
Now, we have to custom the Burp Suite Proxy, by clicking on the right corner, there is a small Fox icon. That is the Foxy Proxy icon. Click into it, and then click "Options" button.
![[Pasted image 20210709131735.png]]
</br>

### Step 4
Next, click the "Add" button to add the custom Burp Suite Proxy.
![[Pasted image 20210709131942.png]]

And we will be prompt to "Add Proxy" page
![[Pasted image 20210709132155.png]]
</br>

### Step 5
With Burp Suite is running, go to the "Options" tab under "Proxy", then you can see the Burp Suite IP Address and Port.
![[Pasted image 20210709132733.png]]

- Fill the "Title or Description" with "Burpsuite" name,
- Fill the "Proxy IP Address or DNS name" with the IP Address in your Burpsuite app,
- Fill the "Port" with the matching port in your Burpsuite app.
- Next, click Save. Leave the username and password to blank.
![[Pasted image 20210709134242.png]]
</br>
![[Pasted image 20210709134414.png]]
</br>

### Step 6
Add the Burp CA (if not already done) by going to `127.0.0.1:8080` to Firefox, next click on "CA Certificate" to download the Burpsuite Port Swigger CA Certificate.
![[Pasted image 20210709134747.png]]

</br>

Go to Firefox "Preference"
![[Pasted image 20210709134851.png]]
</br>

### Step 7
Click "Privacy & Security" button. Next, scroll down to "Certificates", and then click "View Certificates" and hit the "Import Button"
![[Pasted image 20210709135119.png]]
</br>
![[Pasted image 20210709135207.png]]
</br>
![[Pasted image 20210709135309.png]]
</br>
A prompt will be asking to import the `cacert.der`, just import them where you place the file. After you import the CA Certification, you'll see the PortSwigger as the Authorities of Burpsuite application.
![[Pasted image 20210709135648.png]]
</br>