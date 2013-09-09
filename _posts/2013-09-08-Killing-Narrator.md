---
layout: post
published: true
title: "Giving Windows Narrator a terrible, painful death"
---

## It will not be an honorable death.

While I was in the speaker room preparing for my talk before Austin Code Camp, I ran into a guy who was running into issues with Windows Narrator coming up randomly while he was typing. I showed him how to delete it and he said I should do a talk on it (lol).

Anyways, thought I'd share with this with all you lovely people :]

### Find that [*explitive noun*]
For me, that little [*another explitive*] was hiding in my System32 folder (C:\Windows\System32).

![Whoops! Image didn't load](https://docs.google.com/file/d/0B77SPp78ooL1bzZxLWVMMVZXZnc/edit?usp=sharing)

### Own that guy.
If you try and delete Narrator.exe, Windows won't let you. We need to take ownership of the file.
Right click -> Properties -> Security tab -> Advanced button
![Whoops! Image didn't load](https://docs.google.com/file/d/0B77SPp78ooL1a1g4VDBaNlN3d2c/edit?usp=sharing)
Click the 'change' link and make yourself the user, or any group that you belong to (Administrators, Users, whatever)

### All the permissions
Give the new owner of the file the appropriate permissions (Select the user and click edit, then give the user full permissions).
![Whoops! Image didn't load](https://lh6.googleusercontent.com/8uOsy7UzOFZO6681VMCmRBssc_icoGAKLzVzvy0Biqdi9YGFur0f-TcflwJ0Y-xhcA=w1085-h780)

Click ok all the way down. Windows will probably complain about security and stuff. 

### Kill it with fire
Delete it and you're done!

Well that was fun wasn't it?