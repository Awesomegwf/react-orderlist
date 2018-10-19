###JSX
###Props和State
props是组件对外的接口，外部组件通过props将数据或方法传给当前组件使用。
state是组件对内的接口，组件内部的接口，用于维护组件内部的状态。
-----------------------
###组件的生命周期
比如：在组件完成挂载的时候，可以调用服务端的接口来获取组件所需要的数据。
1.Mounting阶段
  constructor
  render()
  componentDidMount()
2.Updatig
  render()
  componentDidUpdate()
3.Unmounting
  componentWillUnmount()
------------------------------
###列表和Keys

````
const number = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li key={number.toString()}>{number}</li>
)
````
react底层会基于key属性，当列表项发生变化时，把key作为列表项的唯一标识去判断有没有发生变化，以减少没必要的渲染。
------------------------------
###事件处理
  1.事件名称采用驼峰写法
  2.在组件的构造函数中对事件处理函数进行this指向绑定到当前组件。
  3.箭头函数：内部this指向为当前函数定义的上下文。
-------------------------
###表单
  1.非受控组件
  2.受控组件
