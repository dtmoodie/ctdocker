all:
	(cp ../ct -r build/)
	(cd base; docker build -t ct:18.04 .)
	(cd build; docker build . --no-cache)
