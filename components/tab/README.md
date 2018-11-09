<h1>tab</h1>
<section>
  <h2>properties</h2>
  <ul>
    <li>
      <dl>
        <dt>length</dt>
        <dd>type: Number</dd>
        <dd>value:0</dd>
        <dd>控制tab组件的标签数</dd>
      </dl>
    </li>
    <li>
      <dl>
        <dt>items</dt>
        <dd>type:Array</dd>
        <dd>value:[]</dd>
        <dd>定义tab组件的标签栏内容</dd>
      </dl>
    </li>
    <li>
      <dl>
        <dt>item-key</dt>
        <dd>type: String</dd>
        <dd>value:'name'</dd>
        <dd>定义标签内容对应的key</dd>
      </dl>
    </li>
    <li>
      <dl>
        <dt>current-page-index</dt>
        <dd>type:Number</dd>
        <dd>value:0</dd>
        <dd>当前显示的标签栏</dd>
      </dl>
    </li>
    <li>
      <dl>
        <dt>css</dt>
        <dd>type:String</dd>
        <dd>value:''</dd>
        <dd>定义tab的样式</dd>
      </dl>
    </li>
    <li>
      <dl>
        <dt>position</dt>
        <dd>type:String</dd>
        <dd>value:'top'</dd>
        <dd>定义tab的标签栏的位置</dd>
      </dl>
    </li>
  </ul>
</section>
<section>
  <h2>events</h2>
  <ul>
    <li>
      <dl>
        <dt>tab</dt>
        <dd>当切换标签时，会触发tab事件</dd>
      </dl>
    </li>
  </ul>
</section>
<section>
  <h2>slot</h2>
  <ul>
    <li>
      <dl>
        <dt>tab-nav-{{index}}</dt>
        <dd>其中index代表对应的标签序号，比如有第一个标签栏对应tab-nav-0,以此类推</dd>
      </dl>
    <li>
    <li>
      <dl>
        <dt>tab-{{index}}</dt>
        <dd>其中index代表对应的标签内容序号，比如有第一个标签内容栏对应tab-0,以此类推</dd>
      </dl>
    <li>
  </ul>
</section>
<section>
  <h2>example</h2>
  <pre>
    &lt;model-tab 
    length="{{2}}" 
    current-page-index="{{0}}" 
    position="bottom"
    bindtab="tab"&gt;
      &lt;view slot="tab-nav-0"&gt;标签内容1&lt;/view&gt;
      &lt;view slot="tab-nav-1"&gt;标签内容2&lt;/view&gt;
      &lt;view slot="tab-0"&gt;标签内容1&lt;/view&gt;
      &lt;view slot="tab-1"&gt;标签内容2&lt;/view&gt;
    &lt;/model-tab&gt;
  </pre>
</section>