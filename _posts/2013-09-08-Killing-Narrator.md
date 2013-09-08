---
layout: post
published: true
title: How to give Windows Narrator a terrible and painful death
---

## It will not be an honorable death.

While I was in the speaker room preparing for my talk before Austin Code Camp, I ran into a guy who was running into issues with Windows Narrator coming up randomly while he was typing. I showed him how to delete it and he said I should do a talk on it (lol).

Anyways, thought I'd share with this with all you lovely people :]

### Find that [*explitive noun*]
For me, that little [*another explitive*] was hiding in my System32 folder (C:\Windows\System32).

![Whoops! Image didn't load](https://lh5.googleusercontent.com/ZR8wfBengw2SgFB-gBkIH7v5i9KzrMP8pgT5n0PZmANIE8QzBT14ithEMKZ7eiybWw=w1828-h808)

### Own that guy.
If you try and delete Narrator.exe, Windows won't let you. We need to take ownership of the file.
Right click -> Properties -> Security tab -> Advanced button
![Whoops! Image didn't load](https://lh6.googleusercontent.com/vEr53nXXCv8i6k3FrztCcF7ew7jgTIuH1Kr_3N5nKQ8ggNKKO-NZPQ6LtR4oSvyNIg=w1828-h808)
Click the 'change' link and make yourself the user, or any group that you belong to (Administrators, Users, whatever)

### All the permissions
Give the new owner of the file the appropriate permissions (Select the user and click edit, then give the user full permissions).
![Whoops! Image didn't load](https://lh5.googleusercontent.com/R4FVmyjh_TT6rtZ3tRkhE9xoc3ClR8bRR-v6947xfHk-MCjpCGnCRL85b8YCEvkeaQ=w1828-h808)

Click ok all the way down. Windows will probably complain about security and stuff. 

### Kill it with fire
Delete it and you're done!

Well that was fun wasn't it?
