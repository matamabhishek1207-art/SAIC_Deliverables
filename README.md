# SAIC_Deliverables
# 1st Question.
After reading question number 1, there is a system in which the admin has missed somre point from where I can get access to the complete server, for this to check this, I need a virtual machine to run in device, at first i didn't understand what a VM is. After knowing that, I installed the VM
and imported the drive file into it and opened the VM of sent. After getting logged in with the given data, I started to check all files first, as there may be any clue, but None was there. So i started the commands in linux.
## The approach after getting into the VM.
I checked from the terminal if there were any files that were hidden; the result is negative. 
So I read the question again and tried to search **localhost** on Firefox, then it showed the only text **Helios Internal Dashboard**. What I thought at first, at seeing this helio -- earth, internal -- iner, dashboard-- something is shown openly, so I checked is there anything i can find in the web backend, so I used F12 key to see what was happening in the back, but this is also came negitive.
And I went into the terminal and used **ps aux | grep root**. Is there anything I will get that is in the root? And after I searched for Nginx and Apache, to see if they might running,  I came across Python files.
There i got attention with the name helios which i seen in web. so i went into that directory and seen that there are few files in that, and i am not allowed to access wroker file and i went into web directory and there i seen server.py and when i seen that i found some things that the server is trusting anothere server, this means I am a student and i can't access, but if i can go through the token_number, website i can i thought so i got token number from **/etc/helios/** directory and there seen into web.env there i got INTERNAL_TOKEN =  9877981220e470cfcc49e73d98ba5a. But also i am not getting access to worker.env after usinf curl command




