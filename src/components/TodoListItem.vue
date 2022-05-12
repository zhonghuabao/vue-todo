<template>
      <!-- todo 项目，外层容器用于显示背景、圆角边框 -->
            <div class="todo-item">
                <!-- 用 label 包裹后，点击里边任何一个元素都能触发 checkbox 的事件 -->
                <label>
                <input type="checkbox" />
                    Todo 1
                <!-- 自定义的复选按钮 -->
                <span class="check-button"></span>
                </label>
            </div>
          
</template>

<script>
export default {
    name:"TodoListItem",

}
</script>


<style scoped>

/* 添加框 */
.input-add {
  position: relative;
  display: flex;
  align-items: center;
}

.input-add input {
  padding: 16px 52px 16px 18px;
  border-radius: 48px;
  border: none;
  outline: none;
  box-shadow: 0px 0px 24px rgba(0, 0, 0, 0.08);
  width: 100%;
  font-size: 16px;
  color: #626262;
}

.input-add button {
  width: 46px;
  height: 46px;
  border-radius: 50%;
  background: linear-gradient(#c0a5f3, #7f95f7);
  border: none;
  outline: none;
  
  color: white;
  position: absolute;
  right: 0px;

  cursor: pointer;
}

.input-add .plus {
  display: block;
  width: 100%;
  height: 100%;
  background: linear-gradient(#fff, #fff), linear-gradient(#fff, #fff);
  background-size: 50% 2px, 2px 50%;
  background-position: center;
  background-repeat: no-repeat;
}
</style>