Day 08

It took me 2 days to connect with SSH on UTHO I do not have AWS.

Launched an instance on Utho 
connected with SSH. 
<img width="618" height="403" alt="day8 1" src="https://github.com/user-attachments/assets/71ab9fa5-548b-4b4f-8f1f-0635110ac686" />

Then I installed NGINX, configured the security group on Utho opened port no. 80 for the nginx webpage.
<img width="850" height="342" alt="day8 2" src="https://github.com/user-attachments/assets/dd09ed71-fda6-4f31-8c07-595916bc4892" />

Saved the log to the home directory,
<img width="856" height="68" alt="day8 3" src="https://github.com/user-attachments/assets/46eab1ed-f66e-4e3c-b28d-3fb697b524ef" />

CHALLENGES:

The main challenge was to connect on Utho server using ssh, because UTho uses OPENSSH encryption and my local system uses RSA encryption.
this was causing an invalid format of encryption, someone from discord suggested me the UTHO Documentation and I followed as it is It worked!!

basically I generated my own sshkey on the laptop and uploaded that public key to the UTHO and Deployed using that key.
