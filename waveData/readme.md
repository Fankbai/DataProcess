
#waveData ͨ�ð����������ݷ���
##DataPlot ���ݻ���
- _plotWaterFall ����Ƶ��
Args:
    x: list
        x������list,��ÿ��Ԫ������Ҫ���Ƶ�x������
    y: list
        y������list,��ÿ��Ԫ������Ҫ���Ƶ�y������,
        ����ע�⣺�����y������z�����
    type:string
        type = 'line'��������ʽ����waterfall��type='poly'���߷�line���������״��ʽ����
    fig: matplotLib.figure
        ��ͼ�����������룬��û��ax������������ax
    ax:
        ����ϵ��Ĭ��ΪNone,���Զ�����
    order: list
        ÿ��x,y��Ӧ�����,������ã���1��ʼ������len(x)
    edgecolors:
        �߽�����ɫ
        (0,0,0,0):int,int,int,int:R,G,B,A
    facecolors:
        �����ɫ
        (0,0,0,0):int,int,int,int:R,G,B,A
	sameColor:
        ������type='line'ʱ����ɫһ��
        (0,0,0,0):int,int,int,int:R,G,B,A
Return:
    [fig,ax] : list
        ����fig��ax����ָ��������ԭ������ûָ���������µ�
type = 'line'ģʽ��

![](https://github.com/czyt1988/DataProcess/raw/master/waveData/doc/DataPlot/01-_plotWaterFall-type-line.png)

type = 'poly'ģʽ��

![](https://github.com/czyt1988/DataProcess/raw/master/waveData/doc/DataPlot/02-_plotWaterFall-type-poly.png)

type = 'line',sameColor='r' ģʽ��

![](https://github.com/czyt1988/DataProcess/raw/master/waveData/doc/DataPlot/03-_plotWaterFall-type-line-sameColor.png)
