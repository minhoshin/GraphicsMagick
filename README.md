# GraphicsMagick

```
# Install build dependencies
yum install -y gcc libpng libjpeg libpng-devel libjpeg-devel ghostscript libtiff libtiff-devel freetype freetype-devel

# Get GraphicsMagick source
wget ftp://ftp.graphicsmagick.org/pub/GraphicsMagick/1.3/GraphicsMagick-1.3.9.tar.gz
tar zxvf GraphicsMagick-1.3.9.tar.gz

# Configure and compile
cd GraphicsMagick-1.3.9
./configure --enable-shared
make
make install

# Ensure everything was installed correctly
gm version

# which gm

- `tar xvzf gm.tar.gz`
- 압축 후 나온 `gm` 디렉터리를 적당한 곳에 이동(여기서는 편의상 `$HOME` 밑에 둠)
- `$HOME/.bashrc` 파일의 마지막에 다음 라인 추가
    - `export PATH=$PATH:$HOME/gm/bin`
    - `export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$HOME/gm/lib64`
- 재로그인을 하거나 `source $HOME/.bashrc` 명령을 실행하여 환경변수 새로고침
- `gm version` 으로 설치 여부 확인
- 번들의 `giftest.gif`, `jpgtest.jpg`, `pngtest.png` 파일들을 가지고 테스트해볼 것(`gm identify 파일명`)
```

