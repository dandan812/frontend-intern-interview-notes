横向居中（text-align）
<div style="width: 200px; border: 1px solid #000; 
text-align: center;">
  <span>我是居中的文字</span>
</div>


text-align: center; 只对 行内元素或 inline-block 元素生效
面试点：span 是行内元素 → 可以直接用 text-align


<div style="width: 200px; height: 100px; display: flex; justify-content: center; align-items: center; border: 1px solid #000;">
  <span>居中显示</span>
</div>

display: flex → 开启弹性布局
justify-content: center → 水平居中  主轴
align-items: center → 垂直居中  交叉轴


// 创建1--100的数组
const arr = [];
for (let i = 1;i<=100;i++){
    arr.push(i);
}
console.log(arr);


网格布局
place-items: center; 
