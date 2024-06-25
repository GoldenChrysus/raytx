# Raytx

Raytx is a command-line tool written in Rust for performing token swap operations on Raydium.

## Project Dependencies

Before getting started, ensure that the following software is installed on your system:

- [Node.js](https://nodejs.org/)
- [Rust](https://www.rust-lang.org/)


## Build
```
cargo build -r
```
This will generate an executable file raytx, located in the target/release/ directory.

## Using the Command-Line Tool
*Quote mint only supports wsol*
### Buy
```
./target/release/raytx swap <mint> buy --in-amount=<in-amount>
```
### Sell
```
# sell 50%
./target/release/raytx swap <mint> sell --in-amount-pct=0.5

# sell all, close wallet ata when sell all
./target/release/raytx swap <mint> sell --in-amount-pct=1

# Sell 1000
./target/release/raytx swap <mint> sell --in-amount=1000
```
Replace <mint> with the address of the token you want to swap, and <in-amount> with the quantity|<in-amount-pct> with the percentage you want to swap.

# Contributing
Contributions to this project are welcome. If you have any questions or suggestions, feel free to raise an issue.

# License
This project is licensed under the MIT License.
