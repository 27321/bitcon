# bitcon
【项目名称】 forge a signature to pretend that you are Satoshi

【项目简介】伪造一个签名假装自己是中本聪（参考新闻）。

【代码说明】

ECDSA的哈希部分是算法不可获取的部分。如果验证者本身没有运行哈希，则ECDSA的安全属性不会成立，伪造会变得微不足道。

如果验证者自己不执行哈希，但仅接受签名者给出的值，则给定公钥P，选择随机非零值a和b，计算R=aG+bP，那么， (R.x, R.x/b)是密钥P对消息哈希 (R.x*a/b)的有效签名。

![image](https://user-images.githubusercontent.com/105579212/180791518-f0c1cd8c-0fe1-441c-bca2-d7549165692a.png)


【运行截图】
![image](https://user-images.githubusercontent.com/105579212/180790263-6f09af54-a00b-4d1c-b268-9ace650e16a9.png)
