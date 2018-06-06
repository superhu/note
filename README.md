## Welcome to GitHub Pages

用github pages托管前端页面,
用apicloud为后台,搭建免费动态网站,试验中

```javascript
    var now = Date.now();  
    var appKey = sha1("A6067856527384"+"UZ"+"D0588DC0-4FA1-F9E5-7BD7-E97450CC40B7"+"UZ"+now)+"."+now;
    $.ajax({
    "url": "https://d.apicloud.com/mcm/api/comment?filter=%7B%22where%22%3A%7B%7D%2C%22skip%22%3A0%2C%22limit%22%3A20%7D",
    "cache": false,
    "headers": {
        "X-APICloud-AppId": "A6067856527384",
        "X-APICloud-AppKey": appKey
    },
    "type": "GET"
    }).success(function(data, status, header) {
        console.log(data, status, header);
        $('#data').text(JSON.stringify(data));
    }).fail(function(header, status, errorThrown) {
        console.err(errorThrown);
    })
```

### Markdown
[首页](https://superhu.github.io) 

[test](https://superhu.github.io/test.html)
