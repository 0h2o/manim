## Background
Stupid 0h2o worked for days, finally he found a simple way to support Chinese characters in both **TextMobject** and **TexMobject** string.
## Install guide
1.Prepare a PC/VM running on a linux system(my case Xubuntu).

2.Install the following packages:
```
sudo apt-get install ffmpeg
#sudo apt-get install latex #(no longer needed)
sudo apt-get install sox
```
Uninstall this in advance:
```
pip uninstall aggdraw
```

3.Install textlive **FULL** package (about 2GB):
```
sudo apt-get -y install texlive-full 
```
You can also skip this procedure, but later on you will come across numerous mistakes caused by lacking dependencies, you will have to find the exact packages needed for your project and install them one by one :(

4.Clone this repository, cd ./ and install python dependencies:
```
pip install -r requirements.txt
```

If you meet the `command 'x86_64-linux-gnu-gcc' failed with exit status 1` error, just do the following thing:

```
sudo apt-get install build-essential libssl-dev libffi-dev python-dev
```

5.Run the manim engine and enjoy!
```
python extract_scene.py example_scenes.py CNSS_TEST -pl
```

**For further details, please refer to the original repo from [3b1b](https://github.com/3b1b/manim).**
