# alipay_install
我在运行的时候报错ImportError: cannot import name 'Alipay' from 'alipay'
  这个表示安装的包重复了 
  我了解到有两个保存在
    alipay-sdk-python	3.3.398	官方
    python-alipay-sdk	2.0.1	第三方
  我先安装了官方的 然后又安装了第三方的 所以报错 后来我吧两个都卸载了 然后运行pip install alipay
  没有报错 但是调用不了支付的接口函数
  最后经过尝试 发现官方的旧版本适应python但是新版本中没有适应python所以我特地找了官方旧版本 可以尝试
  
  第三方的安装 也就是我上传的alipay.zip
  解压之后 python setup.py install就可以了
  官方有两个文件 一个是.whl结尾的 直接 pip install 跟上文件名字即可
                 一个是两重压缩包 解压以后直接python setup.py install就可以了
  不推荐直接pip install alipay
