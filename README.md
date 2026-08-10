# estresso
A simple program to stress test the CPU written in Rust.

Estresso puts some load on your CPU to be able to check stability and temperature of the CPU under stress.

## NOTE

This is a (very) small private project mainly for practice on coding in Rust. The current state is just a starting point so don't be surprised that it's basically nothing at the moment, but I plan to be working on it as soon as I am done working on my bachelor's thesis.

If you have any suggestions for a feature or how to improve the code (although there is not much at the moment lol) please let me know by opening an issue :D

### Currently Planned Features

- [ ] Show live temperature monitoring
- [ ] Take testing time as argument
- [ ] Automatically determine default worker count
- [ ] Show stats like max temperature after running

## Installing
Make sure, you have the [Rust toolchain](https://www.rust-lang.org/learn/get-started) installed.

Clone this repository to your machine and open a command line in the directory of the project.

In the command line, run 
```
cargo build
```

## Running the program

Run the program using the command 
```
cargo run -- --count <COUNT>
```
where \<COUNT\> represents the number of workers to start.

For example, if you want to stress test a CPU with 8 Threads, run
```
cargo run -- --count 8
```