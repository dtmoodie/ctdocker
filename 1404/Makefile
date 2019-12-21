all:
	(rm -rf build/ct)
	(cp -r ../ct build/)
	(cd base; docker build -t ct:14.04 .)
	(cd build; docker build . --no-cache)
