#### ��װ
- �������=>ʹ�ù���ԱȨ��ִ��`dotnet Host.dll action:install`
- ����=>ʹ�ù���ԱȨ��ִ��`Host.exe action:install`

#### ж��
- �������=>ʹ�ù���ԱȨ��ִ��`dotnet Host.dll action:uninstall`
- ����=>ʹ�ù���ԱȨ��ִ��`Host.exe action:uninstall`

#### ��Ԫ����
��Ԫ������һ��JSON�ı��ļ�,����`ASCII(ANSI)`,��ʽ����
```json
{
    //Ӧ�ó������·��
    "AbsolutePath": "C:\\Windows\\System32\\ping.exe",
    //Ӧ�ó�����Ŀ¼,����Ӧ�ó�����Ҫ����,���鶼��д
    "WorkPath": "C:\\Windows\\System32\\",
    //Ӧ�ó������
    "Params": "hello.wind2",
    //Ӧ�ó����Ƿ�������
    "AutoStart": true,
    //Ӧ�ó��������ӳ�,��λ��
    "AutoStartDelay": 10,
    //�Ƿ����̨Ӧ�ó���,���ǰ��Ч,����·�
    "IsConsoleApp": false,
    //�Ƿ��¼��־,���ǰ��Ч,����·�
    "EnableLogger": false
}
```
�������ô�����Wind2��ʼ����ɺ�,�ȴ�10��,������`C:\Windows\System32\ping.exe`,�������ù���Ŀ¼`C:\Windows\System32\`  

��ʽ�����δ��дӦ�ó������·����Ӧ�ó����ļ�������,��˵�Ԫ�ļ��ᱻ����,��Ԫ�����ļ��������Wind2Ŀ¼�µ�Units�ļ�����  

- `IsConsoleApp`���Ϊ`true`,��õ�Ԫ����**�����д���**,��stdIO�ᱻ�ض���  
- `EnableLogger`���Ϊ`true`,��õ�Ԫ���¼��־
- ��ǰ��֧���й���ͼ������Ӧ�ó���