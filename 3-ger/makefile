# CUDA build
CUDADIR ?= /usr/local/cuda

# This machine reports compute capability 5.0.
# Override for another GPU with: make sm=XX
sm=50
GENCODE_SM   = -gencode arch=compute_$(sm),code=sm_$(sm)
GENCODE_COMP = -gencode arch=compute_$(sm),code=compute_$(sm)

LIB=-L${CUDADIR}/lib64 -lcublas

all:
	nvcc ${GENCODE_SM} ${GENCODE_COMP} ger.cu -o ger ${LIB}

clean:
	rm -rf ger

