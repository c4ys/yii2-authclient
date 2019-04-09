Yii Authclient for Weibo,QQ,Wechat

**Demo**
http://simpleforum.org/site/login

**Config Setting**

```
'components' => [
    'authClientCollection' => [
        'class' => 'yii\authclient\Collection',
        'clients' => [
            'weibo' => [
                'class' => 'c4ys\authclient\Weibo',
                'clientId' => 'wb_key',
                'clientSecret' => 'wb_secret',
            ],
            'qq' => [
                'class' => 'c4ys\authclient\Qq',
                'clientId' => 'qq_appid',
                'clientSecret' => 'qq_appkey',
            ],
            'weixin' => [
                'class' => 'c4ys\authclient\Weixin',
                'clientId' => 'weixin_appid',
                'clientSecret' => 'weixin_appkey',
            ],
              'weixinmp' => [  // for account of https://mp.weixin.qq.com/
                  'class' => 'c4ys\authclient\Weixin',
                  'type' => 'mp',
                  'clientId' => 'weixin_appid',
                  'clientSecret' => 'weixin_appkey',
              ],
        ],
    ]
    // other components
]
```
