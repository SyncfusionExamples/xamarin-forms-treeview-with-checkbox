# How to use checkbox in treeview?
This example illustrates how to use checkbox in treeview.

## Sample

### XAML
```xaml
<ContentPage.Content>
    <syncfusion:SfTreeView CheckBoxMode="Recursive">
        <syncfusion:SfTreeView.Nodes>
            <treeviewengine:TreeViewNode Content="Australia" IsChecked="True" IsExpanded="True">
                <treeviewengine:TreeViewNode.ChildNodes>
                    <treeviewengine:TreeViewNode x:Name="newSouthWales" Content="New South Wales">
                        <treeviewengine:TreeViewNode.ChildNodes>
                            <treeviewengine:TreeViewNode Content="Sydney"/>
                            <treeviewengine:TreeViewNode Content="New York">
                                <treeviewengine:TreeViewNode.ChildNodes>
                                    <treeviewengine:TreeViewNode Content="San Francisco"/>
                                </treeviewengine:TreeViewNode.ChildNodes>
                            </treeviewengine:TreeViewNode>
                        </treeviewengine:TreeViewNode.ChildNodes>
                    </treeviewengine:TreeViewNode>
                    <treeviewengine:TreeViewNode Content="United States of America">
                        <treeviewengine:TreeViewNode.ChildNodes>
                            <treeviewengine:TreeViewNode Content="New York">
                                <treeviewengine:TreeViewNode.ChildNodes>
                                    <treeviewengine:TreeViewNode Content="San Francisco"/>
                                </treeviewengine:TreeViewNode.ChildNodes>
                            </treeviewengine:TreeViewNode>
                            <treeviewengine:TreeViewNode Content="California">
                                <treeviewengine:TreeViewNode.ChildNodes>
                                    <treeviewengine:TreeViewNode Content="San Francisco"/>
                                </treeviewengine:TreeViewNode.ChildNodes>
                            </treeviewengine:TreeViewNode>
                        </treeviewengine:TreeViewNode.ChildNodes>
                    </treeviewengine:TreeViewNode>
                    <treeviewengine:TreeViewNode Content="New South Wales" IsChecked="True">
                        <treeviewengine:TreeViewNode.ChildNodes>
                            <treeviewengine:TreeViewNode Content="Sydney"/>
                            <treeviewengine:TreeViewNode Content="New York">
                                <treeviewengine:TreeViewNode.ChildNodes>
                                    <treeviewengine:TreeViewNode Content="San Francisco"/>
                                </treeviewengine:TreeViewNode.ChildNodes>
                            </treeviewengine:TreeViewNode>

                        </treeviewengine:TreeViewNode.ChildNodes>
                    </treeviewengine:TreeViewNode>
                    <treeviewengine:TreeViewNode Content="United States of America" IsChecked="True">
                        <treeviewengine:TreeViewNode.ChildNodes>
                            <treeviewengine:TreeViewNode Content="New York">
                                <treeviewengine:TreeViewNode.ChildNodes>
                                    <treeviewengine:TreeViewNode Content="San Francisco"/>
                                </treeviewengine:TreeViewNode.ChildNodes>
                            </treeviewengine:TreeViewNode>
                            <treeviewengine:TreeViewNode Content="California">
                                <treeviewengine:TreeViewNode.ChildNodes>
                                    <treeviewengine:TreeViewNode Content="San Francisco"/>
                                </treeviewengine:TreeViewNode.ChildNodes>
                            </treeviewengine:TreeViewNode>
                        </treeviewengine:TreeViewNode.ChildNodes>
                    </treeviewengine:TreeViewNode>
                </treeviewengine:TreeViewNode.ChildNodes>
            </treeviewengine:TreeViewNode>
        </syncfusion:SfTreeView.Nodes>

        <syncfusion:SfTreeView.ItemTemplate>
            <DataTemplate>
                <ViewCell>
                    <ViewCell.View>
                        <Grid Padding="5">
                            <SfCheckBox:SfCheckBox 
                                Text="{Binding Content}"
                                IsChecked="{Binding IsChecked, Mode=TwoWay}" />
                        </Grid>
                    </ViewCell.View>
                </ViewCell>
            </DataTemplate>
        </syncfusion:SfTreeView.ItemTemplate>
    </syncfusion:SfTreeView>
</ContentPage.Content>
```

## Requirements to run the demo

To run the demo, refer to [System Requirements for Xamarin](https://help.syncfusion.com/xamarin/system-requirements)

## Troubleshooting
### Path too long exception
If you are facing path too long exception when building this example project, close Visual Studio and rename the repository to short and build the project.
