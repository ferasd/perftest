# perftest

# Build with Cuda enabled by:
./autogen.sh
./configure --prefix=/usr --libdir=/usr/lib64 --sysconfdir=/etc CUDA_H_PATH=/usr/local/cuda/include/cuda.h
make

# Make sure nv_peer_mem module is loaded:
lsmod | grep nv_peer_mem
