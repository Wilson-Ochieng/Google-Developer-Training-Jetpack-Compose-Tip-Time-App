###TESTS

Testing, in the context of software, is a structured method of checking your software to make sure that it works as expected. Automated testing is code that checks to ensure that another piece of code that you wrote works correctly.

Testing is an important part of the app development process. By running tests against your app consistently, you can verify your app's correctness, functional behavior, and usability before you release it publicly.

Testing also provides a way to continuously check the existing code as changes are introduced.

While manual testing almost always has a place, testing in Android can often be automated. Throughout the remaining course, you focus on automated tests to test the app code and the functional requirements of the app itself. In this codelab, you learn the very basics of testing in Android. In later codelabs, you learn more advanced practices of testing Android apps.

As you become familiar with Android development and testing Android apps, you should make it a regular practice to write tests alongside your app code. Creating a test every time you create a new feature in your app reduces your workload later as your app grows. It also provides a convenient way for you to make sure your app works properly without spending too much time manually testing your app.

Automated testing is an essential part of all software development and Android development is no exception. As such, there's no better time to introduce it than right now!

Why automated tests are important
At first, it might seem like you don't really need tests in your app, but testing is needed in apps of all sizes and complexities.

To grow your codebase, you need to test existing functionality as you add new pieces, which is only possible if you have existing tests. As your app grows, manual testing takes much more effort than automated testing. Furthermore, once you start working on apps in production, testing becomes critical when you have a large user base. For example, you must account for many different types of devices running many different versions of Android.

Eventually, you reach a point where automated tests can account for the majority of usage scenarios significantly faster than manual tests. When you run tests before you release new code, you can make changes to the existing code so that you avoid the release of an app with unexpected behaviors.

Remember that automated tests are tests executed through software, as opposed to manual tests, which are carried out by a person who directly interacts with a device. Automated testing and manual testing play a critical role in ensuring that users of your product have a pleasant experience. However, automated tests can be more precise and they optimize your team's productivity because a person isn't required to run them and they can be executed much faster than a manual test.

Type of automated tests
Local tests
Local tests are a type of automated test that directly test a small piece of code to ensure that it functions properly. With local tests, you can test functions, classes, and properties. Local tests are executed on your workstation, which means they run in a development environment without the need for a device or emulator. This is a fancy way to say that local tests run on your computer. They also have very low overhead in terms of computer resources, so they can run fast even with limited resources. Android Studio comes ready to run local tests automatically.

Instrumentation tests
In the context of Android development, an instrumentation test is a UI test. Instrumentation tests let you test parts of an app that depend on the Android API, and its platform APIs and services.

Unlike local tests, UI tests launch an app or part of an app, simulate user interactions, and check whether the app reacted appropriately. Throughout this course, UI tests are run on a physical device or emulator.

When you run an instrumentation test on Android, the test code is actually built into its own Android Application Package (APK) like a regular Android app. An APK is a compressed file that contains all the code and necessary files to run the app on a device or emulator. The test APK is installed on the device or emulator along with the regular app APK. The test APK then runs its tests against the app APK.

Read More Here:https://developer.android.com/courses/pathways/android-basics-compose-unit-2-pathway-3#codelab-https://developer.android.com/codelabs/basic-android-kotlin-compose-write-automated-tests