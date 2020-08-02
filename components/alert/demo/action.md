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
import React, { useState } from 'react';
import { Alert, Button, Space } from 'antd';

const CloseInAction = () => {
  const [shouldClose, setShouldClose] = useState(false);

  const handleClose = () => {
    setShouldClose(true);
  };

  return (
    <Alert
      shouldClose={shouldClose}
      message="Close in action"
      description="Add shouldClose for handle close from outside"
      type="info"
      showIcon
      action={
        <Space>
          <Button size="small" type="text">
            Other
          </Button>
          <Button size="small" type="primary" ghost onClick={handleClose}>
            Close
          </Button>
        </Space>
      }
    />
  );
};

ReactDOM.render(
  <>
    <CloseInAction />
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
