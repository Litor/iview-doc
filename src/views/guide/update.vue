<style>
    .doc-update .ivu-timeline .ivu-timeline-item-content{
        top: -14px;
    }
    .doc-update h2{
        margin: 0;
        font-weight: normal;
    }
    .doc-update code{
        margin: 8px 0 10px;
    }
    .doc-update ul{
        padding-left: 22px !important;
    }
    .doc-update-important{
        color: #3399ff;
    }
    .doc-update-loop.ivu-load-loop{
        animation-duration: 3s;
    }
</style>
<template>
    <i-article>
        <h1>更新日志</h1>
        <article class="doc-update">
            <Timeline pending>
                <Timeline-item>
                    <Anchor title="2.0.0-rc.11" h2></Anchor>
                    <p>
                        <code>2017-04-22</code>
                    </p>
                    <ul>
                        <li>修复 Cascader 在 disabled 模式下扔能使用 clearable 功能的bug。<issue id="635"></issue></li>
                        <li>修复 Message 的 destroy 方法无法使用的bug。<mention id="lcx960324"></mention></li>
                        <li>修复 BreadcrumbItem 动态添加时，无法显示分隔符的bug。<mention id="Becavalier"></mention></li>
                        <li>修复 Menu 的 active-name 为 0 时无法正确匹配的bug。</li>
                        <li>修复 Slider 在 range 模式下，主动设置 value 时显示错误的bug。<issue id="724"></issue></li>
                        <li>修复 Select 在单选可搜索模式下，数字 0 默认不会被选中的问题。<issue id="718"></issue></li>
                        <li>修复 Select 在单选可搜索模式下，第一次展开选项显示不全的bug。<issue id="712"></issue></li>
                        <li>Table 新增远程过滤。<mention id="hezhiying"></mention> <issue id="714"></issue></li>
                        <li>Step 新增 slot。<mention id="purocean"></mention></li>
                    </ul>
                </Timeline-item>
                <Timeline-item>
                    <Anchor title="2.0.0-rc.10" h2></Anchor>
                    <p>
                        <code>2017-04-10</code>
                    </p>
                    <ul>
                        <li>Modal 的 DOM 移动到了 body。<issue id="583"></issue> <issue id="380"></issue></li>
                        <li>Select 新增 <code>on-query-change</code> 事件。</li>
                        <li>Cascader 新增 <code>on-visible-change</code> 事件。<issue id="593"></issue></li>
                        <li>修复 Date 在 Table 内使用时，样式错误的问题。<issue id="577"></issue></li>
                        <li>修复 Table 的 slot 无法使用的bug。<issue id="549"></issue></li>
                        <li>修复 Table 在 Modal 和 Tabs 内使用时，宽度计算不正确的bug。<issue id="591"></issue></li>
                        <li>修复 Tree 组件没有正确引入 Icon 组件的bug。<issue id="612"></issue></li>
                        <li>优化 Slider 在靠近边缘时，卡顿的问题。<issue id="461"></issue></li>
                        <li>优化 Select 在搜索模式下的交互体验。<issue id="566"></issue></li>
                        <li>新增西班牙语。<mention id="MatiasVerdier"></mention></li>
                    </ul>
                </Timeline-item>
                <Timeline-item>
                    <Anchor title="2.0.0-rc.9" h2></Anchor>
                    <p>
                        <code>2017-04-01</code>
                    </p>
                    <ul>
                        <li>Table 单元格的 render 方法，支持 <code v-pre>{{ row }}</code>、<code v-pre>{{ column }}</code> 用法。<issue id="438"></issue></li>
                        <li>Select 支持 IE。</li>
                        <li>BreadcrumbItem 新增 prop <code>replace</code> ，并支持 vue-router 的 push 和 replae 两种跳转。</li>
                        <li>Modal 新增 prop <code>transition-names</code>，支持自定义动画。<issue id="505"></issue></li>
                        <li>优化 DatePicker 在某些时候无法关闭弹窗的问题。</li>
                        <li>修复部分组件结合 vue-i18n 使用时，无法翻译的bug。</li>
                        <li>修复动态使用 Col 时，gutter 无法更新的bug。<issue id="540"></issue></li>
                        <li>修复 Cascader 修改 <code>data</code> 后，不能更新选中项的bug。<issue id="553"></issue></li>
                        <li>修复 Transfer 修改 <code>data</code> 后，不能更新内容的bug。<issue id="555"></issue></li>
                        <li>Input 组件：</li>
                        <ul>
                            <li>修复使用 slot 时，icon 不显示的bug。<issue id="554"></issue></li>
                            <li>优化默认情况下有右间距的问题。</li>
                            <li>优化使用 slot 时，不是圆角的问题。<issue id="397"></issue></li>
                        </ul>
                        <li>新增土耳其语。<mention id="ndrshn"></mention></li>
                    </ul>
                </Timeline-item>
                <Timeline-item>
                    <Anchor title="2.0.0-rc.8" h2></Anchor>
                    <p>
                        <code>2017-03-29</code>
                    </p>
                    <ul>
                        <li>修复 <code>Form</code> 无法对 <code>Cascader</code> 组件及时验证的bug。<issue id="525"></issue></li>
                        <li>修复 <code>Select</code> 在单选可搜索模式下，从外部清空数据时，视图没有更新的bug。<issue id="518"></issue></li>
                        <li>优化 <code>Date</code> 类型组件，点击小图标也可以显示选择器。<issue id="528"></issue></li>
                    </ul>
                </Timeline-item>
                <Timeline-item>
                    <Anchor title="2.0.0-rc.7" h2></Anchor>
                    <p>
                        <code>2017-03-27</code>
                    </p>
                    <ul>
                        <li>重构 <code>Tree</code> 组件。<issue id="468"></issue></li>
                        <li>修复 <code>Cascader</code> 数据置为空时，视图并没有更新的bug。<issue id="488"></issue></li>
                        <li>修复 <code>Form</code> 无法对 <code>Date</code> 类型的组件及时验证的bug。<issue id="494"></issue></li>
                        <li>优化 <code>Radio</code> 组合使用时，无法识别 label 为 0 的情况。<issue id="425"></issue></li>
                        <li><code>Tabs</code> 新增附加内容 slot <code>extra</code>。</li>
                    </ul>
                </Timeline-item>
                <Timeline-item>
                    <Anchor title="2.0.0-rc.6" h2></Anchor>
                    <p>
                        <code>2017-03-22</code>
                    </p>
                    <ul>
                        <li>Table 的上下文 prop：content 更名为 <code>context</code>。</li>
                        <li>修复 Table 在生产环境时，自定义单元格渲染上下文失效的bug。<issue id="454"></issue></li>
                        <li>iCol 增加名称 <code>Col</code>。</li>
                        <li>iForm 增加名称 <code>Form</code>。</li>
                        <li>修复 Input 使用 number 模式时，不能正确返回数字类型的bug。</li>
                        <li>Card 增加内部间距 prop：padding。<mention id="muei"></mention></li>
                        <li>Tag 增加 prop：name。</li>
                    </ul>
                </Timeline-item>
                <Timeline-item>
                    <Anchor title="2.0.0-rc.5" h2></Anchor>
                    <p>
                        <code>2017-03-15</code>
                    </p>
                    <ul>
                        <li>Table 的 自定义单元格支持 data、methods。</li>
                        <li>修复 Table 内通过点击操作删除一行数据时，报错的问题。</li>
                        <li>Button 增加自定义事件 @click，可以不用通过 @click.native 来使用了。</li>
                        <li>修复 Modal 不能自定义 header 的 bug。<issue id="407" /></li>
                        <li>优化 RadioGroup、CheckboxGroup、Menu，可以与其它组件进行嵌套使用。</li>
                        <li>修复 Transfer 在没有使用 slot 时报错的 bug。</li>
                        <li>优化 Form 在验证带有搜索功能的 Transfer 组件时，搜索框样式显示错误的问题。</li>
                    </ul>
                </Timeline-item>
                <Timeline-item>
                    <Anchor title="2.0.0-rc.4" h2></Anchor>
                    <p>
                        <code>2017-03-14</code>
                    </p>
                    <ul>
                        <li>修复警告。</li>
                        <li>修复 Table 筛选下拉菜单不关闭的 bug。</li>
                        <li>修复含有 Input 的组件在 Form 内使用时，on-form-change 事件触发错误的逻辑。</li>
                        <li>优化 Select 广播事件重复的问题。</li>
                    </ul>
                </Timeline-item>
                <Timeline-item>
                    <Anchor title="2.0.0-rc.3" h2></Anchor>
                    <p>
                        <code>2017-03-13</code>
                    </p>
                    <ul>
                        <li>修复部分组件在非 template 内书写时不被识别的问题。部分组件新增别名，并兼任1.0版别名。
                            详见 <a href="https://github.com/iview/iview/blob/2.0/src/index.js#L49" target="_blank">https://github.com/iview/iview/blob/2.0/src/index.js#L49</a></li>
                    </ul>
                </Timeline-item>
                <Timeline-item color="green">
                    <Icon type="trophy" size="18" slot="dot"></Icon>
                    <Anchor title="2.0.0-rc.2" h2></Anchor>
                    <p>
                        <code>2017-03-10</code>
                    </p>
                    <ul>
                        <li>Button 支持组件名 <code>Button</code>，兼容 <code>iButton</code>。</li>
                        <li>Input 支持组件名 <code>Input</code>，兼容 <code>iInput</code>，支持 v-model。</li>
                        <li>RadioGroup 支持 v-model。</li>
                        <li>Radio value 改为了 label，使用 v-model，废弃 checked。</li>
                        <li>Checkbox 支持 v-model。</li>
                        <li>CheckboxGroup value 改为了 label，使用 v-model，废弃 checked。</li>
                        <li>Switch 更名为 <code>iSwitch</code>，废弃checked， 改为了 value，使用 v-model。</li>
                        <li>Badge class 改为了 className。</li>
                        <li>InputNumber 使用 v-model。</li>
                        <li>Progress 支持组件名 <code>iProgress</code>，兼容 <code>Progress</code>，新增 on-status-change 事件。</li>
                        <li>Upload 父级不能通过 computed 获取 Upload 的 fileList 了。</li>
                        <li>Collapse 废弃 activeKey，使用 v-model，key 更名为 name。</li>
                        <li>Carousel 废弃 activeIndex，使用 v-model。</li>
                        <li>Circle 更名为 <code>iCircle</code>。</li>
                        <li>Tabs 废弃 activeKey，改用 value，使用 v-model，key 更名为 name。</li>
                        <li>DropdownItem key 改为 name, Dropdown 的 visible 要使用 @on-visible-change 捕获，不再 sync</li>
                        <li>Menu 支持组件名 <code>iMenu</code>，兼容 <code>Menu</code>，MenuItem 和 Submenu 的 key 改为了 name，Menu 的 activeKey 改为 activeName,openKeys 改为 openNames。</li>
                        <li>Select 支持组件名 <code>Select</code>，兼容 <code>iSelect</code>，model 改为 value，支持 v-model。</li>
                        <li>Page class 改为 className。</li>
                        <li>DatePicker 使用 v-model。</li>
                        <li>Modal visible 改为 value，使用 v-model，style 改为 styles。</li>
                        <li>Table 支持组件名 <code>Table</code>，兼容 <code>iTable</code>。</li>
                    </ul>
                </Timeline-item>
                <Timeline-item>
                    <Button type="ghost" size="large" @click="handleBefore">查看 1.x 版本的日志</Button>
                </Timeline-item>
            </Timeline>
        </article>
    </i-article>
</template>
<script>
    import iArticle from '../../components/article.vue';
    import iCode from 'iCode';
    import Code from '../../code/guide';
    import Anchor from '../../components/anchor.vue';
    import issue from '../../components/issue.vue';
    import mention from '../../components/mention.vue';

    import version from '../../config/config';

    export default {
        components: {
            iArticle,
            iCode,
            Anchor,
            issue,
            mention
        },
        data () {
            return {
                code: Code
            }
        },
        mounted () {
            window.localStorage.setItem('version', version.version);
        },
        methods: {
            handleBefore () {
                window.open('http://v1.iviewui.com/docs/guide/update');
            }
        }
    }
</script>