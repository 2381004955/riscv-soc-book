# �ڰ��� PULPino

## 1. PULP����
PULP��Parallel Ultra-Low Power����Ŀ����ʿ��������������ѧ��ETH Z��rich�����ۺ�ϵͳʵ���ң�IIS��Integrated Systems laboratory����������������Ǵ�ѧ��University of Bologna���ĸ���ЧǶ��ʽ�о��飨EEES��Energy-efficient Embedded Systems����������з���Ŀ����ʵ��һ�����š�����չ��SoC���������幦����mW������Ч�ﵽpJ/op[1]��</br>
</br>
����Ŀ����ʵ������������IoT��Internet of Thing���豸�Լ������������󣬵�ǰ��IoT�豸���������վ��������еĹ���ҲԽ��Խ�࣬���Ի�ȡ�ܱߵ�ͼ�񡢻��������ȴ������ݣ�����������ʶ���Ӧ�ã���������Ҫ�����ļ�����������ǰ��IoT�豸�޷����������ֻ�ܽ�����ͨ�����ߵ�ģʽ���͵�����ƽ̨���м��м��㣬����ͨ������Ҫ���Ĵ��������������ڿ���ع����IoT�豸���ԣ����������ɽ�������ʹ��������Ϊ�˽���������⣬�������ض�Ӧ�ü�������Ӧ����IoT�豸����Ϊ��չ���Ƚ����˹��ģ���ʵ���˸ߵļ����������������ַ�ʽ��ȱ�����ȱ������ԣ��ض�Ӧ�ü�������ĳһ���ض������ASIC���������ޣ�PULP�ֲ��������蹵����ͨ���ܹ����Ż���ƣ�ʵ���˼�ӵ��ǿ��ļ���������������IoT�豸�͹�������ͬʱ������ͨ�ô�����������ԡ���ܹ������ͼ8-1��ʾ��</br>
</br>
![](assets/PULP_Arch.png)</br>
ͼ8-1 PULP�ܹ����[2]</br></br>
��ͼ8-1���Ұ�߿��Է���PULP��һ�����SoC���䴦������Ŀǰ�����֣�һ���ǲ���OpenRISCָ���OR10N����һ���ǲ���RISC-Vָ���RI5CY�����˶����ƣ�Ϊ��ʵ�ֵ͹��ġ������ܵ�Ŀ�ģ�PULP������������һЩ�Ż���ƣ�</br>
(1)ָ���չ��PULP��չ��ԭ�е�ָ���ʹ����֧���������ԣ���ϸ���ݻ��ڱ��º����������ν��ܣ���</br>
* ����ָ����չ��ALU Extension��
* Ӳ��ѭ����Hardware Loop��
* ��ַ�����ķô�ָ�post-incrementing Load & Strore Instruciton��
* ���ۼ�ָ�Multiply-Accumulate��
* ����������Vectorial��
</br>
</br>
(2)����ָ��棺����������˹���һ��L1ָ��棬������Ϊ��ά������һ���Դ����ĸ����ԣ����Ҳ��õ���SCM��Standard Cell based Memories���������ڸ��͵ĵ�ѹ�¹������Ӷ���һ�������˹��ġ�</br>
</br>
(3)ָ��ԤȡBuffer�������ָ�����ܻ����ڶ����������ͬʱ���ʣ��������ӳ٣�Ϊ�ˣ�Ϊÿ�������������һ��ָ��ԤȡBuffer����Buffer�Ĵ�Сһ����ָ���line�Ĵ�С������128bit��ͬʱ������RISC-Vָ����ԣ���ָ��ԤȡBuffer��ʵ����16bitѹ��ָ����չΪ32bit��</br></br>
(4)��������ݻ��棺ʹ�õ���Scratchpad Memroy����Ϊ���bank��һ��Ϊ8KB��ÿ��bank����Ӧһ��SCM��һ��Ϊ1KB��</br></br>
���������Ż������Դ�������Ч����28nm�����£�������ѹ���Ե���0.46V������1mW����ʱ��Ȼ�бȽϺõ����ܱ��֣���Ƶ40MHz��0.2GOPS[3]��</br></br>
PULP���з������У��Ѷ����Ƭ�����8-1��ʾ��</br></br>
��8-1 PULP��Ƭ���<br>
<table>
<tr>
	<td>����</td>
	<td>����</td>
	<td>����</td>
	<td>��Ƶ</td>
	<td>ʱ��</td>
	<td>��ע</td>	
</tr>
<tr>
	<td>Manny</td>
	<td>180nm</td>
	<td>3 W @0.6V 1.5MHz</td>
	<td>1.25 MHz</td>
	<td>2015��</td>
	<td>�ĺ�, 64 kB��������16KB��������ݻ��棬4KBָ���</td>	
</tr>
<tr>
	<td>Diego</td>
	<td>180nm</td>
	<td>3 W @0.8V 15 MHz</td>
	<td>15 MHz</td>
	<td>2015��</td>
	<td>ͬ��</td>	
</tr>
<tr>
	<td>Sid</td>
	<td>180nm</td>
	<td>3 W @1.0V 15 MHz</td>
	<td>15 MHz</td>
	<td>2015��</td>
	<td>ͬ��</td>	
</tr>
<tr>
	<td>Vivosoc</td>
	<td>130nm</td>
	<td>45 mW @1.2V 40MHz</td>
	<td>140 MHz</td>
	<td>2015��</td>
	<td>��������ҽѧ�źŲɼ����ɴ����豸�ϣ�˫��</td>	
</tr>
<tr>
	<td>Vivosoc2</td>
	<td>130nm</td>
	<td>20 mW @1.2V 50MHz</td>
	<td>64 MHz</td>
	<td>2016��</td>
	<td>ͬ�ϣ��������ĺ�</td>	
</tr>
<tr>
	<td>Vivosoc2.001</td>
	<td>130nm</td>
	<td>20 mW @1.2V 50MHz</td>
	<td>64 MHz</td>
	<td>2016��</td>
	<td>ͬ�ϣ��������ĺ�</td>	
</tr>
<tr>
	<td>Mia_Wallace</td>
	<td>65nm</td>
	<td>1 mW @1.2V 1MHz</td>
	<td>400 MHz</td>
	<td>2015��</td>
	<td>�ĺˣ�������һ������������</td>	
</tr>
<tr>
	<td>Fulmine</td>
	<td>65nm</td>
	<td>13 mW @ 0.8 V, 104 MHz</td>
	<td>400 MHz</td>
	<td>2015��</td>
	<td>Mia_Wallace�ĸĽ��ͣ�������һ�����������</td>	
</tr>
<tr>
	<td>Artemis</td>
	<td>65nm</td>
	<td>1 mW @1.2V 1MHz</td>
	<td>500 MHz</td>
	<td>2014��</td>
	<td>�ĺˣ�ÿ����������������һ��FPU</td>	
</tr>
<tr>
	<td>Hecate</td>
	<td>65nm</td>
	<td>1 mW @1.2V 1MHz</td>
	<td>500 MHz</td>
	<td>2014��</td>
	<td>�ĺˣ���������FPU</td>	
</tr>
<tr>
	<td>Diana</td>
	<td>65nm</td>
	<td>1 mW @1.2V 1MHz</td>
	<td>500 MHz</td>
	<td>2014��</td>
	<td>�ĺˣ�1����׼FPU��3���ü���FPU</td>	
</tr>
<tr>
	<td>Phoebe</td>
	<td>65nm</td>
	<td>22 mW @1.2V 100MHz</td>
	<td>500 MHz</td>
	<td>2015��</td>
	<td>Selene�ĸĽ���</td>	
</tr>
<tr>
	<td>Pulp</td>
	<td>28nm</td>
	<td>8 mW @0.7V 10MHz</td>
	<td>475 MHz</td>
	<td>2013��</td>
	<td>�ĺ�</td>	
</tr>
<tr>
	<td>Pulpv2</td>
	<td>28nm</td>
	<td></td>
	<td>1000 MHz</td>
	<td>2014��</td>
	<td>�ĺ�</td>	
</tr>
<tr>
	<td>Pulpv3</td>
	<td>28nm</td>
	<td>1.2 mW @ 0.6V, 50MHz</td>
	<td>66 MHz</td>
	<td>2015��</td>
	<td>ͬ�ϣ�������һ��������������</td>	
</tr>
<tr>
	<td>Honey_Bunny</td>
	<td>28nm</td>
	<td>1 mW @1.2V 1MHz</td>
	<td>60 MHz</td>
	<td>2015��</td>
	<td>��һ��ʹ��RI5CY��Ϊ�������˵�PULP</td>	
</tr>
</table>




## 2. PULPino����
����PULP��PULPino�Ĺ�ϵ��PULPino�Ľṹ��ɡ�RI5CY����Ƭ������
PULP�͹��ĵ�ԭ�򣬹��ĶԱȣ����������жԱȣ����Լ����Թ����ڶ��ֵ�ѹ�����

## 3. ��������ָ��
����ʲô���������㡢RI5CY����������ָ������ص㡢ʵ�ֵ�

## 4. Ӳ��ѭ��
����Ӳ��ѭ����ԭ�����ơ�ʵ�ֵ�

## 5. post increment load/storeָ��
��֪��׼ȷ�ķ�����ʲô

## 6. ��չ����ָ��


## 7. ����Artyƽ̨����ֲ���飨leishangwen��
������ֻ����zedboard�����˲��ԣ���������ҪARM��ϣ�����ƻ�ʹ��Artyƽ̨���ԣ���Freedom E310�Ĳ���ƽ̨��ͬһ������ֲ�󣬿��Զ������У�����ҪARM��ϡ�ͬʱ������ֲ�����У���˳�㽲��ؼ��ű���boot code�����Գ���ȡ����⣬�����ܵ��Թ��̣����Ҳ�ǹ���û�еġ�

## �ο�����
[1]PULP - An Open Parallel Ultra-Low-Power Processing-Platform, http://iis-projects.ee.ethz.ch/index.php/PULP,2017-8</br>
[2]Florian Zaruba, Updates on PULPino, The 5th RISC-V Workshop, 2016.</br>
[3]Michael Gautschi,etc,Near-Threshold RISC-V Core With DSP Extensions for Scalable IoT Endpoint Devices, IEEE Transactions on Very Large Scale Integration Systems</br>