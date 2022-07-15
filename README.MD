# Bevy Hello
Simple program with all the setup needed to print `Hello World!`.

## Run
`cargo run --features bevy/dynamic`

`cargo watch -cx run --features bevy/dynamic`

## Build 
`cargo build --release`

## WebAssembly
You can run it in wasm using a code server following [this guide](https://bevy-cheatbook.github.io/platforms/wasm.html).

Check out the result here: <https://ad-ops.github.io/bevy-hello/>

#### Run
`cargo run --target wasm32-unknown-unknown`

#### Build
```sh
cargo build --release --target wasm32-unknown-unknown
wasm-bindgen --out-dir ./docs/ --target web ./target/
cp -R assets docs
```

