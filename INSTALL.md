# Linux

	sudo apt-get install make git python

	sudo apt-get install byacc flex pkg-config libpng-dev
	git clone https://github.com/rednex/rgbds
	cd rgbds
	sudo make install
	cd ..

	git clone --recursive https://github.com/RonaldMcFrickinDonald/starterpak
	cd starterpak

To build **pokered.gbc**, **pokegreen.gbc** and **pokeblue.gbc**:

	make

To build them individually:

	make red
	make green
	make blue
	
To build them in pairs:

    make red green
	make red blue
	make green red
	make green blue
	make blue red
	make blue green


# Mac

Get [**Homebrew**](http://brew.sh/).

Then in **Terminal**, run:

	xcode-select --install
	brew install rgbds

	git clone --recursive https://github.com/RonaldMcFrickinDonald/starterpak
	cd starterpak

	make


# Windows

To build on Windows, use [**Cygwin**](http://cygwin.com/install.html) (64-bit). Use the default settings.

In the installer, select the following packages:
- `make`
- `git`
- `python`

Then download [**rgbds**](https://github.com/bentley/rgbds/releases).
Extract the archive. Inside should be `rgbasm.exe`, `rgblink.exe`, `rgbfix.exe`, `rgbgfx.exe` and some `.dll` files. Put each file in `C:\cygwin64\usr\local\bin\`. If your Cygwin installation directory differs, ensure the `bin` directory is present in the PATH variable.

In the **Cygwin terminal**:

	git clone --recursive https://github.com/RonaldMcFrickinDonald/starterpak
	cd starterpak
	
	git submodule init
	git submodule update

	make

To build them individually:

	make red
	make green
	make blue

To build them in pairs:

    make red green
	make red blue
	make green red
	make green blue
	make blue red
	make blue green
