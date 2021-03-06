---
title: "Radio Button How To sections"
component: "Radio Button"
description: "Radio Button how to section, name and value in form submit, customize Radio Button appearance."
---

# Set the disabled state

Radio Button component can be enabled/disabled by giving [`Disabled`](https://help.syncfusion.com/cr/blazor/Syncfusion.Blazor~Syncfusion.Blazor.Buttons.SfRadioButton~Disabled.html) property. To disable Radio Button component,
the `Disabled` property can be set as `true`.

```csharp
@using Syncfusion.Blazor.Buttons

<SfRadioButton Label="Option 1" Name="default" Value="Checked" @bind-Checked="stringChecked"></SfRadioButton><br />
<SfRadioButton Label="Option 2" Name="default" Value="Disable" @bind-Checked="stringChecked"></SfRadioButton><br />
<SfRadioButton Label="Option 3" Name="default" Value="None" @bind-Checked="stringChecked" Disabled="true"  ></SfRadioButton>

@code {
    private string stringChecked = "Checked";
}

```

Output be like

![Radio Button Sample](./../images/rb-disabled.png)