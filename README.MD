# Bevy Hello
Simple program with all the setup needed to print `Hello World!`.

## Run
`cargo run --features bevy/dynamic`

`cargo watch -cx run --features bevy/dynamic`

## Build 
`cargo build --release`

## WebAssembly
You can run it in wasm using a code server following [this guide](https://bevy-cheatbook.github.io/platforms/wasm.html)

#### Run
`cargo run --target wasm32-unknown-unknown`


#### Build
`cargo build --release --target wasm32-unknown-unknown` and then

`wasm-bindgen --out-dir ./out/ --target web ./target/`