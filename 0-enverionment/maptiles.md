# 离线瓦片器

 

>  注意：需要在可以连接互联网的情况下进行下载，下载时可先设置一个级别（在配置文件conf.properties中仅仅设置zoom=10）进行下载测试，下载完成后进入设置的下载路径downloadDir看是否有图片可以下载到。若可以下载到，则进行1到17级统一下载。



具体参看以下配置。

用文档编辑器打开bin目录下的conf.properties文件中，修改以下参数。

```properties
#download directory 下载路径
downloadDir=D:\\GoogleMap\\

#zoom=10,11,12,13,14,15（下载至17级）   
zoom=1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17

#leftTopLnglat  118.188171，37.779399 左上角经纬度   
leftTopLnglat=119.48046,37.14453  

#rightBottomLnglat   119.292297，37.18439 右下角经纬度  
rightBottomLnglat=120.99804,35.57031   
```

>   注意：左上、右下角经纬度由所在地市经纬度确定。可由百度坐标拾取网站获得http://api.map.baidu.com/lbsapi/getpoint/index.html   也可由下载包中的getPos.html页面获取。



配置完成后保存，双击start.bat。开始下载。

## 常见问题：

jdk版本问题，下载1.7jdk进行下载。