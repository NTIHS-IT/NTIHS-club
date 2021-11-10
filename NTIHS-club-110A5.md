---
tags: 網頁設計社
---

# 網頁設計社 課前預習 DAY5 (110上)

[TOC]

## 講師:
- xiao xigua#8787

## 網頁前端框架 React
:::warning
:loudspeaker: 以下都是會教的東西，那大家也可以先上網查，先預習，這樣對於之後教學時，可以更快的了解講師在講什麼。
:::

# 前端框架
React, Vue, Angular是前端三大框架  
框架主要是簡化開發步驟加快開發速度的一個工具  
那由於我只會React那就教Reactㄅ  
亞州地區較為流行Vue~~但是我偏不要~~  

# 前端三大框架範例

## Vue
```vue
<template>
  <div id="app">
    Hello {{name}}
  </div>
</template>

<script>
export default {
    name: 'app',
    data() {
        return {
            name: "Taylor"
        }
    }
};
</script>

<style>
</style>
```
#### 如果有寫錯可以跟我講我很久沒寫ㄌ


## React

### function component example

```jsx
function App(props) {
    return (
        <div>
            Hello {props.name}
        </div>
    );
}

ReactDOM.render(
  <App name="Taylor" />,
  document.getElementById('hello-example')
);

```

### class component example

```jsx

class App extends React.Component {
  render() {
    return (
      <div>
        Hello {this.props.name}
      </div>
    );
  }
}

ReactDOM.render(
  <App name="Taylor" />,
  document.getElementById('hello-example')
);
```


## Angular

### 我不會也沒碰過所以就沒寫example搂呵呵


# 為什麼要用框架
- 更有邏輯的開發
- 增加開發效率
- 好維護
- 提升效能

## 以下用React 作範例
### React 寫的話
#### Example 1
<iframe src="https://codesandbox.io/embed/great-wilson-fpmzw?fontsize=14&hidenavigation=1&theme=dark"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="great-wilson-fpmzw"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>

#### Example 2
<iframe src="https://codesandbox.io/embed/react-example-qqlis?fontsize=14&hidenavigation=1&theme=dark"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="react-example"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>

### 原生JavaScript寫的話

#### Example 1
<iframe src="https://codesandbox.io/embed/pedantic-voice-tvibq?fontsize=14&hidenavigation=1&theme=dark"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="pedantic-voice-tvibq"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>
   
#### Example 2

<iframe src="https://codesandbox.io/embed/laughing-butterfly-f6okz?fontsize=14&hidenavigation=1&theme=dark"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="laughing-butterfly-f6okz"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>
---

以上範例可以發現使用框架會更直白


# 上課使用editor(編輯器)
[codesandbox](https://codesandbox.io/)