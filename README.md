# Auto Monkey For Android #

### �汾 1.1

### ���ܼ�� ###
1. ��ȫ�Զ���ֻ��Ҫ���������豸
2. ֧�ֶ���豸
3. ֧����ʱ�Ͽ��豸���������豸��ÿ5s��ʱ����豸�Զ�����
4. �����󣬷����ʼ����ʼ����ݣ�ִ��ʱ����crash log
5. ֧��Windows��Macϵͳ
6. ֧�������ļ�

### ϵͳ������������ ###
1. ���Ի�����Mac OS��Windows 10��Python 2.7.10
2. ���� **adb**

### �����޸� ###
user_config/default.conf

    ```
    [config]
    package_name = com.testerhome.nativeandroid
    adb_location = /Users/smzdm/Documents/01_Android/adt-bundle-mac-x86_64-20140702/sdk/platform-tools/adb

    # �������������
    mail_host = smtp.xxxx.com
    # �����˺�
    mail_user = xxxxxx@xxx.com
    # ��������
    mail_pass = ******

    [mail_to_list]
    # ���÷��͸��ռ���, ��ʽ���£��Ⱥ��Ҳ�����
    aaaaaa@163.com =
    bbbbbb@163.com =

    [monkey_parameters]
    # monkey ��صĲ�������Ҫ��Щ��ֱ�������水��ʽ���ȥ��ǰ��� # ���ż���. ����Ҫ��ֵ�Ĳ����Ⱥź������վͿ���
    -v =
    --throttle = 300
    --pct-trackball = 0
    --pct-syskeys = 5
    --pct-nav = 0
    --pct-anyevent = 0
    # --pct-majornav = 0
    # --pct-appswitch = 0
    # --pct-flip = 0
    # --pct-pinchzoom = 0
    # --pct-permission = 0
    # --pct-touch = 0
    # --pct-motion = 0

    # COUNT ������Ҫ�������
    4000000 =
    ```

### ���� ###

1. ִ������
    ִ��Ĭ�������ļ��� user_config/default.conf

    ```shell
    python /your_location/monkey_android/performance/monkey/monkey_server.py`
    ```
    ִ���Զ��������ļ�(monkey_android/user_config ·����)��user_config/custom.conf

    ```shell
    python /your_location/monkey_android/performance/monkey/monkey_server.py user_config/custom.conf
    ```
    ����ʹ�������ļ���ȫ·��
    ```shell
    python /your_location/monkey_android/performance/monkey/monkey_server.py /your_dir/custom.conf
    ```
2. �����ֻ�

### �ر�monkey ###

1. ͣ��monkey_server��ǰ����û���������е� monkey_server
2. ����monkey_stop

    ```shell
    python /your_location/monkey_android/performance/monkey/monkey_stop.py
    ```
3. ������һ̨û��monkey_server �ĵ��ԣ�ִ�������ֻ�

    ```shell
    adb reboot
    ```


### �ʼ���ͼ ###
<img alt="summary" src="https://github.com/wangyunshuai/monkey_android/blob/master/performance/img/mail.png">


