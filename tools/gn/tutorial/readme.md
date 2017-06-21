## gn实战

1：在tools/gn/tutorial目录下添加BUILD.gn 文件。

```
executable("hello_world") {
  sources = [
    "hello_world.cc",
  ]
}
```

2: 在相同目录下面需要创建.gn文件，需要指定buildconfig。

```
buildconfig = "//build/BUILDCONFIG.gn"
```

3：build文件下面的文件夹从example拷贝过来，是一些通用的配置操作。

4：生成ninja需要的文件。

```
./gn gen out/test
```

5: 编译

进入out/test目录，执行ninja即可。