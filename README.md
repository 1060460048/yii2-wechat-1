yii2-wechat
===============


��������
------------
- >= php5.4
- Yii2

��װ
------------

������ʹ��composer����װ, ������д���������``composer.json``�ļ��в�ִ��``composer update``����

```json
{
    "require": {
       "lujian/yii2-wechat": "dev-master"
    }
}
```

ʹ��ʾ��
------------
��ʹ��ǰ,���Ȳο�΢�Ź���ƽ̨��[�����ĵ�](http://mp.weixin.qq.com/wiki/index.php?title=%E9%A6%96%E9%A1%B5)

Wechat���巽ʽ
```php
//��config/web.php�����ļ��ж���component������Ϣ
'components' => [
  .....
  'wechat' => [
    'class' => 'lujian\wechat\Wechat',
    'config' => [
        'token'=>'tokenaccesskey', //��д���趨��key
        'encodingaeskey'=>'encodingaeskey', //��д�����õ�EncodingAESKey
        'appid'=>'wxdk1234567890', //��д�߼����ù��ܵ�app id, ����΢�ſ���ģʽ��̨��ѯ
        'appsecret'=>'xxxxxxxxxxxxxxxxxxx', //��д�߼����ù��ܵ���Կ
        'partnerid'=>'88888888', //�Ƹ�ͨ�̻���ݱ�ʶ��֧��Ȩ��ר�ã�û�пɲ���
        'partnerkey'=>'', //�Ƹ�ͨ�̻�Ȩ����ԿKey��֧��Ȩ��ר��
        'paysignkey'=>'' //�̻�ǩ����ԿKey��֧��Ȩ��ר��
    ]
  ]
  ....
]
// ȫ�ֹ��ں�sdkʹ��
$wechat = Yii::$app->wechat;




```

�������״���
------------
��������[����](https://github.com/lujian/yii2-wechat/issues)���������ʹ���������������Bug.
�һ��ڵ�һʱ��ظ������޸�.

��Ҳ���� �����ʼ�254461627@qq.com���Ҳ���˵����������.

������и��ô���ʵ��,��fork��Ŀ����������pull request.�һἰʱ����. ��л!