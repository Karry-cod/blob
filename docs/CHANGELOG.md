# Change Log

## [1.0.3] - 2024-5-29

### Refactored

- 修复了一些在 **Accessibility** 上的问题
- 优化了部分内容，速度更快了

## [1.0.4] - 2024-5-30

### Refactored

- 优化了部分内容，评分 **395**
- 修改了 README

## [1.1.0] - 2024-6-2

### Features

- 新增 `ProjectCard`
- 完善了 Project 页面

### Refactored

- 取消了头图的懒加载，删去了莫名其妙的 br

## [1.1.1] - 2024-6-2

### Refactored

- 优化链接样式，在 `pagespeed.web` 获得 400 分

## [1.1.2] - 2024-6-12

### Features

- 新增 `busuanzi` 计数器

## [1.2.0] - 2024-6-16

### Features

- `css` 已经改为 `scss`
- 自定义了 `waline` 的样式
- 完善了 `Footnotes` 的样式
- 添加图标

## [1.2.1] - 2024-6-28

### Features

- 爆改 `scss` 文件，基本上改成了 `Tailwind`
- 修改了 `footer` 的样式

### Refactored

- 微调了部分组件的样式
- 微调了文章样式
- 删去了不必要的友链

## [2.0.0] - 2024-7-8

### Features

- `Lighthouse` 400
- 文本压缩……启动！！
- 页脚修改……返璞归真

### Refactored

- 删除 `busuanzi` 计数器

### Fix

- 修复了文章内标签跳转的问题

## [2.1.0] - 2024-7-9

### Features

- 新增搜索功能

### Refactored

- 微调页脚
- 微调导航栏

## [2.1.1] - 2024-7-9

### Fix

- 修复了不能跳转的问题（原因未知）

## [2.1.2] - 2024-7-10

### Features

- （半成品）添加 `twikoo` 评论
- 一些组件，将在 2.2.0 总结

### Refactored

- 完善了搜索的黑夜模式

## [2.2.0] - 2024-7-13

### Features

- 添加目录功能！（终于加了）
- 添加了一篇指导文章
- 添加了新的组件

### Refactored

- 修改了行距

### Fix

- 修复了在手机屏幕下页脚显示不全的问题

## [2.3.0] - 2024-7-18

### Features

- 添加了代码框的行号
- 提交了如何修改代码框主题的教程

### Refactored

- 修改了 `astro.config.mjs` 现在代码框样式完全了

## [2.3.1] - 2024-7-19

### Fix

- 修复了 `astro.config.mjs` 中的问题（我填错了位置了）
- 完善了白天的代码框样式

## [2.4.0] - 2024-7-21

### Refactored

- 更改了 `<main>` 的位置，现在它只包含 card 而不包含 footer
- 重写了有关**社交链接**、**菜单**、**导航栏**以及**评论**的 `.astro` 文件，现在它们通过 `consts.ts` 来生成其内容
- 把**社交链接**的 svg 与配置文件分离
- 删去了不必要的文件与 `import`

### Fix

- 修复了原 JS 文件中的一堆 error ，现在它们都有了防 null 判断而不会出错
- 指定了 page 与 post 的数据结构，现在不会报 never 错误了
- 修复了若干错误，现在项目可以通过 `npx astro check`

## [2.5.0-alpha] - 2024-7-22

### Features

- 新增返回顶部按钮
- 新增适用于平板的界面样式
- 新增文章、仓库卡片的样式
- 新增导航栏图标，适配平板样式
- 现在你可以通过 `consts.ts` 自定义主题中的辅助文字内容

### Refactored

- 全面重写页面，将原本的元素内滚动改成了通过 grid 搭建的页面，解决了无法平滑跳转、滚动条乱飞的问题。现在整个页面成为一个更紧密结合的整体
- 侧边栏重写，使用 sticky 定位，添加了图标
- 重写文章、仓库卡片的样式，现在文章的标题、简介不再会被隐藏而是会自动适应
- 重写文章、仓库卡片在小屏幕下的样式
- 重写按钮的样式，现在它们被集成到侧边栏中，而不是脱离于主页面
- 重写目录的样式，现在它会自动生成在侧边栏中

### Fix

- 修复了原 tag 文件中变量的命名问题
- 统一了 Astro.props 的格式（使用断言）
- 修复了文章标题、简介过长导致的溢出问题

## [2.5.0-alpha.2] - 2024-7-22

### Features

- 清理了 global.scss
- 为没有标签的文章自动添加了一个不可点击的未分类标签，视觉上更统一
- 为 collapse 与 diff 添加了 m-2 ，现在它们不会突出去了

### Refactored

- 全部改成 Tailwind

### Fix

- 修复了上一页、下一页按钮与页脚黏在一起的问题

## [2.5.0-alpha.3] - 2024-7-23

### Fix

- 修复了手机视图下导航栏消失不见的问题

## [2.5.0-alpha.4] - 2024-7-24

### Fix

- 修复了项目卡片无法获取信息的问题
- 修复了在博客、项目页面下目录跳转的问题

## [2.5.0-alpha.5] - 2024-7-26

### Fix

- 修复了项目卡片中错误的样式类
- 修复了有关于类型的问题，现已通过 check 0.8.2

## [2.5.0-beta] - 2024-7-29

### Features

- 现在行号和顶栏已经与代码分开且被固定
- 新增代码框显示语言的功能

### Refactored

- 重写了代码框的结构（使用 shiki 转换器）

### Fix

- 修复了在手机视图下卡片显得过小的问题

## [2.5.0-beta.2] - 2024-7-29

### Refactored

- 调整了一下代码框顶栏，现在元素垂直居中了
- 调整了在手机视图下卡片的 padding

### Fix

- 修复了文章跳转 target 错误的问题（为什么才发现这个严重问题）

## [2.5.0-beta.3] - 2024-7-30

### Features

- `consts.ts` 添加了标签页的配置，这是主名称
- `BaseLayout.astro` 添加了标签页的配置，现在你可以为每一个页面添加属于它自己的标签页名称

### Refactored

- 断言界定了 JS 中元素的类型，避免 TS 报错
- 调整了一下代码框结构，现在代码右侧与代码框有了一定的留白
- 调整了博客与项目页面的结构，统一 `mt-8` `mb-8`

### Fix

- 修复了昼夜切换按钮实际操作区域与显示区域不一致的问题
- 修复了昼夜切换按钮不同步的问题，现在两个按钮与其实际主题统一

## [2.5.0-rc] - 2024-8-1

### Features

- 常驻了上下页的按钮，这下大家就知道我的博客其实是有做分页的了
- 添加了分页的按钮，终于不用一页一页地跳了

### Refactored

- 单页页面改成了十篇文章
- 去掉了 layout 的 title

## [2.5.0] - 2024-8-2

### Features

- 添加分类功能，现在你可以为你的文章添加两个独立的索引：分类与标签
- 给分类与标签的文章列表页面添加了分页功能，不再是一整页了
- 在侧边栏集成了分类的功能，来自 issue #10

### Refactored

- 现在如果文章没有图片，它的文章信息将会填充
- 修改了分页按钮的样式
- 微调样式，来自 issue #9

### Fix

- 修复在文章过多时分页失效的问题
- 修复在 issue #11 中提到的问题

## [2.5.1] - 2024-8-4

### Features

- 修改了 README
- 添加了 Vercel Web Analytics （不使用 vercel 的用户需要注意一下）

### Refactored

- 改善了整体排版，现在段落之间更清楚了
- 修复了页脚一些奇怪的居中问题
- 更换了 Footnotes 的卡片颜色
- 删除了底部版权信息卡片的阴影
- 添加了表格每一行的分割线
- 把 `<code>` 的字体稍微改大了一点

## [2.5.2] - 2024-8-7

### Features

- 改进了 `TimeLine` 的格式，现在比之前方便多了
- 在侧边栏添加分类与标签卡片，移除原来的分类页面

### Refactored

- 修改了卡片样式
- 修改了链接样式
- 清理了原评论系统中不必要的代码

### Fix

- 修复了部分手机导航栏无法跳转的问题

## [2.5.3] - 2024-8-12

### Features

- 添加了页面跳转的动画

### Fix

- 修复了不规范的导航栏文本
- 修复了在不同主题下跳转页面导致的闪烁问题
- 移除了 `astro:transition` 改成了 `swup` 修复了鼠标指针的闪烁问题

## [2.5.4] - 2024-8-12

### Fix

- 修复了目录没有被正确更新的问题
- 修复了文章搜索框没有正确显示的问题
- 修复了文章里面 Code 的复制按钮丢失的问题

## [2.5.4-hotfix.1] - 2024-8-13

### Fix

- 修复了搜索组件无法正常加载的问题

## [2.5.5] - 2024-8-18

### Features

- 添加了置顶功能，现在你可以给文章 badge 属性 设置为 `Pin` 来置顶你的文章

### Refactored

- 清理了项目代码
- 修改了侧边卡片的样式
- 修改了原 DaisyUI 内建的逻辑，改成点击按钮收回而不是点击外部收回

## [2.5.6] - 2024-8-22

### Features

- 添加了图片放大功能（仅对 BaseCard 中的图片有效）

### Refactored

- 根据用户反馈，回退了手机端导航栏的逻辑
- 修改了在博客页面下标签栏的标题

## [2.5.7] - 2024-9-7

### Features

- 添加了对 robots.txt 的支持
- 为站外链接添加了图标
- 添加字数统计与阅读时间统计

### Refactored

- 修改了 TimeLine 的样式
- 更新了评论系统的样式
- 修改了评论系统的定位 id 防止被覆盖

### Fix

- 修复了评论系统反应表情加载不出来的问题（图床垮了）
- 修复了 `global.scss` 中错误的 applt 拼写

## [2.6.0] - 2024-9-15

### Features

- 新增了导航栏的逻辑，现在点击按钮也可以收回（🚧 此内容可能存在问题，需要收集更多信息 🚧）
- 为每一个标题添加了按钮，您可以将指针放在标题上，点击按钮即可跳转
- 为卡片图片添加了一个跳转样式，鼠标放上后会有一个放大的动画与箭头
- 为链接添加了新的样式，现在它们更生动、更引人注目
- 添加了字数统计与阅读时间计算的功能，您可以在博客中看到它们的统计结果
- 新增分享功能，现在您可以通过文末按钮直接将文章分享到社交媒体上
- 新增 i18n ，移除了老旧的 `infoTest` ，现在所有的语言都在 `public/locales` 文件夹中

    这意味着您可以添加多种语言并随时切换，教程如下：

    1. 在 `public/locales` 文件夹中添加您的语言文件，先添加一个名为语言代码的文件夹，然后在里面添加一个 json 文件，文件名必须为 `translation.json`
    2. 复制已有的 `translation.json` 文件，然后修改其中的内容，比如：

        ```json
        {
        "label": {
          "noTag": "No tags assigned",
          "tagCard": "Tags",
          "tagPage": "Tag - ",
          "noCategory": "No categories assigned",
          "categoryCard": "Categories",
          "categoryPage": "Category - ",
          "link": "Link: ",
          "prevPage": "Recent posts",
          "nextPage": "Older posts",
          "wordCount": "words",
          "readTime": "minutes"
          }
        }
        ```

    3. 在 `astro-i18next.config.mjs` 中添加您的语言代码，比如：

        ```mjs
        export default {
        defaultLocale: "en",
        locales: ['en', 'zh', 'xx'] // 这里添加您的语言代码
        };
        ```
    
    4. 在 'BaseLayout.astro' 中更改为您的语言代码，比如：

        ```astro
        ...
        import i18next, { t, changeLanguage } from "i18next";

        changeLanguage("xx");
        ...
        ```

> [!NOTE]
> 欢迎大家为主题添加语言支持！

### Refactored

- 新增 docs 文件夹
- 修改了 blockquote 的内边距
- 修改标签页标题，坚持内容优先，把 `${SITE_TAB} - ${title}` 改成了 `${title} - ${SITE_TAB}`

### Fix

- 修复了在标题与 alert 中错误的外链 svg 样式
- 修复了 toc 错误获取 # 的问题
- 修复了导航栏逻辑

## [2.6.1] - 2024-9-21

### Features

- 在 `consts.ts` 中新增了 `USER_SITE` ，用来生成网站底部卡片的链接
- 添加了网站加载时的进度条

### Refactored

- 修改了 swup 的配置项

### Fix

- 修复了文章在标签、分类过多时按钮溢出的问题
- 修复了一堆拼写错误（存在于 2.6.0 的 release 中）
- 删除了在 LinkCard 中不恰当的图片放大功能
- 移除了 `transition.scss` ，改用 swup 默认主题代替（我不知道这对改善崩溃问题是否有用）

## [2.7.0] - 2024-10-12

### Features

- 添加昼夜转换过渡
- 自定义了博客中的标题 `ID` ，当前命名格式为 `heading-${headingCount}` ，避免了出现同名标题无法跳转的问题
- 为博客目录功能添加了 "聚焦" 功能，现在目录会根据您当前阅读的部分自动滚动
- 为博客 `main` 中的卡片添加了逐次进入样式，使用 `sass` 制作：

    ```scss
    .fade-in-up {
      opacity: 0;
      transform: translateY(50px);
      animation: fadeInUp 0.5s ease forwards;

      @for $i from 1 through 10 {
        &:nth-child(#{$i}) {
          animation-delay: #{$i * 0.1}s;
        }
      }
    }

    @keyframes fadeInUp {
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }
    ```

### Refactored

- 修改了原网站图标
- 修改了原不规范的文件命名
- 修改了原不合理的布局
- 修改了侧边栏按钮的样式，使用 `join` 组合元素
- 微调 `padding`

### Fix

- 修复了在重名 `ID` 下无法跳转的问题

## [2.7.1] - 2024-10-19

### Refactored

- 有关事件监听的部分更改

### Fix

- 修复了滚动问题
- 修复了在站内跳转时目录中 `active` 保留的问题

## [2.8.0-rc] - 2024-11-3

### Features

- 学习了 Astro 中自定义元素的用法，现在两个交互按钮单独分为 widget 可以重用
- 在 `consts.ts` 新增了 `SITE_LANG` 作为网站的语言配置
- 在 `consts.ts` 新增了 `DAIYSUI_THEME` 作为 DaiysUI 的主题配置，详见 https://daisyui.com/docs/themes/ （此内容需要更多适配）
- 在 `consts.ts` 新增了 `CODE_THEME` 作为 shiki 的主题配置

#### preview

### Refactored

- 侧边栏与导航栏修改
- 移除了不必要的工具
- 修改了 active 样式（选择性）

### Fix

- 修复了控制台报错
- 补上了 `ProjectCard` 缺失的颜色过渡

## [2.8.0] - 2024-11-9

### Features

- 为 Navbar 添加了操作：下滑页面收起，上滑放下
- 重做了代码复制按钮，减少客户端代码，具体样式详见演示

### Refactored

- 整体页面调整（之前一直觉得 “贴屏幕贴得太近了” 这种感觉，现在好很多）包括宽度与字号

### Fix

- 修复了若干问题

## [2.8.1] - 2024-12-5

### Features

- 新增 `sitmap.xml` 代替自动生成的 `sitmap-0.xml`
- 重写 `rss.xml.ts` 完善了格式并在 RSS 中添加了全文内容
- 新增可重用组件 `GithubInfo` 路径:src\widget\GithubInfo.astro
- 新增卡片布局 包括 `Aside` / `Horizontal` / `Vertical`
- 为博客文章内容添加了渐入效果
- 添加了手动开关评论系统的功能

### Refactored

- 组件布局统一并修改
- 重写了博客底部 License 组件的样式
- 清理了全局的 ClassName 以简化代码
- 将 `tag` 路由更名为 `tags`

### Fix

- 可访问性修复:为必要的组件添加了 `aria-label` 以及由 `sr-only` 包裹的文本
- 为代码框中的复制按钮添加了随机的专属的 `id` 与表单链接
- 修复了分页按钮在仅有一页时出现的样式错误
- 修复了在标签与分类页面下不显示字数与阅读时长的问题

### Chore

- 使用 `iconify` 代替了本地存储 svg 的方式