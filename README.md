DessertClicker
==================================

Solution code for Android Kotlin Fundamentals Codelab 4.1: Lifecycles and logging.

_您将使用一款名为 DessertClicker 的初始应用。在此应用中，每当用户点按屏幕上的甜点时，该应用就会为用户“购买”相应甜点。应用会在布局中更新已购甜点的数量值，以及用户消费的总金额。_

![Example Image](img.png)

Introduction
------------

DessertClicker is a game about making desserts. Press the button, make a dessert,
earn the big bucks.

You use this app in the course to explore the Android lifecycle and log messages to
the Android console (Logcat).

Pre-requisites
--------------

You need to know:
- How to open, build, and run apps with Android Studio.
- What an activity is, and how to create one in your app.
- What the activity's onCreate() method does, and the kind of operations
  that are performed in that method.
- How to create layouts in your activity, and how to update a layout in runtime.


Getting Started
---------------

1. Download and run the app.


import Dependencies
---------------
````
```
定义版本号
ext {
    navigationVersion = "2.3.0"
}
引入依赖'androidx.navigation.safeargs'
dependencies{
    implementation "androidx.navigation:navigation-fragment-ktx:$navigationVersion"
    implementation "androidx.navigation:navigation-ui-ktx:$navigationVersion"
}
运行时报错
Duplicate class androidx.lifecycle.ViewModelLazy found in modules 
lifecycle-viewmodel-2.4.0-runtime (androidx.lifecycle:lifecycle-viewmodel:2.4.0) and
lifecycle-viewmodel-ktx-2.2.0-runtime (androidx.lifecycle:lifecycle-viewmodel-ktx:2.2.0)
```
尝试以下方法来解决问题：

1.执行以下命令获取项目的依赖关系树：`./gradlew app:dependencies`
  -出现了关系树，但我看不明白，尝试删掉相冲突的依赖但仍没有解决问题最后选择放弃

2.检查项目中的其他依赖项，并确保它们与所需的 androidx.lifecycle 版本兼容。
 可以尝试更新这些依赖项的版本，以使用与 androidx.lifecycle:lifecycle-viewmodel:2.4.0 兼容的版本。
  -我将navigationVersion提升到2.5.0就可以运行成功
  


````

# 1.创建界面状态类

# 2.创建ViewModel

# 3.将应用逻辑和数据转移到ViewModel

# 4.调用ViewModel







Readme基本语法和书写格式
---------------

> Text that is a quote

Use `git status` to list all new or modified files that haven't yet been committed.

Some basic Git commands are:
```
git status
git add
git commit
```

The background color is `#ffffff` for light mode and `#000000` for dark mode.

This site was built using [GitHub Pages](https://pages.github.com/).

- George Washington
* John Adams
+ Thomas Jefferson

1. James Madison
2. James Monroe
3. John Quincy Adams

1. First list item
   - First nested list item
     - Second nested list item

- [x] #739
- [ ] https://github.com/octo-org/octo-repo/issues/740
- [ ] Add delight to the experience when all tasks are complete :tada:

@octocat :+1: This PR looks great - it's ready to merge! :shipit:

Here is a simple footnote[^1].

A footnote can also have multiple lines[^2].

[^1]: My reference.
[^2]: To add line breaks within a footnote, prefix new lines with 2 spaces.
  This is a second line.
  
Let's rename \*our-new-project\* to \*our-old-project\*.

| Command | Description |
| --- | --- |
| git status | List all new or modified files |
| git diff | Show file differences that haven't been staged |

| Command | Description |
| --- | --- |
| `git status` | List all *new or modified* files |
| `git diff` | Show file differences that **haven't been** staged |

| Left-aligned | Center-aligned | Right-aligned |
| :---         |     :---:      |          ---: |
| git status   | git status     | git status    |
| git diff     | git diff       | git diff      |

| Name     | Character |
| ---      | ---       |
| Backtick | `         |
| Pipe     | \|        |

<details><summary>CLICK ME</summary>
<p>

# asdasd
#### We can hide anything, even code!

```ruby
   puts "Hello World"
```

</p>
</details>

````
```
Look! You can see my backticks.
```
````

```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```

Here is a simple flow chart:

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```

This sentence uses `$` delimiters to show math inline:  $\sqrt{3x-1}+(1+x)^2$

$$\left( \sum_{k=1}^n a_k b_k \right)^2$$

https://github.com/github/docs/labels/enhancement
