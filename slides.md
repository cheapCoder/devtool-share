---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: "text-center"
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
colorSchema: "light"
selectable: true
---

# Devtool 小技巧分享

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="abs-br m-6 flex gap-2">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:edit />
  </button>
</div>

---

# 命令菜单

> Google Developers: You may be familiar with a similar feature in Visual Studio Code called the Command Palette, which was the original inspiration for the Command Menu.

<br/>
<br/>

##### 打开方式:

- `Command+Shift+P`
- 运行命令

<br/>

##### 操作

- 文件/命令
- 截图
- 中文
- 停用 JavaScript
- 清除网站数据
- ...

---

# Console

- `$`和`$$`
- `$_`
- `$0`
- `copy`
  - copy(location)
  - copy($0)
- `getEventListeners($0)`
- `document.designMode='on'` / `document.body.contentEditable = true`
- 异步
  - `await navigator.storage.estimate()`
  <!-- - `monitor`/`monitorEvents` -->
- 实时表达式

---

layout: image-right
image: https://p1-jj.byteimg.com/tos-cn-i-t2oaga2asx/gold-user-assets/2018/12/9/1679379780c11ef3~tplv-t2oaga2asx-zoom-in-crop-mark:1304:0:0:0.awebp

---

# Elements

- `option + click`
- 通过 `h` 来隐藏
- Mutation 断点
- 编辑器特性

---

## layout: center

---

<!-- layout: contain -->
<!-- image: https://p1-jj.byteimg.com/tos-cn-i-t2oaga2asx/gold-user-assets/2018/12/11/1679a0d3a708ef3e~tplv-t2oaga2asx-zoom-in-crop-mark:1304:0:0:0.awebp -->
<!-- --- -->

### console.log 打印对象使用引用

<br/>

  <img width='700' src="https://p1-jj.byteimg.com/tos-cn-i-t2oaga2asx/gold-user-assets/2018/12/11/1679a0d3a708ef3e~tplv-t2oaga2asx-zoom-in-crop-mark:1304:0:0:0.awebp">

---

# Network

- `Replay XHR`
- `copy as fetch`
- `Capture screenshots`
- [过滤接收正则](https://chinese.freecodecamp.org/news/chrome-devtools-network-tab-tricks/)
  - `ctrl + space`
  - `-`

---

# Overrides, Snippets and Changes

> This technique allows the mapping of local javascript or CSS file to files on the production site. This is very useful for debugging production issues.

> Many times the UAT / Production environment has environment-specific data like database, migration scripts, etc so making the local environment with the same data as UAT / Production is not possible. In this case, local overrides become very handy. You can quickly execute any javascript or CSS directly on UAT / Production by mapping local files without the need of deploying the changes.

- Overrides: 覆盖

- Changes: 查看变更

- Snippets: 新加
  - 命令面板`!`查找(无`<`)

---

# 其它

- Sources 的`Event Listener Breakpoints`
- `Coverage`
<!-- - `Animations` -->
- `Show media queries`
- `Performance` 的 Network 和 CPU
- Rendering
  - `Paint flashing`
  - `Web vitals`

---

参考：

- https://developer.chrome.com/docs/devtools/

- https://umaar.com/dev-tips/

- https://juejin.cn/post/7085135692568723492?share_token=4ce3a677-b4e4-4853-ac29-daa493bcab41

- https://javascript.plainenglish.io/super-useful-tips-and-tricks-of-chrome-developer-tools-8b3c27d3ebca

- https://juejin.cn/post/6844903734212821000
