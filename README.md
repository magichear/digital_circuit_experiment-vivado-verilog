# digital_circuit_experiment-vivado-verilog

## Some usefull websites

- [Vivado各模块资源占用情况查看方法](https://blog.csdn.net/weixin_45143788/article/details/111328155)
- [VivadoWNS显示负数的解决办法](https://blog.csdn.net/m0_59487432/article/details/131681844.)

在Vivado中查看WNS和资源使用情况的步骤如下：

1. 首先，你需要完成Implementation过程。这个过程包括opt_design、place_design和route_design三个步骤。

2. 完成Implementation后，在Flow Navigator下的IMPLMENTATION中点击Open Implemented Design。

3. 然后选择Report Utilization¹。这个报告会显示你的设计在FPGA上使用了多少资源，包括查看各个模块的资源占用情况。

4. 对于WNS，你可以运行“report_timing”或“report_timing_summary”命令来获取。WNS（Worst Negative Slack）表示所有时序路径上的最差松弛，用于分析最大延迟²。当WNS为负数时，表示有问题；当WNS为正数时，表示没有冲突。


