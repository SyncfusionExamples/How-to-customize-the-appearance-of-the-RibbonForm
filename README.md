# How to customize the appearance of the RibbonForm?
You can customize the appearance of each RibbonControlAdv items by setting its property “RibbonStyle” as TouchStyle and by specifying your desired color in TouchStyleColorTable and applying it to the RibbonControlAdv using ApplyTouchStyleColorTable function. For more details please refer [How to customize the appearance of RibbonForm](https://www.syncfusion.com/kb/3735/how-to-customize-the-appearance-of-items-in-ribboncontroladv).

# C#

//Object creation for TouchStyleColorTable 
TouchStyleColorTable TouchStylecolor = new TouchStyleColorTable();
//Sets the Ribbon style
this.ribbonControlAdv1.RibbonStyle = RibbonStyle.TouchStyle;
//Sets the color for Ribbon Header
TouchStylecolor.ActiveHeaderBackground = Color.White;
//Sets the color for BackStageButton
TouchStylecolor.BackStageButtonColor = Color.Blue;
//Sets the Color of the BackStageButton for Hovering
TouchStylecolor.BackStageButtonHoverColor = ColorTranslator.FromHtml("#2a8dd4");
//Sets the color of the CloseButton in BackStage visible mode
TouchStylecolor.BackStageCloseButtonBackground = Color.Red;
//Sets the color of the System Button in Backstage visible mode.
TouchStylecolor.BackStageSysytemButtonBackground = Color.White;
//Sets the color for BackStageTab.
TouchStylecolor.BackStageTabColor = ColorTranslator.FromHtml("#0272c5");
//Sets the Color of the BackStageTab for Hovering.
TouchStylecolor.BackStageTabHoverColor = ColorTranslator.FromHtml("#2a8dd4");
//Sets the color of the Button for pressed state.
TouchStylecolor.ButtonPressedColor = ColorTranslator.FromHtml("#92c0e0");
//Sets the color of the Button for hover state
TouchStylecolor.ButtonHoverColor = ColorTranslator.FromHtml("#cde6f7");
//Sets the color of the Button for checked state
TouchStylecolor.ButtonCheckedColor = ColorTranslator.FromHtml("#b1d6f0");
//Sets the color for MenuButton Arrowcolor
TouchStylecolor.MenuButtonArrowColor = Color.White;
//Sets the color for the DropDown Text
TouchStylecolor.DropDownTextForeColor = Color.Black;
//Sets the color for DropDown MenuItem.
TouchStylecolor.DropDownMenuItemBackground = ColorTranslator.FromHtml("#0272c5");
//Sets the color for DropDownSelected Item.
TouchStylecolor.DropDownSelectedTextForeColor = Color.White;
//Sets the color for DropDown
TouchStylecolor.DropDownBodyColor = Color.White;
//Sets the color for Image Margin.
TouchStylecolor.ImageMargin = Color.White;
//Sets the color for the DropDown Title
TouchStylecolor.DropDownTitleBackground = Color.LightGray;
//Sets the color for ToolStripBorder
TouchStylecolor.ToolStripBorderColor = ColorTranslator.FromHtml("#0272c5");
//Sets the color for RibbonHeader
TouchStylecolor.HeaderColor = ColorTranslator.FromHtml("#0272c5");
//Sets the color for MenuButtonArrow
TouchStylecolor.MenuButtonArrowColor = Color.White;
//Sets the color for MenuButtonArrow for hover state
TouchStylecolor.MenuButtonHoverArrowColor = Color.Red;
//Sets the color for the DropDown Title
TouchStylecolor.DropDownTitleBackground = Color.LightGray;
//Apply colors to RibbonControlAdv
this.ribbonControlAdv1.ApplyTouchStyleColorTable(TouchStylecolor);