# jd - 一个单页购物车模仿
一个模仿京东购物车页面的单页angular.JS v1的单页应用</br>
使用的框架是ionic，Angular JS的版本为V1。

<h4>在编写过程中主要遇到的问题</h4>
<p>1、在使用ng-repeat生成list中使用 $index 来获取索引时，编辑状态删除了商品之后，$index获取到的索引不是之前的，对list的所有增删改查都会出错。
参考 http://web.jobbole.com/82470/  将传入的$index 改为了item，就解决了这个问题。</p>
<p>2. 一开始的时候把购物车和下方的推荐列表放在了两个controller里面，导致最后的factory中很多公共数据需要引用，
      不过考虑到这个是单个页面，所以后来还是合并到一个controller，保留factory里面的的公共数组。</p>
