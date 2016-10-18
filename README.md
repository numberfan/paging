# paging  分页
## 使用说明
###1.引入文件
````
  <script src="http://cdn.bootcss.com/jquery/3.1.0/jquery.min.js"></script>
  <script type="text/javascript" src="js/base.js"></script>
````
###2.使用
````
$('.pager').paging(1, 6, {
    first: "首", //设置false则不显示，默认为false
    last: "末", //设置false则不显示，默认为false  
    prev: "上一页", //设置为false,则不显示，默认为“上一页”
    next: "下一页", //设置为false,则不显示，默认为“下一页”
    numOrignClass: ".num", //分页样式
    numHoverClass: ".num-active", //分页激活样式
    firstClass: ".first", //“首页”按钮样式
    lastClass: ".last", //“尾页”按钮样式
    prevClass: ".prev", //“上一页”按钮样式
    nextClass: ".next", //“下一页”按钮样式
    callback: function(nowNum, allNum) {
      console.log(nowNum, allNum)
    }
});
````
