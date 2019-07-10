--Readme document for *author(s)*, *email(s)*, *UCI id(s)*--
JONATHAN JUAREZ, jonatj3@uci.edu, 74242436
EMERY VALENCIA, emvalenc@uci.edu, 59325878

1. How long, in hours, did it take you to complete this assignment?
20 hours


2. What online resources did you consult when completing this assignment? (list specific URLs)
https://formidable.com/open-source/victory/guides/animations/
https://formidable.com/open-source/victory
http://docs.nativebase.io
http://facebook.github.io/react-native/

3. What classmates or other individuals did you consult as part of this assignment? What did you discuss?
None. We only discussed this with one another.


4. Is there anything special we need to know in order to run your code?
Run npm install.
You must install the EXPO CLI to run the React Native app. Instructions are below. You can run this on an emulator or on your personal cellphone by downloading 
the EXPO app and scanning the QR code.

************************EXPO INSTALLATION INSTRUCTIONS***********************
npm install -g expo-cli
npm install  <------ for project dependencies
then finally expo start in the root folder which is ./sleepAppnea
*****************************************************************************

--Aim for no more than a few sentences for each of the following questions.--

NOTE:
To render charts we used static data instead of actual user data for testing. 
The issue is that user data is always logged on the same day unless the user is actively using the app for days. To get around this we just resorted to
static data to be rendered until we connect a database to retrieve data.


5. Did you design your app with a particular type of user in mind? If so, whom? Did you design your app specifically for iOS or Android, or both?
We designed our app to be simple and minimalistic, which makes it easy for users of all backgrounds to use it. We added some accessibility labels to our buttons as 
well. The application uses NativeBase (UX Library) which claims to look the same on both iOS and Android with only minor settle differences like alerts being the 
iOS default and Android, respectively.

6. How can a person log overnight sleep in your app? Why did you choose to support logging overnight sleep in this way?
We utilize a Date-Time component that brings up a calendar once the "log start time" button is clicked. This allows users to 
select the start date of their sleep followed by the start time for their sleep.

They then log their end time which repeats a similar process once the "log end time" is clicked.

We decided utilize this type of entry method because the component uses the iOS or Android native calendar and time selectors. This approach in intuitive
to users since they won't need to learn a new way to enter data.

7. How can a person log sleepiness during the day in your app? Why did you choose to support logging sleepiness in this way?
Users log data by interacting with a slider component. The slider allows an easy way to undo, select, and log data. There is very little error that can
occur while using sliders and the responsiveness is instant.

We also added a dynamic changing of slider colors when the user slides to larger or smaller sleepiness values to provide more feedback.


8. How can a person view the data they logged in your app? Why did you choose to support viewing logged data in this way?
On the navigation bar we have a "Logs" section that contains our logged data. When you click on it, it displays the sleepiness data in an animated bar graph using 
Formidable's Victory library. We decided to implement the sleepiness data logged throughout the day as an average per day. That average is updated as you log more 
sleepiness ratings. Below the sleepiness rating graph is a list that shows your overnight logged sleep data. It shows the date, when you started sleeping, and when 
you stopped sleeping. We decided to support viewing our data this way because it was minimalistic yet informative and we really like the design. A minimalistic
design with a night-sky coloration theme is what we were aiming for, as this app is about sleepiness. 

9. Did you add any "extra" features, such as other data to log or changes to the styling of the app? If so, what did you add? How do these add to the experience of the app?
- Added login and signup buttons (to be implemented)
- Added helper "?" icons on the sleep tracker and sleepiness tracker screen that displays info to the user about that particular screen 
- Added a slider that changes color from pink to a bright seafoam green when moved around
- Added a graph animation to the sleepiness average rating graph in the Logs tab/LogScreen
- Accessibility labels on buttons
- Implemented this in React Native :)


LATE HOURS: 2 hours from Emery Valencia (1 day if you don't include this README change as a day :)  )
