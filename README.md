# pydeps

Package multiple python dependencies into one movable tar folder. Ideal for installing dependencies on machines without internet access.

## Usage
### Create tar from requirements.txt
```
pydeps -r requirements.txt -f myfolder
```
This will create myfolder.tar.gz that can be moved to a box without internet access. Once the tar is moved, you can untar it, cd into it and run ./installdeps, as follows:

```
tar zxvf myfolder.tar.gz
cd myfolder
./installdeps
```

### Create tar from single package
```
pydeps -p requests -f myfolder
```
This will create myfolder.tar.gz that can be moved to a box without internet access. Once the tar is moved, you can untar it, cd into it and run ./installdeps, as follows:

```
tar zxvf myfolder.tar.gz
cd myfolder
./installdeps
```


### Create tar from single package at a specific version
```
pydeps -p requests==2.19.1 -f myfolder
```
This will create myfolder.tar.gz that can be moved to a box without internet access. Once the tar is moved, you can untar it, cd into it and run ./installdeps, as follows:

```
tar zxvf myfolder.tar.gz
cd myfolder
./installdeps
```

## Install
```
curl -sSL https://raw.github.com/roubles/pydeps/master/webinstall.sh | bash
```

## Uninstall
```
curl -sSL https://raw.github.com/roubles/pydeps/master/webuninstall.sh | bash
```
