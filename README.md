# viber-unoffical-root


## Installation: 

snap install snapcraft

sudo addgroup --system lxd
sudo adduser $USER lxd
sudo snap install lxd --channel=candidate
snap install multipass


## Build snap:
snapcraft clean
snapcraft build
sudo snap install --devmode viber-unofficial-root_0.1_amd64.snap




## Build snap in LXD:
lxd init
(accept defaults)
export SNAPCRAFT_BUILD_ENVIRONMENT=lxd 
snapcraft cleanbuild
sudo snap install --devmode viber-unofficial-root_0.1_amd64.snap
