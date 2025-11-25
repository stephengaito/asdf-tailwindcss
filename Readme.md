# asdf-tailwindcss

An asdf plugin which installs the standalone command line interface for
the Tailwindcss tool

## Tailwind 4.1.x needs watchman

To install watchman from release files:

```
cd /usr/local

sudo wget https://github.com/facebook/watchman/releases/download/v2025.11.24.00/watchman-v2025.11.24.00-linux.zip

sudo mkdir tmp
sudo unzip ../watchman-v2025.11.24.00-linux.zip
sudo mv watchman-v2025.11.24.00-linux/ ..
cd ..
sudo rmdir tmp
sudo mv watchman-v2025.11.24.00-linux.zip watchman-v2025.11.24.00-linux

cd /usr/local/bin
sudo ln -s ../watchman-v2025.11.24.00-linux/bin/* .

cd /usr/local/lib
sudo ln -s ../watchman-v2025.11.24.00-linux/lib/* .

sudo mkdir -p /usr/local/var/run/watchman
cd /usr/local/var/run/watchman/
sudo chown <<localUser>>:<<localUser>> .

```