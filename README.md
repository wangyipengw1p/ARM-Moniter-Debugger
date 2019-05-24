# ARM-moniter
course lab for Embedded System Design 北航嵌入式系统设计ARM大作业
 
 ```Approval version``` 
 
 
 </br>
### To do list
 - [ ]error input in R 
 - [ ]special print byte for m 
 - [√]try print10 using MUL
 
### Notes
- You can find the ```ADS1.2``` [Here](http://pan.baidu.com/s/1gdDxImB) and ```System Image ISO``` [Here](https://msdn.itellyou.cn/)
- The print 10 task is implemented in two methods, while the bulided proj file uses the simpler one. 
- For binary to BCD algorithm and demo, please refer to http://www.johnloomis.org/ece314/notes/devices/binary_to_BCD/bin_to_bcd.html
- Please check the ```out_put_example.txt``` for examples.

### Task instructions
#### Project Files

The code you should import to build your monitor project is as follows:
- monitor.s: A skeleton file for your monitor program.
- main.s: The test harness for your monitor. This file doesn't need to be modified.
- getline.a: A binary of the line parsing routine is included since writing your own routine can be tricky.
However, to get maximum marks for the project, you are expected to write your own replacement for this routine.
- vectors.s: Already seen in the "SWI handler" exercise, this is an example on how to initialise the ARM Vector Table to a default state. Modify it to link your monitor to the appropriate events.

#### Mission

For this part of the project, you must write a simple monitor program. A monitor program is a program usually residing in ROM on a stand-alone microprocessor system which allows other programs to be run and debugged in a way very similar to the ARM Toolkit. You are required to write a set of routines that might form the basis of a very simplified version of such a monitor. It will not be loaded into ROM, but run under the ARM Toolkit emulation.

The main application (file main.s), running in User mode, is interrupted in two different manners. The first one is the execution of an undefined instruction. The second one is a software interrupt (SWI). Both interrupts should lead to a jump to your monitor program in order to debug the interrupted application. This should be done in a similar way as in the "SWI handler" exercise studied previously.

The set of commands that you should implement are shown in the table below. All numeric inputs are in
hexadecimal form, with the possible exception of <number>.

![instruction](https://github.com/wangyipengw1p/ARM-moniter/blob/master/image.png)
-----------------------------
WYP 2019.5.24  ```听说Github也有素质三连？（并不）```
