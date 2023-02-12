# Installing command line tools

A good starting point are [Command line tools only](https://developer.android.com/studio#command-line-tools-only).

```bash
cd ~/Android
curl https://dl.google.com/android/repository/commandlinetools-linux-9477386_latest.zip --output commandlinetools.zip
unzip commandlinetools.zip
rm commandlinetools.zip
## A little trick: folder where tools will be reside should be exactly ~/Android/cmdline-tools/tools...
## scripts will fail otherwise 🧐
mkdir cmdline-tools/tools
mv bin/ lib source.properties NOTICE.txt tools
echo 'export PATH="~/Android/cmdline-tools/tools/bin/:$PATH"' >> ~/.bashrc
```

After that you have the main tools to start android development

By now, the two more important commands are `sdkmanager` and `avdmanager`

## sdkmanager

That command will allow you to install all needed packages in order you need them.

You can take a look of available android develop packages executing

```bash
sdkmanager --list
```

It will print a lager list of things, by now one is the most important:

`system-images*`

You can imagine them as `.iso` files in linux distros, system images are prebuild `android operative system` images

Now we have installed the tools 🔨 that will allow us configure all your android development setup, next step we will start 
installing the android emulator.
