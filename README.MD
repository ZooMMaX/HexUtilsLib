# HexUtilsLib

![Maven Central](https://img.shields.io/maven-central/v/ru.zoommax/HexUtilsLib?color=00ff)

### convert byte[] to hex

```java
import ru.zoommax.HexUtils;

public class Main {
    public static void main(String[] args) {
        byte[] b = {(byte) 0x01, (byte) 0x02, (byte) 0x03, (byte) 0x04};
        String hex = HexUtils.toString(b);
    }
}
```
```shell
output: 01020304
```
---

### convert hex to byte[]

```java
import ru.zoommax.HexUtils;

public class Main {
    public static void main(String[] args) {
        String hex = "ABCDEF29";
        byte[] b = HexUtils.fromString(hex);
    }
}
```
```shell
output: 0xAB, 0xCD, 0xEF, 0x29.
```