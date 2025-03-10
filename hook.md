# Hook函数表

<!-- 
本文档描述了一个用于函数钩子的工具集，提供了多个用于创建和管理函数钩子的API。
这些API允许你在运行时动态修改函数的行为，实现函数拦截、修改和监控等功能。
-->

## 主要函数

### create_hook

<!-- 
创建一个基本的函数钩子

参数说明：
- target_function: 目标函数，要被钩子拦截的原始函数
- hook_function: 钩子函数，将替代原始函数执行的新函数
- context: 可选的上下文数据，会传递给钩子函数

返回值：
- hook对象，包含了钩子的控制接口

使用示例：
const hook = create_hook(originalFunc, (args, context) => {
    console.log('函数被调用');
    return args[0] + 1;
});
-->

### create_dynamic_hook

<!-- 
创建一个动态函数钩子，可以在运行时修改钩子行为

参数说明：
- target_function: 目标函数
- hook_config: 钩子配置对象，包含before和after回调
- options: 可选的配置选项

返回值：
- dynamic_hook对象，提供了更新钩子行为的接口

使用示例：
const dynamicHook = create_dynamic_hook(targetFunc, {
    before: (args) => { console.log('调用前') },
    after: (result) => { console.log('调用后') }
});
-->

### create_detour

<!-- 
创建一个底层的函数detour，直接修改函数的机器码

参数说明：
- target_address: 目标函数的内存地址
- detour_function: 替换函数
- original_bytes: 原始函数的字节码备份

返回值：
- detour对象，包含了恢复原始函数的方法

使用示例：
const detour = create_detour(getFunctionAddress(originalFunc), 
    (registers) => {
        // 修改寄存器状态
        return modified_registers;
    }
);
-->

## 高级功能

<!-- 
除了基本的钩子创建功能外，本工具集还提供了以下高级特性：

1. 钩子链：多个钩子可以串联，形成处理管道
2. 条件钩子：可以设置钩子的触发条件
3. 性能优化：采用内联缓存等技术提升性能
4. 安全保护：防止钩子循环调用和栈溢出
-->

## 注意事项

<!-- 
1. 在多线程环境下使用钩子时需要特别注意线程安全
2. 某些系统函数可能无法被钩子拦截
3. 使用detour时要特别小心，错误的修改可能导致程序崩溃
4. 建议在开发环境中充分测试钩子功能
-->