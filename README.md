# it
all things IT related setting up linux with windows virtual box, then diving deep into linux and blockchain development tools and technology.

### Let's Get Started
```
1. Enable the Universe Repository [https://askubuntu.com/questions/148638/how-do-i-enable-the-universe-repository]
---------------------------------------------------------------------------------------
To enable all Ubuntu software (main universe restricted multiverse) repositories use:
    sudo add-apt-repository "deb http://archive.ubuntu.com/ubuntu $(lsb_release -sc) main universe restricted multiverse"
    sudo apt-get update



2. Install cURL:
---------------------------------------------------------------------------------------
    sudo apt-get install curl



3. Install Docker [https://medium.com/@Grigorkh/how-to-install-docker-on-ubuntu-16-04-3f509070d29c]:
---------------------------------------------------------------------------------------
a. First, add the GPG key for the official Docker repository to the system:
    curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
b. Add the Docker repository to APT sources:
    
    # Use the following command to set up the stable repository. You always need the stable repository,
    # even if you want to install builds from the edge or test repositories as well.
    sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
    # Next, update the package database with the Docker packages from the newly added repo:
    sudo apt-get update
    # Make sure you are about to install from the Docker repo instead of the default Ubuntu 16.04 repo:
    apt-cache policy docker-ce

c. Finally Install Docker:
    sudo apt-get install -y docker-ce


4. Install Docker Compose:
---------------------------------------------------------------------------------------
sudo apt install docker-compose



5. Install Go Language:
---------------------------------------------------------------------------------------
a. wget https://dl.google.com/go/go1.10.3.linux-amd64.tar.gz
b. sudo tar -xvf go1.10.3.linux-amd64.tar.gz
c. sudo mv go /usr/local
d. export GOROOT=/usr/local/go
e. export GOPATH=$HOME/Projects/Proj1
f. export PATH=$GOPATH/bin:$GOROOT/bin:$PATH
g. go version (First, use the following command to check Go version.)
h. go env (Now also verify all configured environment variables using following command.)
i. Run this command in your favourite shell and then completely log out of your account and log back in (if in doubt, reboot!):

    sudo usermod -a -G docker $USER


6. Install Node.js:
---------------------------------------------------------------------------------------
curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash -
sudo apt-get install -y nodejs


7. Install Gnome Panel
---------------------------------------------------------------------------------------
You have to install gnome-panel package which comes up with ability to create a application launcher on the desktop or wherever you like. Add --no-install-recommends suffix to prevent other package that aren't necessary.

sudo apt-get install --no-install-recommends gnome-panel

After installing gnome-panel, use following command to create a launcher.

gnome-desktop-item-edit --create-new ~/Desktop
```


