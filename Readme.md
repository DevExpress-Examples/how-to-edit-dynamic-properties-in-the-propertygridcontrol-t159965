<!-- default file list -->
*Files to look at*:

* [CustomPropertyDescriptor.cs](./CS/PropertyGridWithDictionary/CustomPropertyDescriptor.cs) (VB: [CustomPropertyDescriptor.vb](./VB/PropertyGridWithDictionary/CustomPropertyDescriptor.vb))
* [DictionaryWrapper.cs](./CS/PropertyGridWithDictionary/DictionaryWrapper.cs) (VB: [DictionaryWrapper.vb](./VB/PropertyGridWithDictionary/DictionaryWrapper.vb))
* [MainWindow.xaml](./CS/PropertyGridWithDictionary/MainWindow.xaml) (VB: [MainWindow.xaml](./VB/PropertyGridWithDictionary/MainWindow.xaml))
* [MainWindow.xaml.cs](./CS/PropertyGridWithDictionary/MainWindow.xaml.cs) (VB: [MainWindow.xaml.vb](./VB/PropertyGridWithDictionary/MainWindow.xaml.vb))
<!-- default file list end -->
# How to: Edit Dynamic Properties in the PropertyGridControl


The PropertyGridControl supports the standard<a href="https://msdn.microsoft.com/en-us/library/system.componentmodel.icustomtypedescriptor%28v=vs.110%29.aspx"> ICustomTypeDescriptor</a> interface. To be able to display dynamic properties, you can implement this interface in the data source class and pass the instance of this class to <a href="https://documentation.devexpress.com/#WPF/DevExpressXpfPropertyGridPropertyGridControl_SelectedObjecttopic">PropertyGridControl.SelectedObject</a>.<br>
<p>In this example, this interface is implemented in the DictionaryWrapper<T> class. In the GetProperties methods, it returns a collection of custom <a href="https://msdn.microsoft.com/en-us/library/system.componentmodel.propertydescriptor%28v=vs.110%29.aspx">PropertyDescriptor</a> descendants.</p>

<br/>


