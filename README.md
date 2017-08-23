##pca

```
<select id="province"></select>
<select id="city"></select>
<select id="area"></select>
<script type="text/javascript" src="https://cdn.bootcss.com/jquery/3.2.1/jquery.min.js"></script>
<script type="text/javascript" src="pca.js"></script>
<script type="text/javascript">
PCA.init($("#province"),$("#city"),$("#area"));
</script>
```


##layui-pca

```
<div class="layui-form-item">
    <div class="layui-row layui-col-space10">
        <div class="layui-col-xs4 layui-col-sm4 layui-col-md4">
            <select name="province" id="province"  lay-filter="province" >
                <option value="a">选择省</option>
            </select>
        </div>
        <div class="layui-col-xs4 layui-col-sm4 layui-col-md4">
            <select name="city" id="city" lay-filter="city">
                <option value="a">选择市</option>
            </select>
        </div>

        <div class="layui-col-xs4 layui-col-sm4 layui-col-md4">
            <select name="area" id="area" lay-filter="area">
                <option value="a">选择区</option>
            </select>
        </div>
    </div>
</div>

<script>
layui.use(['jquery','form','pca'], function() {
    var $ = jquery = layui.jquery
    ,form = layui.form;
    var pca = layui.pca;
});
</script>
```