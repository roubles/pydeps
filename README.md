# pydeps

Package multiple python dependencies into a tar folder

## Install
```
curl -sSL https://raw.github.com/roubles/pydeps/v1.1/webinstall.sh | bash
```

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

## Uninstall
```
curl -sSL https://raw.github.com/roubles/pydeps/v1.1/webuninstall.sh | bash
```
