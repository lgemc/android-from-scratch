## Android development architecuture

First than you should know is that android is a **operative system** running (most of the time, but not only) 
in **cellphones** started and maintained by google team.

Yep, sounds pretty obious but is very important to keep that in mind.

Main android development architecture responds to this questions:
- How to write code
- How to test code
- How to build code
- How to deploy code

We will start with the most important and simple thing, **say to google tools (we will install them in the next step)** where 
will google code live.

```bash
mkdir -p Android/sdk
echo 'export ANDROID_HOME="~/Android/sdk"' >> .bashrc # you can chose another folder

