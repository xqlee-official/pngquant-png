# Description
The source code of pngquant-png was not written by me, but from the sharing of Gitub Share https://github.com/qwertme/OpenViewerFX

OpenViewerFX 6.6.14 is also the last release to include all kinds of image processors, especially PNG, and I'm just going to move the png code here

#Description of the compression algorithm
The implementation of the pngquant algorithm has a good compression effect, and does not contain any third-party dependencies on a few Java files

## Usage
maven deps
```xml
<dependency>
    <groupId>com.xqlee.image</groupId>
    <artifactId>pngquant-png</artifactId>
    <version>1.0.0</version>
</dependency>
```

````java
String srcFile="C:\\Users\\xqlee\\Desktop\\test\\swagger_logo.png";
String outFile="C:\\Users\\xqlee\\Desktop\\testout\\swagger_logo.png";
try (FileInputStream fis=new FileInputStream(srcFile);
     FileOutputStream fos=new FileOutputStream(outFile)){
    PngCompressor.compress(fis,fos);
}
````

# LICENSE
Under the terms of the GNU Lesser General Public
License as published by the Free Software Foundation; either
version 2.1
