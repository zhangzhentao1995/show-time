# 实时时间展示（HTML+JS）
## 效果
https://blog.csdn.net/zt_16KK/article/details/93158549
## HTML代码
```
<span id="time"></span>
```
## JS代码
```
    setInterval("setTime()", 1000);
    function setTime() {
        var d = new Date();
        document.getElementById("time").innerHTML =
            d.getFullYear() + "-" + addZero((d.getMonth() + 1)) + "-" + addZero(d.getDate()) + " "
            + addZero(d.getHours()) + ":" + addZero(d.getMinutes()) + ":" + addZero(d.getSeconds());
    }
    function addZero(d) {
        if (d < 10) {
            return "0" + d;
        } else {
            return d;
        }
    }
```
## 博客
https://blog.csdn.net/zt_16KK/article/details/93158549
