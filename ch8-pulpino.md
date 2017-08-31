# �ڰ��� PULPino

## 8.1 PULP����
### 8.1.1 ��Ŀ����
PULP��Parallel Ultra-Low Power����Ŀ����ʿ��������������ѧ��ETH Z��rich�����ۺ�ϵͳʵ���ң�IIS��Integrated Systems laboratory����������������Ǵ�ѧ��University of Bologna���ĸ���ЧǶ��ʽ�о��飨EEES��Energy-efficient Embedded Systems����������з���Ŀ����ʵ��һ�����š�����չ��SoC���������幦����mW������Ч�ﵽpJ/op[1]��</br>
</br>
����Ŀ����ʵ������������IoT��Internet of Thing���豸�Լ������������󣬵�ǰ��IoT�豸���������վ��������еĹ���ҲԽ��Խ�࣬���Ի�ȡ�ܱߵ�ͼ�񡢻��������ȴ������ݣ�����������ʶ���Ӧ�ã���������Ҫ�����ļ�����������ǰ��IoT�豸�޷����������ֻ�ܽ�����ͨ�����ߵ�ģʽ���͵�����ƽ̨���м��м��㣬����ͨ������Ҫ���Ĵ��������������ڿ���ع����IoT�豸���ԣ����������ɽ�������ʹ��������Ϊ�˽���������⣬�������ض�Ӧ�ü�������Ӧ����IoT�豸����Ϊ��չ���Ƚ����˹��ģ���ʵ���˸ߵļ����������������ַ�ʽ��ȱ�����ȱ������ԣ��ض�Ӧ�ü�������ĳһ���ض������ASIC���������ޣ�PULP�ֲ��������蹵����ͨ���ܹ����Ż���ƣ�ʵ���˼�ӵ��ǿ��ļ���������������IoT�豸�͹�������ͬʱ������ͨ�ô�����������ԡ�
### 8.1.2 �ܹ�����
��ܹ������ͼ8-1��ʾ��</br>
</br>
![](assets/PULP_Arch.png)</br>
ͼ8-1 PULP�ܹ����[2]</br></br>
��ͼ8-1���Ұ�߿��Է���PULP��һ�����SoC���䴦������Ŀǰ�����֣�һ���ǲ���OpenRISCָ���OR10N����һ���ǲ���RISC-Vָ���RI5CY�����˶����ƣ�Ϊ��ʵ�ֵ͹��ġ������ܵ�Ŀ�ģ�PULP������������һЩ�Ż���ƣ�</br></br>
��1��ָ���չ��PULP��չ��ԭ�е�ָ���ʹ����֧���������ԣ���ϸ���ݻ��ڱ��º����������ν��ܣ���</br>
* ����ָ����չ��ALU Extension��
* Ӳ��ѭ����Hardware Loop��
* ��ַ�����ķô�ָ�post-incrementing Load & Strore Instruciton��
* ���ۼ�ָ�Multiply-Accumulate��
* ����������Vectorial��
��2������ָ��棺����������˹���һ��L1ָ��棬������Ϊ��ά������һ���Դ����ĸ����ԣ����Ҳ��õ���SCM��Standard Cell based Memories���������ڸ��͵ĵ�ѹ�¹������Ӷ���һ�������˹��ġ�</br>
</br>
��3��ָ��ԤȡBuffer�������ָ�����ܻ����ڶ����������ͬʱ���ʣ��������ӳ٣�Ϊ�ˣ�Ϊÿ�������������һ��ָ��ԤȡBuffer����Buffer�Ĵ�Сһ����ָ���line�Ĵ�С������128bit��ͬʱ������RISC-Vָ����ԣ���ָ��ԤȡBuffer��ʵ����16bitѹ��ָ����չΪ32bit��</br></br>
��4����������ݻ��棺ʹ�õ���Scratchpad Memroy����Ϊ���bank��һ��Ϊ8KB��ÿ��bank����Ӧһ��SCM��һ��Ϊ1KB��</br></br>
���������Ż������Դ�������Ч����28nm�����£�������ѹ���Ե���0.46V������1mW����ʱ��Ȼ�бȽϺõ����ܱ��֣���Ƶ40MHz��0.2GOPS[3]��
### 8.1.3 ��Ƭ���
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




## 8.2 PULPino����
### 8.2.1 PULPino��PULP�Ĺ�ϵ
PULPino��PULP�ļ򻯰汾����ͼ8-2��ʾ��</br>
![](assets/PULPino_Arch1.png)</br>
ͼ8-2 PULPino�ܹ���PULP�ܹ��ļ򻯰�[2]</br></br>
�Ա�ͼ8-1PULP�ܹ���ƿ�֪PULPino���PULP�����¼����������˼򻯣�</br>
��1����˱�Ϊ���ˣ�</br>
��2��ָ��RAM������RAM��������Ҫ֧�ֶ�ˣ�</br>
��3��ȥ���˶������棻</br>
��4��ȥ����DMA��</br>
���⻹��һ���仯��Դ������2016��3��1�տ�Դ������ Solderpad license��ʹ�õı��������System Verilog��PULPino֧�ִ��������ǲ���OpenRISCָ���OR10N��������Ŀǰ�Ŀ�Դ�汾��ֻ֧��RISC-Vָ���</br>

### 8.2.2 PULPino�Ľṹ
���ͼ8-2���ԣ�ͼ8-3���Ӿ��塢��������ʾ��PULPino�Ľṹ��</br>
![](assets/PULPino_Arch2.png)</br>
ͼ8-3 PULPino�Ľṹ[4]</br></br>
��ͼ�п��Է���PULPino������һЩ�ص㣺</br>
��1�����õ���ָ��RAM������RAM�ֿ��Ĺ���ṹ��</br>
��2��������һ��Boot ROM�����п��Դ洢�������룬���ø�����������Լ���������SPI�ӿڵ�Flash�еĳ���</br>
��3�����õ�AXI4��APB�������߽ṹ��</br>
��4����������ӿڣ�����GPIO��UART��I2C��SPI�ȡ�</br>
��5������һ��SoC Controllģ�飬������������SoCƽ̨�Ŀ�����Ϣ���������Ƿ�ʹ��ʱ���š�����������ַ���ܹ���Ϣ�ȡ�</br>
��6���ṩ��һ��Advanced Debug Unit���ṩ�˱�׼����JTAG�ӿڣ�ʹ�õ��������Է���ָ��RAM������RAM���������ڲ��Ĵ������Լ������Ӧ�Ŀ��ƼĴ����ȡ�</br>
��7���ṩ��һ��SPI Slave�ӿڣ�ֱ��������AXI���������ϣ�����ͨ���ýӿ��ڲ�Ӱ�촦����������£�����ָ��RAM������RAM���������ڲ��Ĵ������Լ������Ӧ�Ŀ��ƼĴ����ȡ�</br>
ͼ8-2�и�ģ�����ϸ���ܡ��Ĵ������ÿ��Բο�����[4]��</br>

### 8.2.3 ��������
PULPinoĿǰ֧��4�ֲ�ͬ���õġ�����RISC-Vָ��Ĵ������ˣ����£�</br>
��1��RI5CY���������翪Դ�Ĵ������ˣ�֧��RV32-ICM������֧������ָ����չ��ALU Extension����Ӳ��ѭ����Hardware Loop������ַ�����ķô�ָ�post-incrementing Load & Strore Instruciton�������ۼ�ָ�Multiply-Accumulate��������������Vectorial������չ��</br>
��2��RI5CY+FPU������RI5CY���Լ�һ������IEEE-754��׼�ĵ�����FPU��</br>
��3��Zero-riscy��֧��RV32-ICM����ռ����Դ�������Ż���</br>
��4��Micro-riscy: ����4��������ռ����Դ���ٵģ�֧��RV32-EC������16���Ĵ������Ҳ�֧��Ӳ���˷���</br>
��ͬ���õ���Դռ�������ͼ8-4��ʾ��Micro-riscy����Դռ����RI5CY�Ľӽ�1/4��</br></br>
![](assets/resources.png)</br>
ͼ8-4 ��ͬ���õ���Դռ�����[5]</br></br>
ͼ8-5�ǲ�ͬ�����ڲ�ͬӦ�û����е��ܺ��������ͼ�п��Է��֣���ͬ�������ʺ��ڲ�ͬ��Ӧ�ó�����������������źŴ��������бȽ϶�ľ�����㣬��ôRI5CY���ܺ�����͵ģ���Ϊ������ָ����չ���ڲ���ר��Ӳ������ʵ�־�����㡣������ڿ���������ôMicro-riscy���ܺ���͡����ԣ��û���Ҫ���ݲ�ͬ��Ӧ�ó���������PULPino��</br></br>
![](assets/power.png)</br>
ͼ8-5 ��ͬ�����ڲ�ͬӦ�û����е��ܺ����[5]</br>

### 8.2.4 �ӿ�����
�����߿�����https://github.com/pulp-platform/pulpino ���صõ�PULPino��Դ���룬����rtlĿ¼�µ�pulpino_top.sv��PULPino�Ķ����ļ���ͨ�����ļ����Եõ�PULPino�Ľӿ�ʾ��ͼ��ͼ8-6��ʾ�����ڴ�����ӿڶ�����ͨ���ӿ���������_i����_o���ֳ�������ӿڻ�������ӿڡ�</br></br>
![](assets/PULPino_Interface.png)</br>
ͼ8-6 PULPino�ӿ�ʾ��ͼ</br></br>
���չ��ܿ��Է�Ϊ���ࣺȫ���źŽӿڡ�SPI Slave��SPI Master��I2C��UART��GPIO��JTAG��pad config�ȣ���ͼ8-3����һ�¡�����ȫ�ֽӿڵ��������8-2��ʾ��</br></br>
��8-2 PULPino��ȫ�ֽӿ�</br>
<table>
<tr>
	<td>�ź���</td>
	<td>����</td>
</tr>
<tr>
	<td>clk</td>
	<td>ʱ���ź�</td>
</tr>
<tr>
	<td>rst_n</td>
	<td>��λ�ź�</td>
</tr>
<tr>
	<td>clk_sel_i</td>
	<td>����ѡ����ʱ�ӣ������0����ôʱ�Ӿ���clk����֮��ʱ������һ����Ƶ��������ASIC����ʱ��clk_sel_i����Ϊ1</td>
</tr>
<tr>
	<td>clk_standalone_i</td>
	<td>����Ƶ����صĿ����ź�</td>
</tr>
<tr>
	<td>testmode_i</td>
	<td>���Ϊ1����ô��ֹclock gate����֮��ʹ��clock gate</td>
</tr>
<tr>
	<td>fetch_enable_i</td>
	<td>���Ϊ1����ʾ��ʼȡָ����ִ��</td>
</tr>
<tr>
	<td>scan_enable_i</td>
	<td>����Ƶ����صĿ����ź�</td>
</tr>
</table>

### 8.2.5 ��ַ�ռ����
PULPinoĬ�ϵ�ָ��RAM������RAM�Ĵ�С����32KB����rtlĿ¼�µ�core_region.sv���ʼ�����¶��壬�������������޸�ָ��RAM������RAM�Ĵ�С��</br>
~~~module core_region
#(
    parameter AXI_ADDR_WIDTH       = 32,
    parameter AXI_DATA_WIDTH       = 64,
    parameter AXI_ID_MASTER_WIDTH  = 10,
    parameter AXI_ID_SLAVE_WIDTH   = 10,
    parameter AXI_USER_WIDTH       = 0,
    parameter DATA_RAM_SIZE        = 32768, // in bytes
    parameter INSTR_RAM_SIZE       = 32768  // in bytes
  )~~~
</br>  
Ĭ�ϵĵ�ַ�ռ������ͼ8-7��ʾ����ͼ��ο�����[4]��ͼ2.1�в����Ҫ��Boot ROM����ʼ��ַ��ͬ���˴�������ʵ�ʴ���ȷ��Boot ROM��ʼ��ַ��0x0000_8000���ο�����[4]��ͼ2.1��Boot ROM��ʼ��ַ��0x0008_0000��</br>
![](assets/memory_space.png)</br>
ͼ8-7 Ĭ�ϵĵ�ַ�ռ����</br></br>
�����Ͽ��Է�Ϊ�ĸ�����ָ��RAM��Boot ROM������RAM�����衣�����ַ�ռ���䷽������rtlĿ¼�µ�top.sv�ж���ģ����£�����ͨ���޸����еĴ��룬ʵ�ֵ�ַ�ռ���䷽�������¶��塣</br>
`  axi_node_intf_wrap
  #(
    .NB_MASTER      ( 3                    ),
    .NB_SLAVE       ( 3                    ),
    .AXI_ADDR_WIDTH ( `AXI_ADDR_WIDTH      ),
    .AXI_DATA_WIDTH ( `AXI_DATA_WIDTH      ),
    .AXI_ID_WIDTH   ( `AXI_ID_MASTER_WIDTH ),
    .AXI_USER_WIDTH ( `AXI_USER_WIDTH      )
  )
  axi_interconnect_i
  (
    .clk       ( clk_int    ),
    .rst_n     ( rstn_int   ),
    .test_en_i ( testmode_i ),

    .master    ( slaves     ),
    .slave     ( masters    ),

    .start_addr_i ( { 32'h1A10_0000, 32'h0010_0000, 32'h0000_0000 } ),
    .end_addr_i   ( { 32'h1A11_FFFF, 32'h001F_FFFF, 32'h000F_FFFF } )
  );`
 
�������붨����AXI�����������豸�ĵ�ַ�����£�
* �豸1����ʼ��ַ��32'h1A10_0000����ֹ��ַ��32'h1A11_FFFF
* �豸2����ʼ��ַ��32'h0010_0000����ֹ��ַ��32'h001F_FFFF
* �豸3����ʼ��ַ��32'h0000_0000����ֹ��ַ��32'h000F_FFFF
���ͼ8-3��ͼ8-7���Էǳ�ֱ�۵ķ��֣��豸1����ͼ8-7�еĸ�������ĵ�ַ�ռ䣬Ҳ����ͼ8-3�еĹ���APB�����µĸ������裻�豸2����ͼ8-7�е�����RAM���豸3����ͼ8-7��ָ��RAM+Boot ROM��</br>
��rtlĿ¼�µ�instr_ram_wrap.sv������ָ���ַ���ж��Ǵ�Boot ROM���Ǵ�ָ��RAM��ȡָ����£�</br>
`module instr_ram_wrap
  #(
parameter RAM_SIZE   = 32768,                // in bytes
// one bit more than necessary, for the boot rom
    parameter ADDR_WIDTH = $clog2(RAM_SIZE) + 1, 
    parameter DATA_WIDTH = 32
  )(
  ......
// Ϊ1��ʾ��Boot ROM��ȡָ����֮����ָ��RAM��ȡָ
  assign is_boot = (addr_i[ADDR_WIDTH-1] == 1'b1);
......`

��include\apb_bus.sv���ɸ�������ĵ�ַ�ռ䶨�壬���£�
`// MASTER PORT TO CVP
`define UART_START_ADDR       32'h1A10_0000
`define UART_END_ADDR         32'h1A10_0FFF

// MASTER PORT TO GPIO
`define GPIO_START_ADDR       32'h1A10_1000
`define GPIO_END_ADDR         32'h1A10_1FFF

// MASTER PORT TO SPI MASTER
`define SPI_START_ADDR        32'h1A10_2000
`define SPI_END_ADDR          32'h1A10_2FFF

// MASTER PORT TO TIMER
`define TIMER_START_ADDR      32'h1A10_3000
`define TIMER_END_ADDR        32'h1A10_3FFF

// MASTER PORT TO EVENT UNIT
`define EVENT_UNIT_START_ADDR 32'h1A10_4000
`define EVENT_UNIT_END_ADDR   32'h1A10_4FFF

// MASTER PORT TO I2C
`define I2C_START_ADDR        32'h1A10_5000
`define I2C_END_ADDR          32'h1A10_5FFF

// MASTER PORT TO FLL
`define FLL_START_ADDR        32'h1A10_6000
`define FLL_END_ADDR          32'h1A10_6FFF

// MASTER PORT TO SOC CTRL
`define SOC_CTRL_START_ADDR   32'h1A10_7000
`define SOC_CTRL_END_ADDR     32'h1A10_7FFF

// MASTER PORT TO DEBUG
`define DEBUG_START_ADDR      32'h1A11_0000
`define DEBUG_END_ADDR        32'h1A11_7FFF`

### 8.2.6 �жϴ������
PULPino�����ж�������ķ�ʽ�����жϣ�ͼ8-8��Ĭ�ϵ��ж����ͣ������Ӧ���жϴ������̵���ڵ�ַ��ÿ���жϴ�������ռ��4���ֽڣ����Է�ֹһ��32λ��ָ���������16λ��ָ�һ����ת��ָ�ת�Ƶ�������жϴ�������</br>
![](assets/interrupt_vector.png)</br>
ͼ8-8 �ж�������</br>



</br>
�����Ŀ¼Ҫ�޸�

## 8.3 ��������ָ��
����ʲô���������㡢RI5CY����������ָ������ص㡢ʵ�ֵ�

## 8.4 Ӳ��ѭ��
����Ӳ��ѭ����ԭ�����ơ�ʵ�ֵ�

## 8.5 post increment load/storeָ��
��֪��׼ȷ�ķ�����ʲô

## 8.6 ��չ����ָ��


## 8.7 ����Artyƽ̨����ֲ���飨leishangwen��
������ֻ����zedboard�����˲��ԣ���������ҪARM��ϣ�����ƻ�ʹ��Artyƽ̨���ԣ���Freedom E310�Ĳ���ƽ̨��ͬһ������ֲ�󣬿��Զ������У�����ҪARM��ϡ�ͬʱ������ֲ�����У���˳�㽲��ؼ��ű���boot code�����Գ���ȡ����⣬�����ܵ��Թ��̣����Ҳ�ǹ���û�еġ�

## �ο�����
[1]PULP - An Open Parallel Ultra-Low-Power Processing-Platform, http://iis-projects.ee.ethz.ch/index.php/PULP,2017-8</br>
[2]Florian Zaruba, Updates on PULPino, The 5th RISC-V Workshop, 2016.</br>
[3]Michael Gautschi,etc,Near-Threshold RISC-V Core With DSP Extensions for Scalable IoT Endpoint Devices, IEEE Transactions on Very Large Scale Integration Systems</br>
[4]Andreas Traber, Michael Gautschi,PULPino: Datasheet,2016.11</br>
[5]http://www.pulp-platform.org/</br>