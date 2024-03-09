name: Build C++ Project (Optional Testing Removed)
on:
  push:
    branches: [ main ]
  pull_request:
    branches: [ main ]
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - name: Configure CMake
        run: cmake -B ${{github.workspace}}/build -DCMAKE_BUILD_TYPE=Release
      - name: Build
        run: cmake --build ${{github.workspace}}/build --config Release 
