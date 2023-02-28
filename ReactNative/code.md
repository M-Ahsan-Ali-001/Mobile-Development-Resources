# Starter
~~~
// Hybrid vs native => https://rb.gy/tzo6gz
// In hybrid app we use web technologies to develop mobile apps it makes development fast , but theyare slow in speed.  

// Expo go
//terminal code
npx create-expo-app projectname
npm start

~~~

# Core components
~~~
view
Image
Textinput
ScrollView

~~~

# Community components
~~~ 
React Navigation
React Native Screens
React Native Maps
React natives Videos

~~~
# React Native Header with button
~~~
import { StatusBar } from 'expo-status-bar';
import { useState } from 'react';
import { Button, StyleSheet, Text, View } from 'react-native';

function LittleLemonHeader(prope)
{
   
   let [val,chgVal] =useState(prope.txt)
   let chng = ()=>{
    chgVal("Value has been Changed!")
   }
return (
    <View >
        <Text> A {val}</Text>
        <Button title='Click' onPress={chng} />
    </View>
)

}
export default LittleLemonHeader;

~~~
