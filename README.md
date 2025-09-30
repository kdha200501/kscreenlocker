# How to

##### Install dependencies

```shell
$ sudo dnf builddep kscreenlocker
```



##### Compile and install `kwin`

```shell
$ rpm -q kscreenlocker
$ git checkout customize/v<x.y.z>
$ cmake -DCMAKE_INSTALL_PREFIX="/usr" -DKDE_INSTALL_LIBEXECDIR=libexec -B "$PWD/build/" -S "$PWD/"
$ make -C "$PWD/build/" -j"$(nproc)"
$ sudo make -C "$PWD/build/" install DESTDIR="/"
```





# Customization

##### Show the sign-in dialog in the primary screen, only
