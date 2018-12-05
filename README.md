# pydeps

Package multiple python dependencies into one movable tar folder. Ideal for installing dependencies on machines without internet access.

## Usage
### Create tar from requirements.txt
```
pydeps -r requirements.txt -f myfolder
```
This will create myfolder.tar.gz that can be ported to a box without internet access. Once ported, you can untar it, cd into it and run ./installdeps

### Create tar from single package
```
pydeps -p requests -f myfolder
```
This will create myfolder.tar.gz that can be ported to a box without internet access. Once ported, you can untar it, cd into it and run ./installdeps

## Install
```
curl -sSL https://raw.github.com/roubles/pydeps/v1.2/webinstall.sh | bash
```

## Uninstall
```
curl -sSL https://raw.github.com/roubles/pydeps/v1.2/webuninstall.sh | bash
```
