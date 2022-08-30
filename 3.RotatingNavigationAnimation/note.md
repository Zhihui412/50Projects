# 实现左上角只显示四分之一圆角
原理:外层容器设置绝对定位，定位到外层容器的中心是左上角顶点，在设置里面的容器50%，这样就直露出1/4部分
//HTML
```
        <div class="circle-container">
            <div class="circle">
            </div>
        </div>
```

//css
```
.circle-container{
    position: fixed;
    top: -100px;
    left: -100px;
}

.circle{
    background-color: #ff7979;
    height: 200px;
    width: 200px;
    border-radius: 50%;
}
```