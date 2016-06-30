
#waveData ͨ�ð����������ݷ���
##DataPlot ���ݻ���

### _plotWave ���Ʋ���
	ֻ��Ҫһ��wave���ݣ��Ͳ����ʼ��ɻ��Ʋ���
    Args:
        wave:numpy.array ����
        fs:int ������
        ax:matplotlib.ax ��ͼ����ϵ
        color:str or rgb ��ͼ��ɫ
        **kwargs:matplotlib.axes.plot��**kwargs����
    Returns:
        [x,[fig,ax]]:list
            xֵ��[fig,ax]
���磺
```Python
print('_plotWave example')
fs = 10
wave = [1,2,3,5,1,2,4,7,4,6,7,3,2,4,6,8,9,7,6,5,4,2,4,7]
dp._plotWave(wave,fs)
plt.show()
```
![](https://github.com/czyt1988/DataProcess/raw/master/waveData/doc/DataPlot/06-_plotWave.png)


### plotWave  ����һ������ _plotWave�ķ�װ������IData����
����һ��ѹ��ͼ��
    Args:L
        iWaveData:Data���������ȼ���һ��csv����
        indexOrName:int/str
            ����������ͨ�����ƣ�������0��ʼ��ͨ������Ϊstr����

    Returns:
        [[x,y,otherInfo],[fig,ax]]



### _plotWaterFall ����Ƶ��

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

![](https://github.com/czyt1988/DataProcess/raw/master/waveData/doc/DataPlot/01-_plotWaterFall-type-poly.png)

type = 'poly'ģʽ��

![](https://github.com/czyt1988/DataProcess/raw/master/waveData/doc/DataPlot/02-_plotWaterFall-type-line.png)

type = 'line',sameColor='r' ģʽ��

![](https://github.com/czyt1988/DataProcess/raw/master/waveData/doc/DataPlot/03-_plotWaterFall-type-line-sameColor.png)


### plotSpectrum

����ʱƵ����STFT,��matplotlib.plt.spectrum�ӿ�һ�£����ǣ���ֵ������amplitude��ͨ��mode���ã��磺

dp.plotSpectrum(wave,Fs = fs,detrend = 'mean'
,NFFT = NFFTSize,noverlap=int(NFFTSize/4),mode='amplitude'
,plotType = 'other',scale='linear',sameColor='r')
![](https://github.com/czyt1988/DataProcess/raw/master/waveData/doc/DataPlot/04-plotSpectrum.png)

plotType = '3d'ʱ�������ߵķ�ʽ����

![](https://github.com/czyt1988/DataProcess/raw/master/waveData/doc/DataPlot/05-plotSpectrum-3d.png)