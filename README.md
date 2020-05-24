# Tekken Moveset Extractor By [kiloutre](https://twitter.com/kiloutre) 

This tools main purpose is to port over movelists and mechanics from Tekken Tag 2 into Tekken 7.

It also allows you to change the move set of characters already in Tekken 7 to other characters in the 7 roster.

## Getting Started

This is quite an involved process in this early stage but we are working towards making it more accessable for players in the future.


### Prerequisites

There will be a few programs you will have to aqcuired before being able to use the tool with Tekken 7.

* [TekkenMovesetExtractor](https://github.com/Kiloutre/TekkenMovesetExtractor/releases/) - The tool that does all the magic.
* [Cemu](https://cemu.info/) - A emulator used to run the Wii U port of Tekkken Tag 2.
* [Python 3.6.5](https://www.python.org/downloads/release/python-365/) - Packages from Python are needed for this tool to run.
* [PYWIN32 using PIP](http://www.qarevolution.com/5-step-install-pywin32-using-pip/) - Much needed Python extensions.
* [Cheat Engine](https://www.cheatengine.org/) - Used to look into the opcodes in Cemu.
* Wii U Games Files For Tekken Tag 2 - You will have to aquire this yourself

### Installing & Walkthrough

### Python 3.6.5

1. Download version 3.6.5 of Python from the link provided. Making sure to pick the "Windows x86-64 executable installer" under files, if you're running windows that is.

2. Make sure during installation you've checked the "Add Python 3.6 to PATH" option

3. Go Through the normal steps of the installion and take note of where you've installed it as that will come in handy in the future.

4. Once setup has completed hit close.

### PYWIN32 using PIP

1. Make sure this is done after installing Python 3.6.5

2. Follow the instructions on the link provided in Prerequisites

3. If you get a warning saying " WARNING: You are using pip version 19.2.3, however version 20.1.1 is available. You should consider upgrading via the 'python -m pip install --upgrade pip' command." Ignore it as the version provided is fine

### Cemu:

1. To install Cemu head to their main website located [here](https://cemu.info/) and download the latest verison.

2. The only setting you will need to change in Cemu are the input ones as you will have to navigate the menus.

3. Wii U game files will come pacakged as such:

![alt text](https://i.imgur.com/4D9BFBQ.png)

4. Click File -> Load and navigate to the code folder shown in the image above.

5. This folder contains the file we will use to run Tag 2: **Tekken.rpx**

6. Tag 2 should now launch and if you've set your input settings up correctly you should be able to navigate the menus.

7. Select offline mode and then practice.

Note: Picking solo or tag here does not matter as you can select in the Extractor which player you want to export.

8. For this im picking solo and now you can pick the character you wish to transfer over to Tekken 7

Note: Your opponet does not matter

9. Now pick any stage and sit idle in it as we continue installing the rest of the needed programs.

Note: Take note of what version of Tekken Tag 2 you have as there will be 2: US & EU. The US version requires an extra step I will detail later.

### TekkenMovesetExtractor:

1. Go to the link provided in prerequisites and download **TekkenMovesetExtractor.zip** from the latest release.

2. You can place this anywhere. It does not need to be in the same directory as Tekken.

3. Do not run this as we have to configure our most important program first.

### Cheat Engine: 

This part will be the most complex part of this guide so read carefully

1. Make sure you downloaded the latest version of Cheat Engine from the link provided

2. The install is quite straight forward, at the end launch Cheat Engine (you can try out the tutorial if you want)

3. We are going to use Cheat Engine to find our Cemu_Base code

4. In Cheat Engine there will be a icon that is glowing different colours, you will want to clik that button and select Cemu from the list provided.

5. Now that the Cemu process has been selected right click on the box right of where it says Value Type and select the top option which should say "Define new custom type (Auto Assembler)"

6. A box will appear with some code in it, delete all the code in this box and replace it with the code provided in this [Paste Bin](https://pastebin.com/U3xSNvVE) and hit OK.

Note: Now the Value Type box should state "4 Byte Big Endian" 

7. In the blank Value box put in the value "32770" and while doing your first scan (hit New Scan) make sure in Cemu you are crouching in the game during the whole scan process.

8. Once the scan has completed, you can let your chosen character rise. Now in the left address list you will notice that one of the addresses has the value of "32769" this is the address we need to double click.

9. Now that you've doubled clicked the address








## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc
