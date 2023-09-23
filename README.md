# encoderDemo
Java处理url\md5\base64编码案例 -基于Java  
```java
    public static void main(String[] args) throws EncoderException {
        Base64 base64 = new Base64();
        String s = base64.encodeToString("您好".getBytes());
        System.out.println(s);
        String s1 = DigestUtils.md5Hex(s);
        System.out.println(s1);
        String url = "http://baidu.com?name=你好";
        URLCodec urlCodec = new URLCodec();
        System.out.println(urlCodec.encode(url));
    }
```
```java
oldstr="您好";
Base64.Encoder encoder = Base64.getEncoder();//Base64在java.untl包下
String newstr = encoder.encodeToString(oldstr.getBytes("utf-8"));
```
