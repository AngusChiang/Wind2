#### ����
- [ ] UdpЭ�鱻�� => WIP
- [ ] UdpЭ����ƶ�
- [ ] ��Ԫ��ѡ�Ƿ���ҪWind2����־
- [ ] WebSocketЭ�����(���ƶ��޼ƻ�)
- [ ] ��Ԫָ��Ȩ��(�û�)����

#### ��װ
- �������=>ʹ�ù���ԱȨ��ִ��`dotnet Host.dll action:install`
- ����=>ʹ�ù���ԱȨ��ִ��`Host.exe action:install`
- ������Ҫ�ֶ�ȥ����������(services.msc)���� Wind2 ����

#### ж��
- �������=>ʹ�ù���ԱȨ��ִ��`dotnet Host.dll action:uninstall`
- ����=>ʹ�ù���ԱȨ��ִ��`Host.exe action:uninstall`

#### ��Ԫ����
��Ԫ������һ��JSON�ı��ļ�,����`ASCII(ANSI)`,��ʽ����
```json
{
    //Ӧ�ó������·��
    "AbsolutePath": "C:\\Windows\\System32\\nslookup.exe",
    //Ӧ�ó�����Ŀ¼,����Ӧ�ó�����Ҫ����,���鶼��д
    "WorkPath": "C:\\Windows\\System32\\",
    //Ӧ�ó������
    "Params": "-qt=A www.ragnaroks.org",
    //Ӧ�ó����Ƿ�������
    "AutoStart": true,
    //Ӧ�ó��������ӳ�,��λ��
    "AutoStartDelay": 10,
    //�Ƿ��¼��־,���ǰ��Ч,����·�
    "EnableLogger": false
}
```
�������ô�����Wind2��ʼ����ɺ�,�ȴ�10��,������`C:\Windows\System32\nslookup.exe -qt=A www.ragnaroks.org`,�������ù���Ŀ¼`C:\Windows\System32\`  

��ʽ�����δ��дӦ�ó������·����Ӧ�ó����ļ�������,��˵�Ԫ�ļ��ᱻ����,��Ԫ�����ļ��������Wind2Ŀ¼�µ�Units�ļ�����  

`EnableLogger`���Ϊ`true`,��õ�Ԫ���¼**����Wind2��**��־,��Ӧ�ó���������־�����޹�,**��ǰǿ�Ƽ�¼**


#### ȫ������
ȫ��������һ����Ϊ**AppSettings.json**��JSON�ı��ļ�,����`ASCII(ANSI)`,λ�ڶ����Ƹ�Ŀ¼��,��ʽ����
```json
{
    //��־����,��ǰ��Ч
    "LogLevel": 0,
    //�Ƿ����ñ���,�߽��û�����������
    "ControlEnable": false,
    //���ؼ���IPv4��ַ,����'localhost'ֻ��������,'any'��������
    "ControlAddress": "localhost",
    //���ض˿�,����С��1024
    "ControlPort": 27015,
    //������Կ,���ⳤ�������ַ�,����16�ֽ�����,���غͿ��ƶ�ʹ��AES����ͨ��
    "ControlKey": "https://github.com/ragnaroks/Wind2"
}
```

#### ע������
- ���йܵ�Ӧ�ó���Ĭ�ϲ�֧��**����**,��Ҫ������`services.msc`����
- ��ǰ��֧���й���ͼ������Ӧ�ó���
- ���йܵ�Ӧ�ó���Ĭ��ΪLOCAL SYSTEMȨ��,����ֻ�й�**������**��Ӧ�ó���