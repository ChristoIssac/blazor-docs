---
title: "Autocomplete Grouping"
component: "AutoComplete"
description: "This section for Syncfusion ASP.NET autocomplete control demonstrates the grouping with individual header and it's header customization."
---

# Grouping

The AutoComplete supports wrapping nested elements into a group based on different categories. The
category of each list item can be mapped through the
[GroupBy](https://help.syncfusion.com/cr/blazor/Syncfusion.Blazor~Syncfusion.Blazor.DropDowns.AutoCompleteFieldSettings~GroupBy.html) field in the data table. The group
header is displayed as both inline and fixed headers. The fixed group header content
is updated dynamically on scrolling the suggestion list with its category value.

In the following sample, vegetables are grouped according on its category using `GroupBy` field.

```csharp
@using Syncfusion.Blazor.DropDowns

<SfAutoComplete TValue="string" TItem="Vegetables" Placeholder="e.g. Select a vegetable" DataSource="@LocalData">
    <AutoCompleteFieldSettings  GroupBy="Category" Value="Vegetable"></AutoCompleteFieldSettings>
</SfAutoComplete>

@code {

   public IEnumerable<Vegetables> LocalData { get; set; } = new Vegetables().VegetablesList();

    public class Vegetables
    {
        public string Vegetable { get; set; }
        public string Category { get; set; }
        public string ID { get; set; }

        public List<Vegetables>VegetablesList() {
            List<Vegetables>Veg = new List<Vegetables>();
            Veg.Add(new Vegetables { Vegetable = "Cabbage", Category= "Leafy and Salad", ID= "item1" });
            Veg.Add(new Vegetables { Vegetable = "Chickpea", Category= "Beans", ID= "item2" });
            Veg.Add(new Vegetables { Vegetable = "Garlic", Category= "Bulb and Stem", ID= "item3" });
            Veg.Add(new Vegetables { Vegetable = "Green bean", Category= "Beans", ID= "item4" });
            Veg.Add(new Vegetables { Vegetable = "Horse gram", Category= "Beans", ID= "item5" });
            Veg.Add(new Vegetables { Vegetable = "Nopal", Category= "Bulb and Stem", ID= "item6" });
            Veg.Add(new Vegetables { Vegetable = "Onion", Category= "Bulb and Stem", ID= "item7" });
            Veg.Add(new Vegetables { Vegetable = "Pumpkins", Category= "Leafy and Salad", ID= "item8" });
            Veg.Add(new Vegetables { Vegetable = "Spinach", Category= "Leafy and Salad", ID= "item9" });
            Veg.Add(new Vegetables { Vegetable = "Wheat grass", Category= "Leafy and Salad", ID= "item10" });
            Veg.Add(new Vegetables { Vegetable = "Yarrow", Category = "Leafy and Salad", ID = "item11" });
            return Veg;
        }
    }
}
```

The output will be as follows.

![AutoComplete](./images/grouping.png)
