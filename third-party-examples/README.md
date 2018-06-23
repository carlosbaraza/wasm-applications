Compile
```
docker run --rm -v $(pwd):/src trzeci/emscripten emcc -o change.js change.c -lm -O3 -s WASM=1 -s EXPORTED_FUNCTIONS="['_change']" -s BINARYEN_IMPRECISE=1

emcc -o change.js change.c -lm -O3 -s WASM=1 -s EXPORTED_FUNCTIONS="['_change']" -s BINARYEN_IMPRECISE=1
```