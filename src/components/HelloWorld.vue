<script setup>
</script>

<template>
  <div class="login">
    <div class="loginBox">
      <div class="title">管理系统</div>
      <div class="container">
         <!-- 注册部分 -->
         <div class="container-from container-signup " style="display: none;">
            <form action="#" class="form" id="from1">
                <h2 class="form-title">注册账号</h2>
                <input type="text" placeholder="请输入账号" class="input" />
                <input type="email" placeholder="请输入密码" class="input" />
                <input type="password" placeholder="Password" class="input"/>
                <button type="button" class="btn">点击注册</button>
            </form>
        </div>
        <!-- 登录 -->
        <div class="container-from container-signin">
            <form action="#" class="form" id="from2">
                <h2 class="form-title">欢迎登录</h2>  
                
                <input type="email" placeholder="请输入账号" class="input" />
                <input type="password" placeholder="请输入密码" class="input"/>
                <div>
                  <a href="#" class="link rememberMe">记住我</a>
                  <a href="#" class="link forget">忘记密码</a>
                </div>
                <button type="button" class="btn">登录</button>
            </form>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container button {
  font-size: 1.4rem;
}
.loginBox {
  background-color: #ffffff;
  width: 380px;
  height: 600px;
  border-radius: 40px;
}

.loginBox .title {
  color: #646cff;
  font-size: 30px;
  padding: 20px 20px;
}

.form-title {
            /* 标题界面 */
            font-weight: 300;
            margin: 0;
            margin-bottom: 2rem;
        }
        .link {
            /* 忘记密码部分 */
            color: #333;
            font-size: 0.9rem;
            margin: 1.5rem 0;
            margin-bottom: 2px;
            /* 用于去除文本的装饰效果 */
            text-decoration: none;
        }
        .input {
            /* 对整体文本框的一个优化 */
            width: 70%;
            background-color: #fff;
            padding: 0.9rem 0.9rem;
            margin: 0.5rem 0;
            border:1px solid #c6c6c6;
            outline: none;
            border-radius: 6px;
        }
        .btn {
            /* 对整个按钮的样式美化 */
            background-color: #646cff;/*背景颜色，阴影，弧度，文字颜色，鼠标样式，文字样式*/
            box-shadow: 0 4px 4px #4d52c1;
            border-radius: 6px;
            color: #e7e7e7;
            cursor: pointer;
            font-size: 0.8rem;
            font-weight: bold;
            /* 属性设置字符间的间距为 0.1rem。这意味着文本中的字符将会相对于默认的间距稍微拉宽或缩小 */
            letter-spacing: 0.1rem;
            padding: 0.9rem 4rem;
            /* 关于缓动函数，ease-in 是其中一种，它在动画开始时具有较慢的加速度，逐渐加快。除了 ease-in，还有很多其他的缓动函数可供选择，如 ease-out（慢慢变慢）、ease-in-out（加速再减速）等。 */
            /* transition 属性指定了过渡效果的属性、持续时间和缓动函数。具体来说，transform 是过渡效果应用到的 CSS 属性，80ms 是过渡效果的持续时间，ease-in 是过渡效果的缓动函数。 */
            transition: transform 80ms ease-in;
        }
        .form>.btn {
            margin-top: 1.5rem;
        }
        /* btn被点击的时候，进行缩放动画 */
        .btn:active {
            transform: scale(0.8);
        }
        .forget,
        .rememberMe {
          display: flex;
        }
        .forget {
          justify-content:flex-end;
        }
        
</style>

