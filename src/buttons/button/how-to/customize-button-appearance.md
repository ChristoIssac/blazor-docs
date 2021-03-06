---
title: "Customize Button Appearance"
component: "Button"
description: "Button how to section, block button, repeat button, tooltip for Button, customization of button appearance, input and anchor elements."
---

# Customize Button Appearance

You can customize the appearance of the Button by using the Cascading Style Sheets (CSS). Define the CSS according to your requirement, and assign the class name to the [`CssClass`](https://help.syncfusion.com/cr/blazor/Syncfusion.Blazor~Syncfusion.Blazor.Buttons.Syncfusion.Blazor~CssClass.html)
property. In the following code snippet the background color, text color, height, width, and sharp corner of the Button can be customized through the `e-custom` class for all states (hover, focus, and active).

```csharp

@using Syncfusion.Blazor.Buttons

<SfButton CssClass="e-custom">CUSTOM</SfButton>

<style>
    .e-custom {
        border-radius: 0;
        height: 30px;
        width: 80px;
    }

    .e-custom, .e-custom:hover, .e-custom:focus, .e-custom:active {
        background-color: #ff6e40;
        color: #fff;
    }
</style>

```

Output be like

![Button Sample](./../images/button-custom.png)