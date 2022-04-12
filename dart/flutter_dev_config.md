## Flutter Dev Config

install:
```sh
sudo pacman -S flutter
```

add current user to group flutterusers
```sh
gpasswd -a <user> flutterusers
```

```sh
newgrp flutterusers
```

```sh
flutter config --no-analytics
```

install `android studio` and `android-sdk`
```sh
sudo pacman -S android-studio
```

check
```sh
flutter doctor
```

enable desktop support
```
flutter config --enable-linux-desktop
```

```sh
flutter devices
```

Add desktop support to an existing Flutter project(select the platforms what you need):
```sh
flutter create --platforms=windows,macos,linux .
```

```sh
flutter run
```
or
```sh
flutter run -d linux
```
