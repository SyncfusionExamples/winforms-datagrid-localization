# WinForms DataGrid Localization

This repository contains sample which shows localization of Syncfusion [WinForms DataGrid](https://www.syncfusion.com/winforms-ui-controls/datagrid) (SfDataGrid).


You can [localize](https://help.syncfusion.com/windowsforms/localization#localize-syncfusion-windows-forms-control-using-resx-file) the `WinForms DataGrid` by adding resource file for each language.

### Changing application culture

When you are changing the application culture, then you can localize the application based on application culture by creating .resx file.

``` csharp
public partial class Form1 : Form
{
    public Form1()
    {
        Thread.CurrentThread.CurrentCulture = new System.Globalization.CultureInfo("de-DE");
        Thread.CurrentThread.CurrentUICulture = new System.Globalization.CultureInfo("de-DE");
        InitializeComponent();
    }
}
```

### Creating .resx files

You can create .resx files for any languages by following steps,

1. Right click your project and click `New Folder` and set name as `Resources`.

2. Add [Windows Forms Control Localization default resource files](https://github.com/syncfusion/winforms-controls-localization-resx-files) of libraries you are using into `Resources` folder.

3. Now, right click on `Resources` folder and select `Add` and then `New Item`. In the `Add New Item wizard`, select Resources File option and name the file name as `Syncfusion.SfDataGrid.WinForms.<culture name>.resx` for German culture. For example, you have to give name as `Syncfusion.SfDataGrid.WinForms.de-DE.resx` for `German` culture. In the same way, add new resource files for other libraries used in your application.

4. Now, select Add and add resource file for `German` culture in `Resources` folder.

5. Now, you can copy the key names from default resource files and change its corresponding value based on the culture.