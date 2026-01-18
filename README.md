# SAIC_Deliverables
# 1st Question.
After reading question number 1, there is a system in which the admin has missed somre point from where I can get access to the complete server, for this to check this, I need a virtual machine to run in device, at first i didn't understand what a VM is. After knowing that, I installed the VM
and imported the drive file into it and opened the VM of sent. After getting logged in with the given data, I started to check all files first, as there may be any clue, but None was there. So i started the commands in linux.
## The approach after getting into the VM.
I checked from the terminal if there were any files that were hidden; the result is negative. 
So I read the question again and tried to search **localhost** on Firefox, then it showed the only text **Helios Internal Dashboard**. What I thought at first, at seeing this helio -- earth, internal -- iner, dashboard-- something is shown openly, so I checked is there anything i can find in the web backend, so I used F12 key to see what was happening in the back, but this is also came negitive.
And I went into the terminal and used **ps aux | grep root**. Is there anything I will get that is in the root? And after I searched for Nginx and Apache, to see if they might running,  I came across Python files.
There i got attention with the name helios which i seen in web. so i went into that directory and seen that there are few files in that, and i am not allowed to access wroker file and i went into web directory and there i seen server.py and when i seen that i found some things that the server is trusting anothere server, this means I am a student and i can't access, but if i can go through the token_number, website i can i thought so i got token number from **/etc/helios/** directory and there seen into web.env there i got INTERNAL_TOKEN =  9877981220e470cfcc49e73d98ba5a. But also i am not getting access to worker.env after usinf curl command
# 4th Question.
**The flag I found =  SAIC{ev3n_l0g5_cAn_l13_tRu5t_n0_0n3}**
## The way I found this
First, I installed the link,
And went to the terminal and started extracting it with ** tar -xvzf chall6.tar.gz** this thing I searched how to extract the things from these types of files, I know only for .zip extensions. After this, it extracted all.
Few words got my attention like lost, lost and found. I just moved forward to check what is present in this file.
I saw in README.md that there  any direclty written  flag. But no use.
And i tried **git grep FLAG $( git rev-list--all) then also i didn't found anything.
Then I thought that there will histroy of git will not be deleted. So I recovered the lost data from **git fsck --lost-found**.  Then I got these  a3e00065651d7bb9a54c10a9157696e07903ebac,  like this number, and when I saw the ls in chall6 directory new directories showed up like oven.py, baked_goods.txt, 

I thought if these were deleted, then the flag must be in this only, so I  checked out them and i found one word flag, and i thought there is somes code encryption so there may be link with the list of numbers given in bake_goods.txt.

so I asked how to write code to decode the code because i never seen this type of encryption, i pasted code and ran it but nothing is showed, i checked and came to know that i need to find n and e still, and then i use -m in with the thing which i got earlier then i found the n and e and then given these values and then ran it, it gave the flag.


# 5th Question.
For this question, I am not able to decode the pattesrn.

After downloading the PNG file, I went into the terminal, 
And tried exiftool, which is commonly used for PNG file things, there I saw a pattern that is repeating, and I tried to write a code that can change this into a flag, but I tried so many ways. I tried these codes from AI.




