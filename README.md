import 'package:flutter/material.dart';

class DeveloperProfileScreen extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: SingleChildScrollView(
        child: Column(
          children: [
            Image.network('https://1.bp.blogspot.com/-7A4WynwLsMw/XbBpCXG8fHI/AAAAAAAAMt4/uOa1bpLskYgrwGbllhSu2SDj_Mig8SXJQCLcBGAsYHQ/s1600/2000_600px.gif'),
            SizedBox(height: 16),
            Text(
              'Hi 👋, I\'m Md. Sohel Rana',
              style: TextStyle(fontSize: 24, fontWeight: FontWeight.bold),
              textAlign: TextAlign.center,
            ),
            Text(
              'A passionate App Developer from Bangladesh',
              style: TextStyle(fontSize: 16),
              textAlign: TextAlign.center,
            ),
            SizedBox(height: 20),
            Image.network(
              'https://cdn.dribbble.com/users/730703/screenshots/6581243/avento.gif',
              width: 400,
              height: 185,
              fit: BoxFit.cover,
            ),
            Padding(
              padding: const EdgeInsets.all(16.0),
              child: Column(
                crossAxisAlignment: CrossAxisAlignment.start,
                children: [
                  Text('🔭 I’m currently working on Flutter.'),
                  Text('🌱 I’m learning more about App Development.'),
                  Text('💬 Ask me about C, Dart, Flutter, Java, Android.'),
                  Text('📫 Reach me at sohelrana.diucse@gmail.com'),
                ],
              ),
            ),
            SizedBox(height: 20),
            Text('Languages and Tools', style: TextStyle(fontSize: 20, fontWeight: FontWeight.bold)),
            Wrap(
              spacing: 10,
              children: [
                Image.network('https://raw.githubusercontent.com/devicons/devicon/master/icons/android/android-original-wordmark.svg', width: 40),
                Image.network('https://raw.githubusercontent.com/devicons/devicon/master/icons/c/c-original.svg', width: 40),
                Image.network('https://www.vectorlogo.zone/logos/dartlang/dartlang-icon.svg', width: 40),
                // Add more icons here
              ],
            ),
            SizedBox(height: 20),
            Text('GitHub Stats', style: TextStyle(fontSize: 20, fontWeight: FontWeight.bold)),
            Image.network('https://github-readme-stats.vercel.app/api/top-langs?username=sohelrana-cse&show_icons=true&locale=en&layout=compact'),
            Image.network('https://github-readme-streak-stats.herokuapp.com/?user=sohelrana-cse'),
          ],
        ),
      ),
    );
  }
}
