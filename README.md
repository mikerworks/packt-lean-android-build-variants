# Android build variants sample

It is not unlikely that you will need to deliver more than one version of your app. In fact, it could be a smart thing to deliver your app under multiple names, each with a different look and feel. It is great for targeting more than one audience. Another example is that of delivering a light and paid (or free and pro) version of an app. Although a flavour often is used to customize the look and feel, there is no reason why you could it not use it for enabling or disabling features.

In addition to a particular flavour, you might need to create build types with different configurations. Think of an app that is communicating against a backend. You probably want to test your app with a different endpoint than the one you use for your app in production. That allows you to safely test your app without the need to worry that it will mess up your production data. 

The term “build flavour” is reserved for customization where the build type is for configuration purposes. The combination of a flavour and a build type is called a “build variant”.

We can use multiple Gradle tasks to build each variant.

# Lean mobile app development book

This sample is described in chapter 18 about Continuous Integration and delivery (CI/CD) in the book 'Lean mobile app development'. It will arrive by the end of this year.

In this chapter we will see how we can organize a workflow in which we automate the process of testing and delivering your app.  You can do this for both the beta and the public releases of your app.  To make the build-measure-feedback loop really work you, you need to release early and often. 

You can install Jenkins or TeamCity on a build server or another dedicated machine to make a new build of your app each time a new feature becomes available. Basically it comes down to that but there are many interesting strategies to consider. For example: What is your branching strategy (git workflow)? Do you want to run unit or UI-tests on the build server? How can you support variants (Android) or targets (iOS) for your app? Let’s find out in this chapter.
We will have a look at various tools that can help us with the ad hoc distribution of the app. 