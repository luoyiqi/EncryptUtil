# EncryptUtil

android AES\DES\DES3\RSA加密，详情见博客http://blog.csdn.net/u011697203/article/details/64921882

```
使用AES\DES\DES3

String strTestData = "MainActivity";

//加密
String AesEncryptECB = EncryUtils.AesDesEncrypt(strTestData,AES_KEY,"",EncryUtils.Encryption.AES, EncryUtils.EncryptMode.ECB);

//解密
EncryUtils.AesDesDecrypt(AesEncryptECB,AES_KEY,"", EncryUtils.Encryption.AES,EncryUtils.EncryptMode.ECB)


使用RSA
String rsaTestData = "asdgasgegesgasdgasgegesgasdgasgegesgasdgasgegesgasd";


String encryptPub = RSAUtil.EncryptDataOfPublicKey(rsaTestData,mContext.getResources().openRawResource(R.raw.rsa_public_key));


String decryptPri = RSAUtil.DecryptDataOfPrivateKey(encryptPub,mContext.getResources().openRawResource(R.raw.rsa_private_key));
```
