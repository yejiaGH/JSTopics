# 深入浅出Redux源码
## React的优点
### 01 高效的根据数据变化自动更新View
### 02 完善的View模块化机制
### 03 完整的同构体系

## React的缺点

### 数据单向流动，只能父->子，而不能从子->父，
### 广泛流行的双向数据流，无法预测谁更新的数据

## 01 Redux是什么
### action: 对象，reducer: 函数，store: 对象（数据的管理中心，相当于数据库）
### store的好处：数据发生变化可预测；业务逻辑集中在一起，避免分散，降低维护成本

## 02 Redux组成源码剖析
### store是全局唯一的对象，对象里有数据。
### reducer是函数们可以一个或多个，建议多个
### 中间件 在处理具体的reducer之前要用的一些函数。
## 03 React与Redux结合
### 01 不破坏React单向数据流
### 02 store的数据变化与Component界面关联
Provider 解决获取store的问题
Connect Store的更新通知到View的更新
