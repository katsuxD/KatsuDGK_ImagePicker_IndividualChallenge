# katsudgk_image_picker

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

For help getting started with Flutter, view our
[online documentation](https://flutter.dev/docs), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Hello GDG Viet Nam and people who reading this.

I picked the 2nd challange which is Image Picker (Individual).
At the begin, I start to search the key words "How to pick image in Gallery - Flutter" 
Recently, it leads me to this post: https://androidkt.com/how-to-upload-image-using-multipart-in-flutter/
By reading this article, I have known that this is a 3rd libary which can support me to choose any pics in gallery and display it into screen by using getImage().
But this function didn't provide by Image-Picker: ^0.8.4+4 so I try to replace with the recommended "pickImage()", then I have to create a variable to save the file return.
"ImagePicker.pickImage() shows the familiar image picking screen and returns"

After that, I created a widget to display the selected Image. It's a Stack which contains the selected Image and the Camera icon to take pics if user want.
So in this step I just have to create a function to using camera by ImageSource.camera which is provided by ImagePicker to take picture from camera and add it to onPressed in Camera icon.
Finised that step, thing become more easily because I just need to create 1 more button to pass the function which I have created above to selected picture from gallery and displayed into screen . 
But in last 5days training, by reading the docs from GDG and Flutter page. I have learned a bit about state_management which is Getx and I want to try to use it in this project.
As you know GetX is a very usable to navigation or change the state data from children widgets. 
So that's why I try to create a function which is imagePickerOption() by using bottomsheet to navigate to a widget (SingleChildScrollView) which contains list buttons to show select options.
And if user pick one of these options like taking pics from camera or gallery, then it will be displayed back to the screen.

Totally this project is using:

-image_picker: ^0.8.4+4

-get: ^4.5.1


![ezgif com-gif-maker](https://user-images.githubusercontent.com/52829521/145080885-6882fb70-2145-4de9-8eea-4e840d1cd649.gif)

![1638899641914](https://user-images.githubusercontent.com/52829521/145081387-6b40fae0-8306-48a2-b08f-a23517d2c028.jpg)
![1638899641900](https://user-images.githubusercontent.com/52829521/145081394-2bf20b35-8c35-4e76-9da2-e9de886540ce.jpg)

