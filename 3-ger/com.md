nvidia-smi

3.ger

make sm=52
./ger 33 9 10
./ger


4.gemm
nvcc --version
nvidia-smi
make sm=52

./gemm 1 1       # Single scalar multiplication
./gemm 2 1       # Small matrix
./gemm 17 7      # Irregular size, multiple matrices
./gemm 32 1000   # Maximum matrix size, larger batch