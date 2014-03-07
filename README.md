CE3_Bapty
=========
### Moore

![alt tag](https://raw.github.com/seanbapty/CE3_Bapty/master/moore%20testbench%20out.JPG)

The output of the Moore elevator controller was manually checked. By looking at the VHDL generated output it can be seen that when the input "up_down" is set to '1' and the input "stop" is set to '0' the elvator rises from the first to fourth floors. Conversely, the elevator goes from the fourth to first floors when "up_down" is '0' and stop is '0'. Finally, whenever stop is '0' the elevator does not change with the rising clock edge.

### Mealy

![alt tag](https://raw.github.com/seanbapty/CE3_Bapty/master/mealy_upDownWithoutStop.JPG)

The output of the Mealy elevator controller was manually checked. By looking at the VHDL generated output it can be seen that the "floor" output is the same as the Moore elevator contoller. Additionally, the nextfloor output correctly denotes the value of floor whenever it is allowed to proceed. One thing to note is that at the top floor when up_down is set to go up means that both floor and nextfloor should and does output the fourth floor value.

