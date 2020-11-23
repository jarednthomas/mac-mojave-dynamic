# mac-mojave-dynamic

### Installation
Change directory to your Pictures folder.
```sh
cd Pictures
```

Create a Wallpapers directory if it doesn't exist already.
```sh
mkdir Wallpapers
```

Clone this repo into "Wallpapers" (/home/user/Pictures/Wallpapers).
```sh
cd Wallpapers
git clone https://github.com/jarednthomas/mac-mojave-dynamic
```

Fix paths to images in xml file by replacing my user path (/home/jared/) with your username.
```sh
cd mac-mojave-dynamic
sed -i 's/jared/'$(whoami)'/g' mojave_dynamic.xml
```

Set background to xml file.

GDM Steps: Tweaks > Appearance > Background > Select XML File
