---
title: "Right-To-Left"
component: "Button"
description: "Button how to section, block button, repeat button, tooltip for Button, customization of button appearance, input and anchor elements."
---

# Right-To-Left

Button component has RTL support. This can be achieved by setting [`EnableRtl`](https://help.syncfusion.com/cr/blazor/Syncfusion.Blazor~Syncfusion.Blazor.Buttons.SfButton~EnableRtl.html) as true.

The following example illustrates how to enable right-to-left support in Button component.

```csharp
@using Syncfusion.Blazor.Buttons

<SfButton IconCss="e-icons e-setting-icon" EnableRtl="true">Settings</SfButton>

<style>
    .e-setting-icon::before {
        content: '\e679';
    }
</style>
```

Output be like

![Button Sample](./../images/button-rtl.png)