
我们已经了解了许多关于 Webpack 的知识，但要完全熟练掌握它并非易事。一个很好的学习方法是通过实际项目练习。当我们对 Webpack 的配置有了足够的理解后，就可以尝试重构一些项目。本次我选择了一个[纯HTML/JS的PC项目](https://github.com)进行重构，项目位于 GitHub 上，非常感谢该项目的贡献者。


重构案例选择了两个页面：首页 index.html 和购物车页面 cart.html。


![](https://img2024.cnblogs.com/blog/1408181/202410/1408181-20241010221719751-1249748259.png)


项目目录结构清晰，根目录包含了各个 HTML 页面，同一层级下还有 CSS、JS 和 IMG 文件夹。每个 HTML 页面对应各自的 CSS 和业务 JS 文件。


![](https://img2024.cnblogs.com/blog/1408181/202410/1408181-20241010221728758-1590367133.png)


### 初始化 npm 项目


首先，创建一个新的空文件夹，并在其中运行 `npm init -y` 命令来初始化项目。接着，在项目根目录下创建 src 文件夹，将 `index.html` 文件复制到 src 目录下，以此为基础进行重构。打开 `index.html` 文件，可以看到页面中引入了 CSS、图片和 JS 资源。然后将 CSS、IMG 和 JS 文件夹也移至 src 目录下。


![](https://img2024.cnblogs.com/blog/1408181/202410/1408181-20241010221740459-2038660054.png)


随后，我们观察 `index.html` 文件中的  和 

