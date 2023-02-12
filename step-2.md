# Installing command line tools

A good starting point are [Command line tools only](https://developer.android.com/studio#command-line-tools-only).

```bash
cd ~/Android
curl https://dl.google.com/android/repository/commandlinetools-linux-9477386_latest.zip --output commandlinetools.zip
unzip commandlinetools.zip
rm commandlinetools.zip
echo 'export PATH="~/Android/cmdline-tools/bin/:$PATH"' >> ~/.bashrc
```

After that you have the main tools to start android development

By now, the two more important commands are `sdkmanager` and `avdmanager`

## sdkmanager

That command will allow you to install all needed packages in order you need them.

You can take a look of available android develop packages executing

```bash
sdkmanager --list
```
