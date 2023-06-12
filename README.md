# Matrix Addition With Unified Memory
## Aim:
To demonstrate matrix addition using CUDA programming with unified memory.

## Procedure:
Allocate unified memory for matrices A, B, and C.
Initialize matrices A and B with appropriate values.
Define the grid and block dimensions for the CUDA kernel.
Launch the CUDA kernel to perform matrix addition.
Synchronize the device to ensure all CUDA operations are completed.
Print the result matrix C.
Free the allocated device memory.
## Output:
![243189365-01038d16-b6c6-4f07-9a14-458c9d7bebcd](https://github.com/durga46/PCA-Matrix-Addition-With-Unified-Memory/assets/75235704/7a83889d-5606-4179-baa2-3670956f7777)
![243189374-d187a3b8-373f-485b-a52d-c68968cc507e](https://github.com/durga46/PCA-Matrix-Addition-With-Unified-Memory/assets/75235704/2a8ecc8e-3598-4de4-a8c5-fe2f3d33d372)
![243189380-81e4f3bc-a3d7-46e9-a250-d1c1b2917b10](https://github.com/durga46/PCA-Matrix-Addition-With-Unified-Memory/assets/75235704/7db40e12-2b8d-49e8-ade5-97c5046c771a)

## Result:
The memset function calls are not necessary in this program. They were originally used to set the memory blocks for matrices A, B, and C to zero. However, the subsequent initialization loops already assign specific values to each element of the matrices, overwriting the previous values set by memset. Removing the memset calls does not affect the correctness of the program and has no significant impact on its performance. It is good practice to remove unnecessary code to improve code readability and maintainability. The result printed to the console, showing the elasped time in the Host and the GPU to compare their performance.
