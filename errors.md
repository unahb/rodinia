## Gaussian
Error when running the following commands.
`clang++ gaussian.cu -o gaussian --cuda-path=/usr/local/cuda-10.1 --cuda-gpu-arch=sm_35 -L/usr/local/cuda-10.1/lib64 -lcudart_static -ldl -lrt -pthread -save-temps -v`

`/data/bgarg6/spirv_on_x86/build/Demo gaussian-cuda-nvptx64-nvidia-cuda-sm_35.bc kernel.bc 1 1 1 512 1 1`

Error: Demo: /home/robinhan/llvm10.x/llvm/lib/Analysis/BasicAliasAnalysis.cpp:844: llvm::AliasResult llvm::BasicAAResult::alias(const llvm::MemoryLocation&, const llvm::MemoryLocation&, llvm::AAQueryInfo&): Assertion `notDifferentParent(LocA.Ptr, LocB.Ptr) && "BasicAliasAnalysis doesn't support interprocedural queries."' failed.
Aborted (core dumped)

## Pathfinder
LLVM ERROR: Cannot select: intrinsic %llvm.nvvm.read.ptx.sreg.ctaid.x