---
title: "Customize progress using cssClass"
component: "Progress Button"
description: "Progress Button how to section, change text content and styles, hide spinner, customize progress."
---

# Customize progress using cssClass

You can customize the background filler UI using the [`CssClass`](https://help.syncfusion.com/cr/blazor/Syncfusion.Blazor~Syncfusion.Blazor.SplitButtons.SfProgressButton~CssClass.html) property.

* Adding `e-vertical` to `CssClass` shows vertical progress.
* Adding `e-progress-top` to `CssClass` shows progress at the top.

You can also show reverse progress by adding custom class to the [`CssClass`](https://help.syncfusion.com/cr/blazor/Syncfusion.Blazor~Syncfusion.Blazor.SplitButtons.SfProgressButton~CssClass.html) property.

```csharp
@using Syncfusion.Blazor.SplitButtons

<SfProgressButton EnableProgress="true" CssClass="e-hide-spinner e-vertical" Duration="4000" Content="Vertical Progress"></SfProgressButton>
<SfProgressButton EnableProgress="true" CssClass="e-hide-spinner e-progress-top" Duration="4000" Content="Progress Top"></SfProgressButton>
<SfProgressButton EnableProgress="true" CssClass="e-hide-spinner e-reverse-progress" Duration="4000" Content="Reverse Progress"></SfProgressButton>

<style>
    .e-reverse-progress .e-progress {
        right: 0;
        left: auto;
    }
</style>

```

Output be like

![Progress Button Sample](./../images/pb-vertical.png)