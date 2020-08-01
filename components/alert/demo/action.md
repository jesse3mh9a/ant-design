---
order: 13
title:
  zh-CN: 基本
  en-US: Action
---

## zh-CN

额外自定义带有操作事件的元素。

## en-US

Additional defining Handling events with React elements.

```tsx
import { Alert, Button } from 'antd';

ReactDOM.render(
  <>
    <p>测试中, 暂时用例会较多</p>
    <br />
    <Alert
      message="Success Text"
      type="success"
      action={
        <Button size="small" type="text">
          Accept
        </Button>
      }
      closable
    />
    <Alert
      message="Success Text Success Text Success Text Success Text Success Text Success Text"
      type="success"
      action={
        <Button size="small" type="text">
          Accept
        </Button>
      }
      closable
    />
    <Alert
      message="Success Text Success Text Success Text Success Text Success Text Success Text"
      type="success"
      action={
        <Button size="small" type="text">
          Accept
        </Button>
      }
      closable
    />
    <Alert
      message="Success Text"
      type="success"
      action={
        <Button size="small" type="text">
          Undo
        </Button>
      }
    />
    <Alert
      message="Success Text"
      type="success"
      action={
        <Button type="text" size="small">
          Accept
        </Button>
      }
      closable
    />
    <Alert
      message="Success Text"
      type="success"
      showIcon
      description="Detailed description and advices about successful copywriting."
      action={
        <Button type="text" size="small">
          Undo
        </Button>
      }
    />
    <Alert
      message="Success Text"
      type="success"
      showIcon
      description="Detailed description and advices about successful copywriting."
    />
    <Alert
      message="Success Text"
      type="success"
      showIcon
      description="Detailed descript"
      action={
        <Button type="danger" size="small" ghost>
          decline
        </Button>
      }
      closable
    />
    <Alert
      message="Success Text"
      type="success"
      closable
      action={
        <Button type="text" size="small">
          Agree
        </Button>
      }
    />
  </>,
  mountNode,
);
```

<style>
.code-box-demo .ant-alert {
  margin-bottom: 16px;
}
</style>
