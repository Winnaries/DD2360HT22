NVCC = nvcc
NVCC_FLAGS = -arch=$(NVCC_ARCH)

ARCH = sm_75
OUTPUT_FILE = heat1D.out
CUDA_LIBDIR = /usr/local/cuda-11.4//targets/x86_64-linux/lib

default: heat1D.cu
	nvcc -o=$(OUTPUT_FILE) -arch=$(ARCH) -L$(CUDA_LIBDIR) -lcusparse -lcublas heat1D.cu
