# cookie-plus

# 1. 作用

提供浏览器中 cookie 操作的 api, 让开发者能更方便的操作 cookie

# 2. 下载

## npm

```ssh
$ npm i --save cookie-plus
```

## yarn

```ssh
$ yarn add --save cookie-plus
```

# api

## getItem(sKey)

### 描述 获取 sKey 对应的值

### 参数

- sKey: cookie 的 key

## setItem(sKey, sValue, vEnd, sPath, sDomain, bSecure)

### 描述 设置/更新一条 cookie

### 参数

- sKey : cookie 的 key
- sValue : cookie 的 值
- vEnd : cookie 的失效时间
- sPath : path (例如 '/', '/mydir') 如果没有定义，默认为当前文档位置的路径。
- sDomain : cookie 生效的域名 (例如 'example.com'， 'subdomain.example.com') 如果没有定义，默认为当前文档位置的路径的域名部分。与早期规范相反的是，在域名前面加 . 符将会被忽视，因为浏览器也许会拒绝设置这样的 cookie。如果指定了一个域，那么子域也包含在内。
- bSecure :secure (cookie 只通过 https 协议传输), 非必填

## hasItem（sKey）

### 描述 判断是否有对应 key 的 cookie

### sKey: key

## removeItem((sKey, sPath, sDomain)

### 描述 删除一条 cookie

### 参数 见 setItem

## keys()

### 描述 获取所有的 cookie 的键

### 参数 无
