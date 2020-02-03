Are you ready to learn Blazor for Cross-Platform Mobile development using Mobile Blazor Bindings
  
In this article we will learn on how to getting started and work with new Mobile Blazor Binding for developing Cross-Platform Mobile application using Blazor, here in this article 
•	How to install Mobile Blazor Binding
•	we will create our first Mobile Blazor Binding Application
•	Create a simple Mobile Game application to kids to learn Alphabets with Sound.
•	Add Text to Speech functionality using the Xamarin Essentials.

On Jan 14th 2020 Microsoft introduced new Experimental Mobile Blazor Binding for developing Cross-Platform Mobile application using Blazor. Yes, for now this is only experimental release but still we can start working and play to learn on Mobile Blazor Binding to develop our Mobile application using the Blazor code. For all the C# programmer this will be great start to develop an mobile application using C# Code and not much need to know about Xamarine ,Andorid or IOS development.  
Mobile Blazor Binding is the combination of Blazor and Xamarin.Forms .UI design part is based on the Xamarin.Forms UI Controls and the components and code part is based on the Blazor. The combination of Blazor, and Xamarin.Forms allows the user to create Native Mobile app development for both IOS and Android using the Web programming pattern. All the design and code part for both Andorid and IOS can be made from the Blazor project and using the Android and IOS project the app can be run on appropriate emulator or device. 
For more details refer : https://devblogs.microsoft.com/aspnet/mobile-blazor-bindings-experiment/ 
Getting Started with Mobile Blazor Binding Application
When we create the Mobile Blazor Binding Blazor application we can see by default 3 project will be added in our solution. In solution we can find 3 projects as 
1)	Blazor Project
The Blazor project where we design our page UI and do all business logic for mobile application development using Blazor. Note for the UI design part we will be using the same Xamarin.Forms UI controls in our Razor pages.In our code part we can see more in detail about adding new page creating our own Game using Blazor code.
2)	Android Project
We can also see the Android project has been added in our solution and this project is used for building and running the Blazor application in Android Emulator or on the Android Device.
3)	IOS Project
We can also see the IOS project has been added in our solution and this project is used for building and running the Blazor application in IOS Simulator or on the IOS Device.

 
Prerequisites
In order to work with Mobile Blazor Binding You need to have .NET Core 3.0 or higher version SDK,You need to have Visual Studio or Visual Studio for Mac,ASP.NET Web Development and Mobile Development with Xamarine.Forms Workloads installed in your computer. Here for my article have installed Visual Studio 2019 latest version and used .NET Core 3.0 SDK,
Visual Studio 2019  
 .NET Core 3.0 SDK

Installing Mobile Blazor Binding Template

After Installing the prerequistes you are ready to work with Mobile Blazor Binding, but for working with Mobile Blazor Binding we need to template to be installed for this open your command prompt.
Click Windows Start: Type CMD and press enter in the command prompt.
In the command prompt enter the below code to install the Microsoft MobileBlazorBindings Templates
We need to run the below code in CMD or from the shell

dotnet new -i Microsoft.MobileBlazorBindings.Templates::0.1.173-beta

wait for few sec for the template to be installed.
 
Now we have installed the Mobile Blazor Binding Template and its time for us to create our first Mobile Blazor Binding applicaiotn.
Code part
Creating Mobile Blazor Binding Applicatoin
Click Windows Start: Type CMD and press enter in the command prompt.
From the Command prompt go to your Drive and Folder in where you want to create the applicaiotn.
Here I have created folder under D:> Drive and I will create my project under the Android/Blazor Folder.
For creating the Project in the command prompt run the below command ,
dotnet new mobileblazorbindings -o ShanuMobile
Note that ShanuMobile is the projectName ,You can add your needed project name over there.

Mobile Blazor Binding Solution Structure:
 
When we create the Mobile Blazor Binding Blazor application we can see by default 3 project will be added in our solution. In solution we can find 3 projects as 
1)	Blazor Project
The Blazor project where we design our page UI and do all business logic for mobile application development using Blazor. Note for the UI design part we will be using the same Xamarin.Forms UI controls in our Razor pages.In our code part we can see more in detail about adding new page creating our own Game using Blazor code.
 
Here we have created the project name as “ShanuMobile” has been created as the Blazor project and in this project, we can see the Microsoift.MobileBlazorBinding and Xamarin.Forms Packages has been added by default.Also the Blazor project contains the files as
•	Imports.razor
The Import.razor file has the default needed import of Xamarin.Forums and MobileBlazorBindings to create native mobile app for Android and IOS using the Xamarin.Forms with Blazor code.
 
•	App.cs
In the App.cs  class we will give the default razor page to be loaded, here in the below code we can see as HellowWorldRazor page has been added to show by default.
 
•	Counter.Razor 
By default we can see the Counter.Razor page has been added .Here in this page we can see the Xamarin.Forums UI controls has been used example like StaclkLayout also we can see the Blazor code functions has been added to perform the increment in the button click event.
 
•	HellowWorld.Razor 
In the HellowWorld razor page we can see as the page was made as the ContentPage and this page will be loaded first and added the Counter page inside the content page of Helloworld to perform the Increment functions.
 

2)	Android Project
We can also see the Android project has been added in our solution and this project is used for building and running the Blazor application in Android Emulator or on the Android Device.
 
Here we have created the project name as “ShanuMobile” and the Android project was been created by default as ShanuMobile.Android.
Here we don’t have much part to deal with as we will be adding our Balzor App in MainActivity to run our mobile application in the Android, We can also add the App display Name in Label here by default the project name has been added  in the Label ,You can change it if need also we can change the ocon for the app from the MainActivity.In order to run our Blazor app in Android mobile Device or in Emulator then set the Android project as Startup Project.
 
3)	IOS Project
We can also see the IOS project has been added in our solution and this project is used for building and running the Blazor application in IOS Simulator or on the IOS Device.
 
Here we don’t have much part to deal with as we will be adding our Balzor App in AppDelegate to run our mobile application in the IOS.In order to run our Blazor app in IOS mobile Device or in Simulator then set the IOS project as Startup Project.

 
Run the Blazor APP in Android:
Now we can see the Counter Demo in Android Device or in the Android Emulator for this first Set the Android project as Startup Project.For this right click the Android project and click on “Set as Startup Project”. You can run the application in the Android connected Device via USB or by the installed Android Emulator.
 
Here I have connected my Samsung Galaxy Not 10 mobile via USB and selected my mobile device to run the Blazor Mobile APplicatoin.You can connect to your Android device or select or Install Android Emulator to run in the emulator.
Once selected our Android Device run the application and wait for few second ,We can see our mobile application will be running in our connected Android mobile device.
  

Kids learn Alphabet Mobile Game Creation using Blazor
What is Shanu Kids Learn Alphabet Game
 
The main aim of this game is for kids age from 3 to 7 Years old to learn Alphabet. The game has functions like Each alphabet character will be display with appropriate words with image and when the Alphabet Character, Word and Image display kids can also hear the speech sound which will be more interactive and kids to learn the character as this game has all Alphabet, Word ,Image and speech sound functions. Whenever the next Alphabets are displayed kids can see the appropriate word image with sound. Kids also can listen the sound again and again for the same Alphabet by clicking the PLAY Sound button. 
For example, when the Kids Learn Alphabet apps open by default we display the Alphabet A with the Image  “Apple” and next we display the text as “A for Apple” and also play the sound pronounce as “A for Apple” ,If the kids want to listen again the pronunciation they can click on the PLAY SOUND button  when ever the users click on the “PLAY Sound” button then the corrected selected Alphabet word will be pronounced ,By this kids can learn the Alphabet easily and the image showing will be fun to kids to learn and play the Kids Learn Alphabet game again and again. This app is very simple and easy to learn for the kids. The app also has “First <<”,” Last >>”,” Next >” and “Previous <” button to show the next previous first and Last Character of the Alphabet. When the user clicks on “First <<” button then display the First Alphabet as “A” for Apple with appropriate image and sound, When the user clicks on “Last  >>” button then display the Last Alphabet as “Z” for Apple with appropriate image and sound, The  ” Next >” and “Previous <” button will display the next and previous character of the alphabet. 
In this game we will have used the Xamarin.Essentials for using the Text to Speech functionality in order to use speech functionality pronounce the Alphabet sound for making  the learning more interesting and helpful for the kids
Step 1: Game.Razor page Add:
Right click the Blazor Project and click on Add New Item and select the Razor Component and give the name as Game.razor and click Add.
 
The Added page will be look like this.
 
Step 2: Adding Xamarin.Essentials package to the Blazor Project
For using the Text to speech functionality in our Mobile Game App we need to install the Xamarin.Essentials packages to the blazor project for this right click on the Blazor project and click on Manage NUGet Packages .
 
Select Browse and search for the Xamarin Essentials and click on the Install. Wait for few second for the packages install on your project.
Adding the Alphabet Images
In our Kids learn Alphabet game we display images for the each character for this first I have download the Free to use ,Share and edit icons from the iconfinder.com all the icons here used are free for commercial purpose.we have download the all the images from Alphabet A to Z example A for Apple Image for Ball Image like this we have downloaded the image and also changed the image name same as the word for example apple means I kept the image name same as “Apple” and zebra image kept the image name same as “Zebra”
 
We can see as from Alphabet A to Z we have collected all the images and copy all this image and add to the Android project under the Drawable folder like below image
 

Step 3: Game Design Part coding
Now open the Game.Razor page and replace the code with below code for our mobile Kids Learn Alphabet design. Next we display the Image and source we bind dynamically bind to the Image from the code. By default first we bind the image as “Apple.png” and show the first image as “Apple” and next we add the label to display the text as per the Alphabet and we bind the result from the code dynamically based on the current alphabet selected by default we display the text as the “A for Apple” and next we design  the buttons for first, next, previous and last alphabet display and finally we add one more button to play the Sound of current selected alphabet words. 
<Frame CornerRadius="10" BackgroundColor="Color.Gold">

    <StackLayout Orientation="StackOrientation.Horizontal" HorizontalOptions="LayoutOptions.Center">
        <Label Text="Kids learn Alphabet Game!"
               FontAttributes="FontAttributes.Bold"
               VerticalTextAlignment="TextAlignment.Center" FontSize="25" />
    </StackLayout>

</Frame>

<Frame CornerRadius="10" BackgroundColor="Color.Yellow">
    <StackLayout Orientation="StackOrientation.Horizontal" HorizontalOptions="LayoutOptions.Center">
        <Image Source="ImageSource.FromFile(curImgName)" HeightRequest="230" WidthRequest="230" />

    </StackLayout>

</Frame>

<Frame CornerRadius="10" BackgroundColor="Color.LightGreen">
    <StackLayout Orientation="StackOrientation.Horizontal" HorizontalOptions="LayoutOptions.Center">
        <Label Text="@(curAlphabetNM)"
               FontAttributes="FontAttributes.Bold"
               VerticalTextAlignment="TextAlignment.Center" FontSize="48" />
    </StackLayout>

</Frame>


<Frame CornerRadius="10" BackgroundColor="Color.DarkBlue">
    <StackLayout Orientation="StackOrientation.Horizontal" HorizontalOptions="LayoutOptions.Center">
        <Button Text="<<" BackgroundColor="Color.LightSkyBlue" OnClick="@showFirstAlphabet" />

        <Button Text=">" BackgroundColor="Color.LightSkyBlue" OnClick="@showNextAlphabet"/>

        <Button Text="<" BackgroundColor="Color.LightSkyBlue" OnClick="@showprevAlphabet"/>
        <Button Text=">>" BackgroundColor="Color.LightSkyBlue"  OnClick="@showLastAlphabet"/>
    </StackLayout>
</Frame>

<Frame CornerRadius="10" BackgroundColor="Color.DarkKhaki">
    <StackLayout Orientation="StackOrientation.Horizontal" HorizontalOptions="LayoutOptions.Center">
        <Button Text="Play Sound" BackgroundColor="Color.LightYellow" OnClick="@playSound"/>
    </StackLayout>
</Frame>

Step 4: Game Code Part 
Now open the Game.Razor page and replace the code with below code for our mobile game code part at the bottom of the above design.
First declared all the needed variables ,here we have created to array for displaying the Character and the appropriate words. 
When user clicks on the ”First <<” button then call the showFirstAlphabet() method and display the first Array of both Alphabets and AlphabetNames and set the CurrentIndex as 0 and call the playSound() method to proncunce the selected curAlphabetNM string using the Xamarin.Essentials.TextToSpeech.SpeakAsync.
When user clicks on the ”Next >” button then call the showNextAlphabet() method and display the Next Array of both AlphabetNames from the CurrentIndex and call the playSound() method to proncunce the selected curAlphabetNM string using the Xamarin.Essentials.TextToSpeech.SpeakAsync.
When user clicks on the ”Previous <” button then call the showprevAlphabet() method and display the previous Array of both Alphabets and AlphabetNames from the  CurrentIndex and call the playSound() method to proncunce the selected curAlphabetNM string using the Xamarin.Essentials.TextToSpeech.SpeakAsync.
When user clicks on the ”Last >>” button then call the showLastAlphabet() method and display the last Array of both Alphabets and AlphabetNames and set the CurrentIndex as maxAlphabetValue and call the playSound() method to proncunce the selected curAlphabetNM string using the Xamarin.Essentials.TextToSpeech.SpeakAsync.
When “Play Sound” Button clicked call the playSound() method to proncunce the selected curAlphabetNM string using the Xamarin.Essentials.TextToSpeech.SpeakAsync. 
@code {
    String curAlphabetNM = "A for Apple";
    String curImgName = "Apple.png";

    private static readonly string[] Alphabets = new[]
         {
          "A", "B", "C", "D", "E", "F", "G", "H", "I", "J",
          "K", "L", "M", "N", "O", "P", "Q", "R", "S", "T",
          "U", "V", "W", "X", "Y", "Z"
         };

    private static readonly string[] AlphabetNames = new[]
       {
          "Apple", "Ball", "Cat", "Dog", "Elephant", "Fish", "Goat", "Hat", "IceCream", "Juice",
          "kite", "Lion", "Mouse", "Noodle", "Orange", "Pencil", "Quarter", "Rose", "Sun", "Toy",
          "Umbrella", "Van", "Watch", "Xylophone", "Yellow", "Zebra"
         };

    int CurrentIndex = 0;
    int maxAlphabetValue = 25;

    void showFirstAlphabet()
    {
        CurrentIndex = 0;
        playSound();
    }

    void showNextAlphabet()
    {
        if (CurrentIndex<maxAlphabetValue)
        {
            CurrentIndex = CurrentIndex+1;
        }

        playSound();
    }

     void showprevAlphabet()
    {
        if (CurrentIndex>0)
        {
            CurrentIndex = CurrentIndex-1;
        }

        playSound();
    }

    void showLastAlphabet()
    {
        CurrentIndex = maxAlphabetValue;
        playSound();
    }

    void playSound()
    {
        curAlphabetNM = Alphabets[CurrentIndex].ToString() + " for " + AlphabetNames[CurrentIndex].ToString();

        curImgName = AlphabetNames[CurrentIndex].ToString()+".png";

        Xamarin.Essentials.TextToSpeech.SpeakAsync(curAlphabetNM).ContinueWith((t) =>
        {
        }, TaskScheduler.FromCurrentSynchronizationContext());
    } 
} 
Step 5: Add the Game.razor page to the main Content page
In the HelloWorld we add the Game razor page in content page to load the game also we change the Title from the Hello World to “Shanu kids Game” 
 
Step 6: Run the Application in Android Device or in Emulator
Here we have used the Samsung Galaxy Not 10 Android app to run our game. You can run in any Android Device on your installed Android emulator.
  
Conclution:
Mobile Blazor Bindings is an experimental release and not for the production use. But for now, it will be good place for getting started and work with Mobile Blazor Bindings for developing native mobile app using the Blazor. This is really a needed one for all the Web Developer as well the C# lovers who are not much familiar with Native app development even not much familiar with Xamarin. We as the C# lovers will always love to work with this kind of native mobile application development that too with Blazor means it’s like and cake with more honey for us. Let’s wait for the production release till that lets experiment more with Mobile Blazor Bindings.Hope you all enjoy reading this article soon we will see with some other new interesting topic.

