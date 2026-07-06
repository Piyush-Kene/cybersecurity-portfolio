Day 79 - Done ✅
- **Practical (TryHackMe)**: - Today, I completed thte John the Ripper room.
- In this room, I learn a lot about hash cracking.
- At first, I learn about the hash-id.py python script which is used for knowing the possible hash type. In below screenshot, I just used hash-id.py for checking the hash type of hash which is in the hash1.txt file.
<img width="1901" height="797" alt="Screenshot 2026-07-01 233002" src="https://github.com/user-attachments/assets/f38169f5-e634-4580-8b73-aeb04ae5822b" />
<img width="1918" height="785" alt="Screenshot 2026-07-01 232949" src="https://github.com/user-attachments/assets/eb02099c-b2ee-4ad6-af72-64f0d41c2024" />

- Then a use john with this command - [ john --format=raw-md5 --wordlist=/usr/share/wordlists/rockyou.txt hash1.txt]  and easily get the original value of hash.

<img width="882" height="512" alt="Screenshot 2026-07-04 194517" src="https://github.com/user-attachments/assets/e276cebc-2ff3-4b33-86c3-1da134c88153" />
- And do same for diffrent hash types -<img width="851" height="428" alt="Screenshot 2026-07-04 201214" src="https://github.com/user-attachments/assets/9a6b3d6a-f8d8-49e3-833f-7a792f64462e" />
<img width="882" height="473" alt="Screenshot 2026-07-04 201725" src="https://github.com/user-attachments/assets/ccb722bf-2957-4eb9-bd4f-66516295a6c1" />

then for cracking passwords in etc/shadow file in linux , I learn about unshadow which combines the content of the /etc/passwd and /etc/shadow files into a single file format that John the Ripper can read ans also about zip2john which generates an readable hash of an zip file which john can understand.
<img width="876" height="787" alt="Screenshot 2026-07-05 202329" src="https://github.com/user-attachments/assets/e7eae33d-7dae-4cc0-9491-6616c5f62b0f" />

And also learn learn about rar2john which does the same job as zip2john but for password-protected RAR archived file
<img width="865" height="587" alt="Screenshot 2026-07-05 205708" src="https://github.com/user-attachments/assets/cdbeca35-d351-4e65-98f4-4778de51fa00" />

And in this way I complete this room.
<img width="1902" height="887" alt="Screenshot 2026-07-05 211836" src="https://github.com/user-attachments/assets/29ce6a87-a7c0-4cab-83c1-a658b8efe295" />
