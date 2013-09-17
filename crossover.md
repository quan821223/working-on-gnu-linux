
## CrossOver

Windows 上多數的軟體在 Linux 裡都有替代方案了，但還是會有些不得不用的特殊軟體，例如 Microsoft Office, Evernote, Adobe Photoshop ... 這時可以選擇有商業支援的 CrossOver 以追求穩定。

穩定的代價就是得花點小錢，若覺得此筆開銷過高，也可等限時免費的活動。

![2013-09-16-crossovr-00.png](imgs/2013-09-16-crossover-00.png "2013-09-16-crossover-00.png")

[CrossOver 官方網站](http://www.codeweavers.com/)

下載 CrossOver 12.5.0-1 套件。

http://media.codeweavers.com/pub/crossover/cxlinux/demo/

	wget http://media.codeweavers.com/pub/crossover/cxlinux/demo/ia32-crossover_12.5.0-1_amd64.deb
 
一開始安裝時會有缺少部份套件的錯誤訊息，這時只需先行補完即可。

	$ sudo aptitude install libc6-i386 ia32-libs ia32-apt-get lib32gcc1 lib32nss-mdns lib32z1 lib32asound2 
	The following NEW packages will be installed:
	  bluez-alsa:i386{a} gcc-4.6-base:i386{a} glib-networking:i386{a} gstreamer0.10-plugins-base:i386{a} gstreamer0.10-plugins-good:i386{a} gstreamer0.10-x:i386{a} 
	  gtk2-engines:i386{a} gtk2-engines-murrine:i386{a} gtk2-engines-oxygen:i386{a} gtk2-engines-pixbuf:i386{a} gvfs:i386{a} gvfs-libs:i386{a} ia32-libs 
	  ia32-libs-multiarch:i386{a} ibus-gtk:i386{a} lib32asound2 lib32gcc1 lib32nss-mdns lib32z1 libaa1:i386{a} libacl1:i386{a} libaio1:i386{a} libao-common{a} 
	  libao4:i386{a} libasn1-8-heimdal:i386{a} libasound2:i386{a} libasound2-plugins:i386{a} libasyncns0:i386{a} libatk1.0-0:i386{a} libattr1:i386{a} 
	  libaudio2:i386{a} libaudiofile1:i386{a} libavahi-client3:i386{a} libavahi-common-data:i386{a} libavahi-common3:i386{a} libavc1394-0:i386{a} libbz2-1.0:i386{a} 
	  libc6:i386{a} libc6-i386 libcaca0:i386{a} libcairo-gobject2:i386{a} libcairo2:i386{a} libcanberra-gtk-module:i386{a} libcanberra-gtk0:i386{a} 
	  libcanberra0:i386{a} libcap2:i386{a} libcapi20-3:i386{a} libcdparanoia0:i386{a} libcomerr2:i386{a} libcroco3:i386{a} libcups2:i386{a} libcupsimage2:i386{a} 
	  libcurl3:i386{a} libdatrie1:i386{a} libdb5.1:i386{a} libdbus-1-3:i386{a} libdbus-glib-1-2:i386{a} libdrm-intel1:i386{a} libdrm-nouveau2:i386{a} 
	  libdrm-radeon1:i386{a} libdrm2:i386{a} libdv4:i386{a} libesd0:i386{a} libexif12:i386{a} libexpat1:i386{a} libffi6:i386{a} libflac8:i386{a} 
	  libfontconfig1:i386{a} libfreetype6:i386{a} libgail-common:i386{a} libgail18:i386{a} libgcc1:i386{a} libgconf-2-4:i386{a} libgcrypt11:i386{a} libgd2-xpm:i386{a} 
	  libgdbm3:i386{a} libgdk-pixbuf2.0-0:i386{a} libgettextpo0:i386{a} libgl1-mesa-dri-lts-raring:i386{a} libgl1-mesa-glx-lts-raring:i386{a} 
	  libglapi-mesa-lts-raring:i386{a} libglib2.0-0:i386{a} libglu1-mesa:i386{a} libgnome-keyring0:i386{a} libgnutls26:i386{a} libgomp1:i386{a} libgpg-error0:i386{a} 
	  libgphoto2-2:i386{a} libgphoto2-port0:i386{a} libgpm2:i386{a} libgssapi-krb5-2:i386{a} libgssapi3-heimdal:i386{a} libgstreamer-plugins-base0.10-0:i386{a} 
	  libgstreamer0.10-0:i386{a} libgtk2.0-0:i386{a} libgudev-1.0-0:i386{a} libhcrypto4-heimdal:i386{a} libheimbase1-heimdal:i386{a} libheimntlm0-heimdal:i386{a} 
	  libhx509-5-heimdal:i386{a} libibus-1.0-0:i386{a} libice6:i386{a} libidn11:i386{a} libiec61883-0:i386{a} libieee1284-3:i386{a} libjack-jackd2-0:i386{a} 
	  libjasper1:i386{a} libjpeg-turbo8:i386{a} libjpeg8:i386{a} libjson0:i386{a} libk5crypto3:i386{a} libkeyutils1:i386{a} libkrb5-26-heimdal:i386{a} 
	  libkrb5-3:i386{a} libkrb5support0:i386{a} liblcms1:i386{a} libldap-2.4-2:i386{a} libllvm3.2:i386{a} libltdl7:i386{a} libmad0:i386{a} libmikmod2:i386{a} 
	  libmng1:i386{a} libmpg123-0:i386{a} libncurses5:i386{a} libncursesw5:i386{a} libnspr4:i386{a} libnss3:i386{a} libodbc1:i386{a} libogg0:i386{a} 
	  libopenal1:i386{a} liborc-0.4-0:i386{a} libp11-kit0:i386{a} libpango1.0-0:i386{a} libpciaccess0:i386{a} libpcre3:i386{a} libpixman-1-0:i386{a} 
	  libpng12-0:i386{a} libproxy1:i386{a} libpulse-mainloop-glib0:i386{a} libpulse0:i386{a} libpulsedsp:i386{a} libqt4-dbus:i386{a} libqt4-declarative:i386{a} 
	  libqt4-designer:i386{a} libqt4-network:i386{a} libqt4-opengl:i386{a} libqt4-qt3support:i386{a} libqt4-script:i386{a} libqt4-scripttools:i386{a} 
	  libqt4-sql:i386{a} libqt4-svg:i386{a} libqt4-test:i386{a} libqt4-xml:i386{a} libqt4-xmlpatterns:i386{a} libqtcore4:i386{a} libqtgui4:i386{a} 
	  libqtwebkit4:i386{a} libraw1394-11:i386{a} libroken18-heimdal:i386{a} librsvg2-2:i386{a} librsvg2-common:i386{a} librtmp0:i386{a} libsamplerate0:i386{a} 
	  libsane:i386{a} libsasl2-2:i386{a} libsasl2-modules:i386{a} libsdl-image1.2:i386{a} libsdl-mixer1.2:i386{a} libsdl-net1.2:i386{a} libsdl-ttf2.0-0:i386{a} 
	  libsdl1.2debian:i386{a} libselinux1:i386{a} libshout3:i386{a} libslang2:i386{a} libsm6:i386{a} libsndfile1:i386{a} libsoup-gnome2.4-1:i386{a} 
	  libsoup2.4-1:i386{a} libspeex1:i386{a} libspeexdsp1:i386{a} libsqlite3-0:i386{a} libssl0.9.8:i386{a} libssl1.0.0:i386{a} libstdc++5:i386{a} libstdc++6:i386{a} 
	  libtag1-vanilla:i386{a} libtag1c2a:i386{a} libtasn1-3:i386{a} libtdb1:i386{a} libthai0:i386{a} libtheora0:i386{a} libtiff4:i386{a} libtinfo5:i386{a} 
	  libtxc-dxtn-s2tc0:i386{a} libudev0:i386{a} libunistring0:i386{a} libusb-0.1-4:i386{a} libuuid1:i386{a} libv4l-0:i386{a} libv4lconvert0:i386{a} 
	  libvisual-0.4-0:i386{a} libvisual-0.4-plugins:i386{a} libvorbis0a:i386{a} libvorbisenc2:i386{a} libvorbisfile3:i386{a} libwavpack1:i386{a} 
	  libwind0-heimdal:i386{a} libwrap0:i386{a} libx11-6:i386{a} libx11-xcb1:i386{a} libxau6:i386{a} libxaw7:i386{a} libxcb-dri2-0:i386{a} libxcb-glx0:i386{a} 
	  libxcb-render0:i386{a} libxcb-shm0:i386{a} libxcb1:i386{a} libxcomposite1:i386{a} libxcursor1:i386{a} libxdamage1:i386{a} libxdmcp6:i386{a} libxext6:i386{a} 
	  libxfixes3:i386{a} libxft2:i386{a} libxi6:i386{a} libxinerama1:i386{a} libxml2:i386{a} libxmu6:i386{a} libxp6:i386{a} libxpm4:i386{a} libxrandr2:i386{a} 
	  libxrender1:i386{a} libxslt1.1:i386{a} libxss1:i386{a} libxt6:i386{a} libxtst6:i386{a} libxv1:i386{a} libxxf86vm1:i386{a} odbcinst{a} odbcinst1debian2{a} 
	  odbcinst1debian2:i386{a} oss-compat{a} xaw3dg:i386{a} zlib1g:i386{a} 
	The following partially installed packages will be configured:
	  ia32-crossover 
	The following packages are RECOMMENDED but will NOT be installed:
	  libqt4-sql-mysql:i386 libqt4-sql-odbc:i386 libqt4-sql-psql:i386 libqt4-sql-sqlite:i386 
	0 packages upgraded, 244 newly installed, 0 to remove and 0 not upgraded.
	Need to get 80.3 MB of archives. After unpacking 252 MB will be used.
	Do you want to continue? [Y/n/?]

安裝 CrossOver

	$ sudo dpkg -i ia32-crossover_11.3.1-1_amd64.deb 
	(Reading database ... 242642 files and directories currently installed.)
	Preparing to replace ia32-crossover 11.3.1-1 (using ia32-crossover_11.3.1-1_amd64.deb) ...
	Unpacking replacement ia32-crossover ...
	Setting up ia32-crossover (11.3.1-1) ...
	Verified OK
	Processing triggers for doc-base ...
	Processing 1 changed doc-base file...
	Registering documents with scrollkeeper...

![2013-09-16-crossovr-01.png](imgs/2013-09-16-crossovr-01.png "2013-09-16-crossovr-01.png")

安裝完成！
