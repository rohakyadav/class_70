##### Topic Automatically populating text input

● Customize the appearance of the bottom tabs by adding custom icons/images to it. 

● Design the input form for the issue/return screen of the app. 

● Write code to automatically populate the input box when book id and student id are scanned.

there are two additional options passed down in createBottomTabNavigator - defaultNavigationOptions and

tabBarOptions.

tabBarOptions take the colors which you want in the bottom tabs to appear when they are active or inactive.

One of the navigation options is tabBarIcon. tabBarIcon returns components which you want to use as an icon in your bottom tab navigation.

This object contains a field called defaultNavigationOptions - which currently returns an empty object. Note that the function gets passed navigation object as argument by default.

The tabBarIcon should return a component (depending on the tab which is selected).

● focused: Returns true when the tab is tapped. Returns false otherwise. 

● horizontal: Returns true when the device is in landscape mode. Returns false if the device is in portrait mode. 

● tintColor: Returns the active set tintColor.

Navigation object which is passed down during function call, contains routeName property inside its state.

routeName property changes depending on which screen is active in the app. 

● If Transaction Screen is active, routeName equals "Transaction" 

● If Search Screen is active, routeName equals "Search" We need to return different components depending on which tab is active.