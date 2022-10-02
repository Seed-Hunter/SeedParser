Python 3.x program performs a recursive search for secret phrases from crypto wallets inside files, checks their validity (i.e. prints only those phrases that comply with the bip39 standard) and displays the passphrase and the path to the file in which it was found. Validation of phrases for compliance with the bip39 standard is performed using the library from the repository of the trezor hardware crypto wallet https://github.com/trezor/python-mnemonic

Sample program output: /home/zzzzz/zzzzzz/Files/wallety/New text document.txt rude cool annual mango hazard stable affair payment kingdom naive crush cancel

/home/zzzzz/zzzzzz/Files/wallety/tron.txt awake window awful off hero coach salmon deer medal bleak crisp noodle

/home/zzzzzzz/FileGrabber/Users/aliraza/Documents/atomic backup pharse wallet.txt focus city expand planet upon power stick begin usual cereal spring damage

/home/zzzzzzz/FileGrabber/Users/tunas/Desktop/torrrez codes.txt sketch swift bronze stadium monster agent office error lock spare split frown

/home/zzzzz/zzzzzz/Files/wallety/ark wallet.txt rude cool annual mango hazard stable affair payment kingdom naive crush cancel

Installation start

1.It is necessary to download and install python from the site https://www.python.org/ of the version not lower than 3.8 2.At the beginning of the Python installation, select the checkboxes "Install Launcher for all users" and "Add Python3.8 to patch" 3.At the end of the installation select "Disable Patch length limit" 4.Install build tools https://visualstudio.microsoft.com/visual-cpp-build-tools/ https://prnt.sc/XUQAJLvWtrU- 5. After completing the above points, you need to run the installation of the python libraries "install_libs"

Let's start setting up the script seed_parser_v*.py. All settings are here.

SOURCE_DIR = 'd:/__dd2/' The path to the logs is indicated here. If you use this program on Windows, you need to use such slashes /

PARCE_ETH=False - enables or disables (if set to False) parsing of ether private keys. If you are going to enable this, set up exclusion files and folders, because there will be a lot of garbage to collect

BAD_DIRS=[ 'ololololz' ] Bad folders (if you often come across a folder with some kind of garbage, then it can be blacklisted and apache with that name will not be scanned).

BAD_FILES=[ 'ololololo' ] Bad files (if you often come across files with some kind of garbage, then they can be blacklisted and files with that name will not be scanned)

WORDS_CHAIN_SIZES = {12, 15, 18, 24} Here you can specify the length of the phrases to be searched. I advise you to leave all supported

EXWORDS=2 The filter is necessary so that only unique phrases are displayed (all phrases where more than 2 words are repeated will be skipped, such phrases do not exist, I advise you not to change)

Once configured, you can start running. Run.bat will make things easier. In the line cd C:\Users\khuram\Desktop[By SeedHunter]seed_parser paste the link to the folder with the script. by clicking on run.bat run the script