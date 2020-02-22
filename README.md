# Share projects and help other AIDE users

AIDE Studio is an Android application to help developers using [Android IDE (AIDE)](https://play.google.com/store/apps/details?id=com.aide.ui) perform some tasks more quickly, as well as having some extra features that AIDE does not natively offer.
Check out [AIDE Studio on the Play Store](https://play.google.com/store/apps/details?id=com.kproject.aidestudio) for more information.

This small guide is intended to teach you how you can submit your projects so that they appear in AIDE Studio and other users can download and get to know them.

At the moment, the only restriction is that they are just Java-Android or Java-Console projects, that is, Android application projects and Java projects to run on the console. It is necessary that the project has been done or tested at AIDE and that it obviously works.

# How to send my projects?
To submit your projects, you have two options:
1. Just make a pull request in the [main JSON file](https://github.com/jsericksk/aidestudio/blob/master/repositories.json) of this repository, adding a new item at the beginning of the repository array. This item must have the same pattern as the previous ones and be filled with the data presented below.
2. Sending an email to **jsericksk@gmail.com** with the required data below. You don't have to send in a JSON format if you don't want to.

## Requirements
**url:** URL of your project's repository on GitHub.

**project_name:** The name of the project. You can use a short title or a simple name, as you prefer.

**author:** The name of the author of the project. If you are not the author but want to share the repository with other users because you used it successfully on AIDE, fill in this field with the repository's username.

**description:** Description of the project. Briefly describe its function so that users can easily understand what it is for. Remember that you can always read the README in the repository (if it exists), but it is important to fill this field with a clear and objective description so that it can appear in AIDE Studio.

**type:** The type of project. The available values ​​are 0 and 1. 0 for Java-Android projects and 1 for Java-Console projects.

**date:** The date the project was added. Always fill in this field with 0. It will be modified containing the current time in milliseconds (corresponding to System.currentTimeMillis() in Java) after the project is approved.

**Note about the name of the project and description**: It is only allowed to fill in these data in 3 languages: English, Portuguese and Spanish. To reach a larger number of users, it is preferable that it be in English, however, you can also use Portuguese or Spanish if it is your native language.

**See a small example below. Remember that you must add your project at the beginning of JSON and not at the end. New projects should always be added at the beginning.**
```
{
  "url": "https:\/\/github.com\/username\/repository-name",
  "project_name": "RecyclerView Animations",
  "author": "EricksK",
  "description": "Project containing useful methods for animating the addition/removal of items from RecyclerView.",
  "type": 0,
  "date": 0
},
{
// Other projects
}
```

## When will my project become available?
After submitting your project, it will undergo a short review and should be available in at least 72 hours. This is the maximum time for it to be published. If it exceeds this limit, for some reason it has not been approved. Some of the reasons that can cause your project not to be approved are:
- The project is not Java-Android or Java-Console.
- It is entirely written in a language other than Java.
- It's a library.
- Does not follow the rule of languages ​​allowed for the project name and description.

**Note that the quality of the projects is the responsibility of the respective developers. AIDE Studio is not responsible for any code errors contained in submitted projects.**
