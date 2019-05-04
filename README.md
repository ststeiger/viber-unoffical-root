# viber-unoffical-root


## Installation: 
```
snap install snapcraft
snap install multipass

sudo addgroup --system lxd
sudo adduser $USER lxd
sudo snap install lxd --channel=candidate

```

## Build snap:
```
snapcraft clean
snapcraft build
sudo snap install --devmode viber-unofficial-root_0.1_amd64.snap
```



## Build snap in LXD:
```
lxd init
(accept defaults)
export SNAPCRAFT_BUILD_ENVIRONMENT=lxd 
snapcraft cleanbuild
sudo snap install --devmode ./viber-unofficial-root_1.0_amd64.snap
```


## Run snap:
```
env BAMF_DESKTOP_FILE_HINT=/var/lib/snapd/desktop/applications/viber-unofficial-root_viber.desktop /snap/bin/viber-unofficial-root.viber %U
```
