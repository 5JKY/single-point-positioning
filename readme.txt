Pseudo-Range:
The pseudo-range (PR) is the distance from the receiver antenna to the satellite antenna including receiver and satellite clock offsets (and other biases, such as atmospheric delays): 
PR = distance + c * (receiver clock offset –satellite clock offset + other biases) 
so that the pseudo-range reflects the actual behaviour of the receiver and satellite clocks. The pseudo-range is stored in units of meters.

Pseudorange definition
The pseudorange (code) measurement is defined to be equivalent to the difference of the time of reception (expressed in the time frame of the receiver) and the time of transmission (expressed in the time frame of the satellite) of a distinct satellite signal.

copy1 采用了单历元伪距定位，
copy2 采用了多历元伪距定位。

历元伪距单点定位流程：
1.观测向量L基于伪距消电离层组合值。假设当前历元有n个卫星的观测，则L是n*1的向量, A是n*4的矩阵（待求参数共四个:dx, dy, dz, ddt ）。
2.假设光速为c。当前历元中，第i个卫星的卫星位坐标和钟差是Xs=(xs, ys, zs, dts)。未知数向量是X=(x, y, z, dt)。C1C观测值是P1，信号频率是f1；C2W观测值是P2 ，信号频率是f2。
3.参考相关计算公式，结合最小二乘法计算未知向量定位。
