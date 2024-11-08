
# llama-on-android
A simple guide on how to install llama on your system using termux and proot-distro 
![ollama client](https://github.com/LegitCoconut/llama-on-android/blob/main/screenshots/ollama.jpg)

## Installation of proot-distro

Install termux from Fdroid or from github

 https://f-droid.org/en/packages/com.termux/

Update all the pakages in termux 
```bash
  pkg update 
```
Now install git and curl on termux
```bash
  pkg install git
  pkg install curl
```
Now clone the proot-distro repository to your home folder 
```bash
  git clone https://github.com/termux/proot-distro.git
```
Move to the proot folder and run the installation script
```bash
  cd proot-distro
  ./install.sh
```
After installation of proot list the available distro by
```bash
  proot-distro list
```
Then install ubuntu from the list and then login to ubuntu
```bash
  proot-distro install ubuntu
  proot-distro login ubunut
```
for more info use following command
```bash
  proot-distro help
```
## Installation of ollama client 

ollama client software helps you to run local LLM on your device

Install ollama by running the command in ubuntu by proot-distro
```bash
  curl -fsSL https://ollama.com/install.sh | sh
```
After installing ollama client start the service 
```bash
  ollama serve &     // runs in backround
  ollama serve      // open new session
```
Install LLM according to the ram availablility of yout phone

now use this command to list all the available LLMs in the s/m
```bash
  ollama list
```

#### For me there was an error due to time not syncing up with the current time so the LLM was not getting downloaded from their server

Install NTPDATE to sync the time of the ubuntu with actual time
```bash
  apt install ntpdate
```

#### Now continue with the installation of LLM 
```bash 
  ollama run llama3.2:1b 
```
this installs and runs the smallest and lightest LLM in your phoen 

#### please do intsall LLM which is lesser than avg available RAM 

for more LLM go to https://ollama.com/library
## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)


## Support

For support, email adisplash@gmx.com  or labzmad44@gmail.com

