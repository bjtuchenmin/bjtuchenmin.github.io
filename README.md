# bjtuchenmin.github.io
	通信系统概述
*简述信号、信息与消息的区别和联系
答：消息是信息的物理形式，信息是消息的有效内容，信号是消息的传输载体。如要通过微信发送一条语音消息，则以电信号为载体，消息播放后才得出信息。
*简述一个通信系统应包括的主要部分及各部分功能
答：一个通信系统主要应包括信源、发送设备、信道、接收设备和信宿。信源的作用为将消息转化为电信号，发送设备的作用是产生适合在信道中传输的信号，包括编码、调制等过程，信道的作用是信号传送到接收端，接收设备和信宿的作用分别与发送设备和信源相反。
*简述随参信道的特点及其对信号的影响并举例（3种）（2016年）
答：随参信道中传输信号的衰耗是时变的，时延是时变的，随参信道会造成多径传播。常见的随参信道有短波电离层反射信道、对流层散射信道、移动通信信道。
*简述多径效应的概念、影响以及列举抗多径传播的方法（2014年）
答：多径效应是指电磁波经不同路径传播后，各分量场到达接收端时间不同，按各自相位相互叠加而造成干扰，使得原来的信号失真，或者产生错误的现象。造成的影响有造成信号包络的瑞利型衰落、频率弥散和频率选择性衰落，即造成信号的快衰落，抵抗措施有分集接收技术、扩频技术、OFDM技术、Rake接收技术和智能天线技术等。
*简述数字通信系统相比于模拟通信系统的优缺点
答：数字通信系统的优点有：抗干扰能力强、传输差错可控、易于集成、便于处理等；缺点有占用较大带宽和需要同步等。
*指出模拟通信系统和数字通信系统各自有效性和可靠性的指标
答：模拟通信系统的指标分别为带宽和信噪比；数字通信系统则为信息速率和误码率。
*列举通信系统中提高传输可靠性的措施（2011年）
答：信道编码、均衡、加重技术
*列举通信系统中提高传输有效性的措施
答：信源编码、部分响应技术、升余弦滚降系统、正交频分复用
	信号与噪声分析
*简述高斯随机过程的至少3个特点
答：高斯随机过程的不相关性和独立性等价、若干个高斯随机过程的线性组合仍为高斯过程，高斯过程的狭义平稳和广义平稳等价。
*简述随机过程与随机变量的关系（2008）
答：随机过程是在时间进程中不同时刻随机变量的集合，即随机过程在任意时刻的值就是一个随机变量。随机变量是随机过程在某一时间上的分布。
*简述白噪声的概念及其功率谱和自相关函数的特点（2012年）
答：功率谱密度在所有频率上均为同一常数的噪声称为白噪声，自相关函数为冲激函数，即任意两个时刻的随机变量不相关。
*简述窄带噪声的概念及其波形特点和包络、相位各自遵循的分布函数类型。（2017年）
答：在窄带传输系统中接入加性高斯白噪声，称为窄带高斯噪声，其波形特点为包络和相位均缓慢变化，其中包络服从瑞利分布，相位服从均匀分布。
*简述一个平稳随机过程具备各态历经性的条件及其现实意义（2016）
答：一个平稳随机过程具有各态历经性的条件是其均值和自相关函数的时间平均值等于统计平均值，意义是任意一次实现都历经了随机过程所有的可能状态，无需测大量样本。
*简述广义平稳和狭义平稳的概念以及二者的关系（2015）
答：一个统计特性与时间起点无关的随机过程称为狭义平稳随机过程；一个均值与时间无关且自相关函数只与时间间隔有关的随机过程称为广义平稳随机过程，对于一般的随机过程，狭义平稳是广义平稳的充分不必要条件，对高斯随机过程而言，二者等价。
	模拟调制系统
*简述调制的概念及其分类与意义
答：调制是把信号转换成适合在信道中传输的过程。根据调制信号可分为模拟调制和数字调制，根据载波可分为连续载波调制和脉冲编码调制。调制的意义有：扩展信号带宽，提高系统抗干扰能力；实现信道多路复用，提高信道利用率；减小天线尺寸。
*简述残留边带滤波器的特点及其相较于单边带调幅和双边带调幅的优势（2011年）
答：残留边带滤波器的系统函数在载波角频率处具有互补对称性，使其在相干解调时能无失真地恢复调制信号。相比于双边带调幅，其占用带宽小，相比于单边带调幅，其更容易实现。
*简述门限效应的概念及其成因，模拟调制系统中哪些会产生门限效应
答：门限效应是指当输入信噪比低于一定值时，解调器的输出信噪比不随着输入信噪比按比例下降，而是急剧恶化的现象。门限效应是由包络检波器的非线性解调作用引起的。包含载波的调幅（AM）采用包络检波解调和调频系统均会产生门限效应。
*简述调频系统中加重技术的原理和意义（2014年）
答：调频系统易发生门限效应，使用加重技术，在调制器前加入预加重滤波器，提升调制信号的高频分量，在解调器前加入去加重滤波器，将调制信号高频端的噪声衰减，并把调制信号高频分量的幅度恢复为初始值。（预加重滤波器和去加重滤波器的系统函数互为倒数）。
*简述过调幅失真的成因及其对调幅系统造成的影响，为什么DSB和SSB不会产
生该现象而AM会？（2009年）
答：调幅系统中若调制信号幅度大于外加直流分量，则产生过调幅，用包络检波法解调会产生失真，因为SSB和DSB均抑制了载波，故不会产生该现象。
*比较调幅系统和调频系统的抗噪声性能（2013年）
答：B（FM）=2（β+1）f=（β+1）B（AM）。调频系统和调幅（AM）的输出信噪比正比于二者的带宽之比的平方，即等于9*（β+1）*（β+1）。故在调制信号和噪声功率谱密度相同的情况下，调频系统抗噪声优于调幅系统。

	模拟信号数字化
*分别简述折叠码和格雷码各自的特点以及优缺点
答：折叠码：用最高位表示电压的极性正负，其余位表示绝对值，即正负极性相对称的部分中只有最高位不同，其余位相同。该码可用单极性编码方法处理双极性电平，简化编码电路和编码过程。
    格雷码：格雷码属于可靠性编码，是一种错误最小化的编码方式，其任意两个相邻的代码只有一位二进制数不同。常用于将模拟量转化为用连续二进制序列表示数字量的系统中 当模拟量发生微小变化而引起数字量从一位变化到相邻位时 在转化过程中 会产生瞬间错误数码，而格雷码可以避免错误数码的产生。
*简述预测编码的原理及其意义
答：预测编码不对抽样值进行独立编码，而是根据前几个抽样值计算出一个预测值，对当前抽样值和预测值进行编码与传输，它利用了相邻抽样值之间的相关性，减小了冗余信息，降低了编码比特率。
*简述模拟信号数字化传输系统的三个功能模块及其各自功能
答：模数转换、数字基带或频带传输系统、数模转换。模数转换通过抽样、量化、编码等功能将模拟信号转换为数字信号，便于进行数字通信，传输系统对信号进行调制等处理后进行传输并解调，数模转换恢复原始模拟信号。
*简述模数转换过程中的三个步骤以及每个步骤的功能
答：抽样、量化、编码。抽样令模拟信号成为时间离散而取值连续的模拟信号，量化对抽样信号的取值进行离散化，使其成为数字信号，编码将量化信号调制为二进制或其他进制的序列，常用脉冲编码调制。
*简述非均匀量化的实现方法和优缺点（2016）
答：非均匀量化方法为先对信号的抽样值进行压缩后再进行均匀量化。在语音信号的量化中，采用类似对数形式的压缩特性，故小信号的量化间隔小，大信号的量化间隔大，所以小信号的量化误差小，由于语音信号中小信号分量多，故采用非均匀量化可以减小总体量化误差。
*简述增量调制系统中量化噪声的分类及其成因
答：一般量化噪声和过载量化噪声。一般量化噪声是由于编码、译码时用阶梯波形去近似模拟信号波形，由阶梯的突跳性产生的，不可避免；过载量化噪声当输入信号上升斜率大于阶梯波最大可能斜率是产生。
*简述使增量调制不发生过载的方法（2008年）
答：根据过载量化噪声产生的原理，采用增大抽样频率的方法，可以保证基本量化噪声和过载量化噪声都不超过要求。
*简述A律PCM设计目标及其技术特点（2005年）
答：技术特点：采用非均匀量化，对抽样值大的信号用较大的量化间隔。
    目标：改善小信号的量化信噪比，提升整体性能。
	数字信号的基带传输
*简述奈奎斯特第一准则（2015年）
答：奈式第一准则为：在理想低通信道条件下，最高码元传输速率为2Baud/Hz，若为理想带通信道，则最高速率为1Baud/Hz，若超过该极限速率，则发生码间干扰。
*简述奈奎斯特速率和奈奎斯特带宽的概念（2012年）
答：奈奎斯特速率：基带传输系统无码间干扰下的理论最高传输速率
    奈奎斯特带宽：在无码间干扰的数字基带传输系统中，设码元长度为Ts，则1/2Ts称为奈奎斯特带宽。
*简述奈奎斯特第二准则
答：有控制地在某些码元的抽样时刻引入码间干扰，而在其余码元的抽样时刻无码间干扰，就能使频带利用率达到理论上的最大值，同时又可降低对定时精度的要求。通常把满足奈奎斯特第二准则的波形称为部分响应波形。利用部分响应波形进行传送的基带传输系统称为部分响应系统。
*简述基带传输系统中码型的设计原则（2017年）
答：在传输方面，要求无直流且低频分量少、功率谱主瓣宽度窄、适应信源特性的变化；在接收方面，要求定时信息丰富、有内在检错能力；另外还要求编译码简单，节约成本。
*简述产生码间干扰及其原因和消除码间干扰的基本思想和条件以及几种方法（2013年）
答：概念与成因：由于系统传输特性不理想，导致码元波形发生畸变，使前面码
元波形出现很长拖尾蔓延到当前码元的抽样时刻上，从而对当前码元的判决造成
干扰，即码间串扰。码间串扰属于乘性干扰，只要信道频带有限，就一定有码间
串扰。
基本思想与条件：若前一码元的波形在后一个码元的抽样判决时刻值为零，
就可满足要求，即只要基带传输系统的冲激响应波形h（t）只在当前码元抽样判决时刻有最大值，且在其他码元的抽样时刻为0，即可消除码间串扰。
方法有：
均衡技术：均衡技术是补偿信道特性，使其满足无码间串扰条件的技术。分
为频域均衡和时域均衡，频域均衡适用于信道特性不变，且低速传输的情况，其在基带系统中插入滤波器，补偿包括滤波器在内的整个系统的频率特性，减小码间串扰的影响； 时域均衡通过精准设计的横向滤波器搭配抽头系数，使系统尽可能满足无码间串扰的时域条件，若横向滤波器有无数个，则理论上可以完全消除码间串扰。（2015年）
多载波调制技术：将信道分成若干子信道，将基带码元均匀分散地对每个子信道的载波进行调制，降低子载波的调制码元速率并减小子信道带宽，若子信道带宽足够小，可认为信道特性接近理想信道特性，有效克服码间串扰。
余弦滚降：基于满足奈奎斯特第一准则的极限情况---理想低通型，设计了余弦滚降特性，使理想LPF的边沿缓慢下降，只需其系统函数H(w)在滚降中心频率处呈奇对称特性，就可满足Nyquist第一准则，实现无码间干扰。
*简述部分响应系统的原理及其优点
答：有控制的在某些码元的抽样时刻引入码间干扰，而在其余码元的抽样时刻无码间干扰，那么就能使频带利用率提高到理论上的最大值，同时又可以降低对定时精度的要求，通常把这种波形称为部分响应波形。利用部分响应波形进行的基带传输系统称为部分响应系统。因为引入的码间干扰是确知的，所以从最终抽样的结果中剔除掉码间干扰，就可以获得本码元的抽样值。能够较好的提高频带利用率。
*简述相关电平编码的概念及其设计依据
答：相关电平编码又称为双二进制编码，它由一个双二进制滤波器和一个奈氏滤波器构成，使信道承载了两倍的二进制载荷，使当前的码元只对下一个码元产生干扰，通过预编码和模2判决消除。
*列举出升余弦频谱的特点（至少三条）
答：在抽样时刻无码间干扰，抗定时抖动能力强，付出了额外的α*f_█(N@)的带宽代价。
*什么是眼图，通过眼图可以看出基带传输系统的哪些性能（2009）年
答：用示波器跨接在抽样判决器输入端，调整示波器水平扫描周期使其与接收码元周期同步，可从示波器上观察到码间干扰和信号噪声等因素影响的情况，具体有最佳抽样时刻、定时误差灵敏度，信号畸变程度，判决门限电平，噪声容限，过零点畸变。
	数字信号的频带传输
*为什么采用频带传输？
答：基带传输系统中，由于基带信号的宽频性和丰富的低频分量，限带脉冲的波形流散导致码间干扰，使传输性能差，故采用频带传输系统，用基带信号调制载波，使信号与信道匹配。
*为什么普通的2FSK频带利用率低？如何解决？
答：用不同频率的独立载波分别表示传号与空号，在1，0转换时不能保证相位连续，相位的跳变进而引起了载波包络的起伏，使信号的功率谱旁瓣衰减缓慢，降低信道的带宽利用率。解决方法为采用压控振荡器(VCO)作为调制单元，可使相位连续。
*为什么引入相对差分相移键控？
答：绝对相移键控的相干检测，若接收端以锁相环形式提取相干载波，可能会使相干载波被锁定在与接收载波相差2π/M的相位，（M为进制数），对于2PSK就导致π相模糊，故将原码变为差分码再去调制，利用差分码之间的相关性，消除π相模糊。
*简述多进制调制相比于二进制调制系统的优缺点（2009年）
答：多进制调制每个码元相比于二进制携带了更多的信息，因此提高了信息速率即提高了有效性，但是可靠性有所下降，其误码率更大。



	数字信号的最佳接收
*简述三种最佳接收机各自遵循的准则及原理
答：匹配滤波器--最大输出信噪比准则；（匹配滤波器的冲激响应使得该滤波器能与信号达到最大程度的适配同时抑制或削弱噪声）。
相关接收机—最小均方误差准则；（相关接收机提供了两个（因为二进制）本地样本函数，用以和接收机的输入信号计算互相关性，信号和哪个样本相关性最强则判为哪个信号）。
最佳接收机—最大后验概率或最大似然准则。
*简述3种最佳接收机等价的条件
答：信道为高斯信道、输入的二元或多元信号先验概率已知或假定相等
*简述匹配滤波器的设计要求及何时输出最大信噪比和输出信号波形
答：接收滤波器的冲激响应为接收波形的镜像延迟（镜像保证了二者最强的互相关性，延迟保证了因果性）。输出信噪比最大时刻为接收码元结束的时刻，输出信号波形为接收信号的自相关函数的延迟。
	信道编码
*简述差错控制的分类及各类别的特点
答：1.前向纠错(FEC)：发送时在信息序列后加上监督码元，接收端可以根据监督规则自动识别并纠正错误。适于高速实时传输，但编译码较复杂。
2.反馈重发(ARQ)：接收端检查接收码，若无误，则反馈确认信息ACK，若有错则反馈NAK请求发送端重新发送，它比FEC需要额外的反馈信道，该差错控制方式适于非实时低速传输。
3.混合纠错(HEC)：是以上两种方式的有机结合，在纠错能力内能予以纠错，超出纠错能力的要求重发，，适于实时传输。
4. 信息反馈(IRQ)：是最简单的差错控制方式，接收端原封不动地将接收码发回给发送端并与发送码进行比较，若发现错误，则重发，适于低速非实时传输。
*简述汉明码的特点（2011年）
答：汉明码属于线性分组码，其最小码距为3，可纠一位错，与其他能纠一位错的等长码相比，其所用监督位最少，即码率最高。（汉明码属于完备码）。
*什么是完备码（2004年）
答：满足等式2^r-1=n的（n，k）线性分组码称为完备码，其监督矩阵H共有（2^r-1）列，每一列都是一个码字，加上全零码字，构成2^r个码字，即错误图样总数等于伴随式数目。
*简述卷积码的特点及其与分组码的区别（2009年）
答：分组码中每一码组的监督员仅与本组的k位信息元有关，卷积码则不然，编码的监督码元不仅和当前的k位信息元有关，也和前面的(N-1)个信息段有关，（即一个一个码组的监督码元监督着N个信息段，N称为编码约束度，nN称为编码约束长度）卷积码的n和k都很小，适于串行传输，延时很小。卷积码常用维特比算法解码。
	常用的现代调制技术
*简述最小频移键控系统的特点和优势（2013年）
答：MSK是一种特殊的2FSK信号，其相位连续，包络恒定，占用带宽达到理论最小值，且严格正交。
*简述正交频分复用的基本思想及设计原理和实现步骤和优缺点（2010年）
答：基本思想和设计原理：OFDM采用了多载波调试的基本思想，降低了每个子载波的调制码元速率和子信道的带宽以克服码间串扰。OFDM将信道分成若干正交子信道，将高速数据信号转换成并行的低速子数据流，调制到在每个子信道上进行传输。正交信号可以在接收端分开，这样可以减少子信道之间的相互干扰(ISI) 。每个子信道上的信号带宽小于信道的相关带宽，因此每个子信道上可以看成平坦性衰落，从而可以消除码间串扰。
    实现步骤：调制：分帧分组、串并变换---编码映射---IDFT---并串变换—数模转换—上变频发射。
    特点和优点：相邻子载波的频谱有1/2重叠，得益于正交性不用信道保护间隔，故信道利用率高，抗多径传播。
    缺点：由于要保证子信道严格的正交性，其对信道产生的频率偏移和相位噪声很敏感；信号峰值功率和平均功率值较大，会降低射频功率放大器的效率。
*简述各种改进型QPSK的原理及意义
答：O(off-set)QPSK：在QPSK的一个支路中加入一个延迟单元Tb，，使两个支路上的基带码元的变换相差一个比特间隔，即每隔一个比特间隔只有一个支路发生相位变换，原来QPSK会出现的π相突变，变为最大只有π/2。
    π/4QPSK：由两个相差π/4的QPSK星座图交替运用，使最大相差变为3π/4.

	多用户通信（初试不考）
	现代通信网及其发展（不考）

