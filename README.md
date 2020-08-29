# Go language
This Repo includes exercises and small projects which i use to learn Go

### Installation

Before trying any of these examples make sure to have the `Go` binary installed on your platform.

OSX:

```bash
# Install Homebrew

/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

```bash
# Install Go

brew install go
```

Linux:

```bash
# Move into $HOME directory
cd ~

# Download the binary for your distribution
curl -O https://dl.google.com/go/go1.12.linux-amd64.tar.gz

# Verify that the downloaded binary is not corrupted. Check if the hash matches the one from downloads page
sha256sum go1.12.linux-amd64.tar.gz

# Extract the binary
tar xvf go1.12.linux-amd64.tar.gz

# Make root user the owner of Go workspace
sudo chown -R root:root ./go

# Move go directory to a standard location
sudo mv go /usr/local
```

For more details regarding `Go` installation check out

[Golang Installation](https://golang.org/doc/install)

For downloading `Go` binary for your platform checkout

[Golang Downloads](https://golang.org/dl/)

To check if you installed `Go` successfully type:

```bash
# Displays installed Go version
go version

# Displays all environment variables defined by Go
go env
```



### Set $GOPATH variable
```bash
sudo nano ~/.profile

# Linux
export GOPATH=/usr/local/go
export GOBIN=$GOPATH/bin
export PATH=$PATH:/$GOBIN

# OSX
export GOPATH=$HOME/go
export GOBIN=$GOPATH/bin
export PATH=$PATH:/$GOBIN

# Save File

# Restart shell configuration
source ~/.profile
```


