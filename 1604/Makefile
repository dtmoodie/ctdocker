all:
	(cp ../ct -r build/)
	(cd base; sudo docker build -t ct:16.04 .)
	(cd build; sudo docker build . --no-cache)
