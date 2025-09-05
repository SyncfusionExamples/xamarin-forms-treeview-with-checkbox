# How to use checkbox in treeview?
This example illustrates how to use checkbox in treeview.

## About the samples

This example describes how SfTreeView works with checkbox. 

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
Visual Studio 2017 or Visual Studio for Mac.
Xamarin add-ons for Visual Studio (available via the Visual Studio installer).

## Troubleshooting
### Path too long exception
If you are facing path too long exception when building this example project, close Visual Studio and rename the repository to short and build the project.

## License

Syncfusion® has no liability for any damage or consequence that may arise from using or viewing the samples. The samples are for demonstrative purposes. If you choose to use or access the samples, you agree to not hold Syncfusion® liable, in any form, for any damage related to use, for accessing, or viewing the samples. By accessing, viewing, or seeing the samples, you acknowledge and agree Syncfusion®'s samples will not allow you seek injunctive relief in any form for any claim related to the sample. If you do not agree to this, do not view, access, utilize, or otherwise do anything with Syncfusion®'s samples.

## Conclusion

I hope you enjoyed learning about How to use checkbox in Xamarin.Forms TreeView (SfTreeView).

You can refer to our Xamarin.Forms TreeViewfeature tour page to know about its other groundbreaking feature representations and documentation, and how to quickly get started for configuration specifications.

For current customers, you can check out our components from the License and Downloads page. If you are new to Syncfusion, you can try our 30-day free trial to check out our other controls.

If you have any queries or require clarifications, please let us know in the comments section below. You can also contact us through our support forums, Direct-Trac, or feedback portal. We are always happy to assist you!