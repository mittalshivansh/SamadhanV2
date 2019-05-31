# Permission Management system

**WorkFlow :**

**Permission Grouping**

* Permissions should be categorized for simplicity of uses. So we will have permission group which will have multiple permissions linked. For eg: Job execution use-case, we need to have multiple permissions and this job execution use-case may be assigned to multiple user profiles like operator, MS etc.
* You can think permission group as list of permission required to perform a particular use-case and a user profile is combination of these use cases.

**Permission linking to profile**

* User profile Will be linked to permission group or permissions to make it more east to create new profiles and play around it.

**Permission linking to businessLine**

* By default Business line will be linked to all permissions, we can mark permissions inactive as per the  requirement like in dcm we will mark farmer\_creation inactive.  

**First Approach :** 

At mobile permission will be fetched at 2 levels :

* First user profile permissions
* Center permissions \(at this level only inactive permissions to optimize the data\)

Mobile app will compute intersection and allow operations accordingly. 

**Second Approach :** Server will compute intersection and send the permissions to client.

 

 





