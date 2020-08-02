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
    <Alert
      message="Success Tips"
      description="Detailed description and advice about successful copywriting."
      type="success"
      action={
        <Button size="small" type="text">
          Accept
        </Button>
      }
      closable
    />

    <Alert
      message="Success Tips"
      description="Detailed description and advice about successful copywriting."
      type="success"
      showIcon
      action={
        <Button size="small" type="text">
          Accept
        </Button>
      }
      closable
    />

    <Alert
      message="Success Tips"
      type="success"
      showIcon
      action={
        <Button size="small" type="text">
          Accept
        </Button>
      }
      closable
    />

    <Alert
      message="Success Tips"
      type="success"
      action={
        <Button size="small" type="text">
          Accept
        </Button>
      }
      closable
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
