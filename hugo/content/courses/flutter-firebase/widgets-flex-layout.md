---
title: Flex Layout
description: Align widgets in rows and columns
weight: 13
lastmod: 2019-05-13T10:23:30-09:00
draft: false
emoji: 🐦
vimeo: 336025145
---

## Example Code

{{< file "dart" "main.dart" >}}
{{< highlight dart >}}
class MyApp extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
   return MaterialApp(
     home: Scaffold(
       body: Container(
         color: Colors.blue,
         padding: EdgeInsets.all(16),
         child: Column(
           mainAxisAlignment: MainAxisAlignment.center,
           crossAxisAlignment: CrossAxisAlignment.stretch,
           children: <Widget>[
             Icon(Icons.cake, color: Colors.white, size: 50,),
             Icon(Icons.cake, color: Colors.white, size: 100,),
             Icon(Icons.cake, color: Colors.white, size: 200,),
           ],
         )
       )
     ),
   );
 }
}

{{< /highlight >}}