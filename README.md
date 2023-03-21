# MauiScrollViewBug

## Bug report
https://github.com/dotnet/maui/issues/14091

## Repro steps
1. Create a File->New MAUI app.
2. In MainPage.xaml
   1. Wrap the ScrollView in a Border
   2. Add enough content (e.g. Labels) to the end of the VerticalStackLayout
3. Build and run the app for iOS.

## Expected behaviour
Scrolling content into view ought to render the content.

## Actual behaviour
Content that is scrolled into view is not rendered on the iOS platform.