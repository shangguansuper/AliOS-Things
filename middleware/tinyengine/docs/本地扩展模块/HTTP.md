# HTTP 模块说明

__HTTP__

<div class="bi-table">
  <table>
    <colgroup>
      <col width="90px" />
      <col width="90px" />
      <col width="90px" />
    </colgroup>
    <tbody>
      <tr>
        <td rowspan="1" colSpan="1">
          <div data-type="p">API</div>
        </td>
        <td rowspan="1" colSpan="1">
          <div data-type="p">参数说明</div>
        </td>
        <td rowspan="1" colSpan="1">
          <div data-type="p"></div>
        </td>
      </tr>
      <tr>
        <td rowspan="1" colSpan="1">
          <div data-type="p">HTTP.request(url,function(data){});</div>
        </td>
        <td rowspan="1" colSpan="1">
          <div data-type="p">功能：请求http url内容。 ​ 参数：url：url地址。 function：http请求的回调函数，data为http请求返回的数据。 ​ 返回值：0 调用成功 -1调用失败。</div>
        </td>
        <td rowspan="1" colSpan="1">
          <div data-type="p">示例：</div>
          <div data-type="p"></div>
          <div data-type="p">HTTP.request(&quot;http://www.baidu.com&quot;,function(result){</div>
          <div data-type="p">    console.log(&#x27;http requst reulst=:&#x27;+result);</div>
          <div data-type="p">});</div>
        </td>
      </tr>
      <tr>
        <td rowspan="1" colSpan="1">
          <div data-type="p"></div>
        </td>
        <td rowspan="1" colSpan="1">
          <div data-type="p"></div>
        </td>
        <td rowspan="1" colSpan="1">
          <div data-type="p"></div>
        </td>
      </tr>
    </tbody>
  </table>
</div>


__JS运行HTTP模块示例：__

```
WIFI.connect(ssid,passwd,function(state){console.log('wifi state:'+state);
if (state == 'CONNECTED'){
	HTTP.request("http://www.baidu.com",function(result){
		console.log('http requst reulst=:'+result);
	});
}
});

```

运行结果log如下：

```
http requst reulst=:HTTP/1.1 200 OK
Date: Wed, 02 May 2018 02:51:08 GMT
Content-Type: text/html
Content-Length: 14615
Last-Modified: Fri, 20 Apr 2018 02:36:00 GMT
Connection: Close
Vary: Accept-Encoding
Set-Cookie: BAIDUID=5DAC0B6CB376127C9EA3E11453262C2A:FG=1; expires
```

 