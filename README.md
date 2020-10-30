# TrainCenterManageSys_Front 交互规范

## 目录规范

分为PC端和Mobile端

页面交互请在相应文件夹中的 `js/page_js`中完成，

`.js`文件名称应和`.html`文件名称一致

## 注释规范

```js
/**
 * 方法作用 测试接口
 * 请求接口 api/test/test
 * @author liangjianhua <github.com/Varsion>
 */
```

## 请求 Url 规范

每个js顶部定义 全局变量 公共路径

```js
var SERVER_PATH = 'http://bread.varsion.cn/'

        $.ajax({
            type : "POST",
            cache:false,
            //contentType: "application/json;charset=UTF-8",
            url : SERVER_PATH+"api/test/test",
            data : {token:userToken},
            dataType:'json',
            success : function(result) {
            },
            error : function(e){
            }
        });


				$.get(SERVER_PATH+"api/test/test",function() {
          
        })
```

## 关于 code

