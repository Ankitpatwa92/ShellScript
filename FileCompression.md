File Compression

#### Create Tar file
A tar file is just package your files without compression. Tar file is alos known as tarball
```
tar -cvf msa.tar /home/msa/
```
c – Creates a new .tar archive file.
v – Verbosely show the .tar file progress.
f – File name type of the archive file.


#### Create tar.gz Archive File
tar.gz is compressed version of tar ball
```
tar cvzf MyImages.tar.gz /home/MyImages
```

### Create tar.bz2 Archive File
tar.bz2 is highly compressed less size file
```
tar cvfj files.tar.bz2 /home/php
```

#### Untar files
```
tar -xvf file.tar
tar -xvf file.tar.gz
tar -xvf file.tar.bz2
#####Untar files in specified Directory ##
tar -xvf file.tar -C /home/public_html/videos/
```

#### untar specific file
```
tar -xvf file.tar myfile.txt
```

#### List Content of tar Archive File
```
tar -tvf uploadprogress.tar
```

#### Create zip file
```
zip -r fileName.zip my_folder
```

#### Unzip zip file (unzip file in specific folder)
```
unzip fileName.zip

unzip fileName.zip -d /home/myfolder  

```

### Add file in existing zip file
```
zip -0 -rv myold.zip file1 file2    //use -j to add only file not folder
```
