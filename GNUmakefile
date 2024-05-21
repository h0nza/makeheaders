
default : build

cmake = cmake
build = build

build : konf


konf :
	$(cmake) -S . -B $(build) $(CMAKE_ARGS) #--preset $(preset)


build : konf
	$(cmake) --build $(build)
