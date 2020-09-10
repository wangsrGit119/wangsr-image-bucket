# wangsr-image-bucket

#### 通过 jsdelivr cdn 来访问
 ###### 在使用GitHub 图床图片的地方将链接换为

 > https://cdn.jsdelivr.net/gh/{user}/{repo}/图片路径
 
 ######  例如：
 > Github中图片的位置(以下地址可能无法访问)
 > https://github.com/wangsrGit119/wangsr-image-bucket/blob/master/img-article/%E7%94%B5%E8%84%91%E5%9B%BE%E7%89%87%E7%B4%A0%E6%9D%902.jpg
 ######  或者
 > https://raw.githubusercontent.com/wangsrGit119/wangsr-image-bucket/master/img- article/%E7%94%B5%E8%84%91%E5%9B%BE%E7%89%87%E7%B4%A0%E6%9D%902.jpg

 ###### 使用jsdelivr访问的URL
 > https://cdn.jsdelivr.net/gh/wangsrGit119/wangsr-image-bucket/img-article/%E7%94%B5%E8%84%91%E5%9B%BE%E7%89%87%E7%B4%A0%E6%9D%902.jpg


----

#### L2Dwidget 使用

##### node 项目
**注意下面jsonPath的路径使用上面成都cdn加速**
```javascript

npm install -S live2d-widget

------------------------------
在需要引入的页面如下：
import {L2Dwidget} from 'live2d-widget'

.....

  created() {
        setTimeout(function () {
            L2Dwidget.init({
                model: {
                    jsonPath: 'https://cdn.jsdelivr.net/gh/wangsrGit119/wangsr-image-bucket/L2Dwidget/live2d-widget-model-haruto/assets/haruto.model.json',
                }
            });
        },1000);
    }

```
#### 普通html
**换不同的模型请根据仓库下不同名称替换即可**

```javascript

<script src="https://cdn.jsdelivr.net/gh/wangsrGit119/wangsr-image-bucket/L2Dwidget/js/L2Dwidget.min.js"></script>
<script>
L2Dwidget.init({
  model: {
    jsonPath: 'https://cdn.jsdelivr.net/gh/wangsrGit119/wangsr-image-bucket/L2Dwidget/live2d-widget-model-haruto/assets/haruto.model.json',
  }
});

</script>
```
