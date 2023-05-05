# Lab 1 - GHDL and GTKWave
- Go to the GitHub repository of Digital System Design (DSD)
- Study VHDL and GHDL
- Go to the GHDL folder
- Install GHDL and GTKWave
- Run the Half Adder example
- Run another example such as D Flip-Flop or 4-to-1 Multiplexer
- Document the results on your GitHub repository
- Exploration: Icarus Verilog



## Examples:
### Hello World!
```
$ ghdl -h
$ ghdl -v
$ ghdl -a hello.vhdl
$ ghdl -e hello_world
$ ghdl -r hello_world
Hello world!
```

![](https://github.com/tnuevaes/CPE322_S23/blob/2ee2d0e682a200dc44ca6cca4abfaa70a3c0294f/lab%201/Hello_world.png)

### Half Adder

```
$ ghdl -a ha.vhdl
$ ghdl -a ha_tb.vhdl
$ ghdl -e ha_tb
$ ghdl -r ha_tb --vcd=ha.vcd
ha_tb.vhdl:47:5:@5ns:(assertion error): Reached end of test
$ gtkwave ha.vcd
```
![](https://github.com/tnuevaes/CPE322_S23/blob/2ee2d0e682a200dc44ca6cca4abfaa70a3c0294f/lab%201/half_adder.png)

### Full Adder
```
$ ghdl -a adder.vhdl
$ ghdl -a adder_tb.vhdl
$ ghdl -e adder_tb
$ ghdl -r adder_tb --vcd=adder.vcd
adder_tb.vhdl:54:5:@8ns(assertion note): end of test
$ gtkwave adder.vcd
```
![](https://github.com/tnuevaes/CPE322_S23/blob/2ee2d0e682a200dc44ca6cca4abfaa70a3c0294f/lab%201/full_adder.png)



### D Flip Flop

```
$ ghdl -a dff.vhdl
$ ghdl -a dff_tb.vhdl
$ ghdl -e dff_tb
$ ghdl -r dff_tb --vcd=dff.vcd
$ gtkwave dff.vcd
```
![](https://github.com/tnuevaes/CPE322_S23/blob/2ee2d0e682a200dc44ca6cca4abfaa70a3c0294f/lab%201/dff.png)

