安装与升级
==========

wechatpy 依赖 six, requests 才能正常运行，目前 wechatpy 支持的 Python 环境有 2.6, 2.7, 3.2, 3.3, 3.4, pypy 和 pypy3。

为了简化安装过程，推荐使用 pip 进行安装::

    pip install wechatpy

升级 wechatpy 到新版本::

    pip install -U wechatpy

如果需要安装 GitHub 上的最新代码::

    pip install https://github.com/messense/wechatpy/archive/master.zip


从 0.8.0 版本开始，wechatpy 消息加解密同时兼容 cryptography 和 PyCrypto, 优先使用 cryptography 库。
因而不再强制依赖 PyCrypto 库。如需使用消息加解密（企业号平台必须），请自行安装 cryptography 或者 PyCrypto 库::

    # 安装 cryptography
    pip install cryptography>=0.8.2
    # 或者安装 PyCrypto
    pip install pycrypto>=2.6.1
