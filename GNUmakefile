-:
	git submodule update --init
	python3 -m pip install --user --upgrade pip
	python3 -m pip install --user meson
	brew install llvm
	brew install libarchive && brew link --force libarchive
	@echo 'export PATH="/opt/homebrew/opt/libarchive/bin:$PATH"' >> /Users/git/.bash_profile
	brew reinstall pkg-config
	meson build && pushd build && ninja && popd
	sudo mkdir -p /usr/local/opt/libarchive/include