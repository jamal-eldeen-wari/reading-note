# Intent Filter:
Is to allow other applications to start your application and it is done by using intent filters. Now to start the application by another application we need to add to our manifest.xml intent filters.

Once the activity has intent filters means that it has to fullfilthe following criteria:
1. Action: A string naming the action to perform. Usually one of the platform-defined values such as **ACTION_SEND** or **ACTION_VIEW**.

2. Data: A description of the data associated with the intent.

3. Category: Provides an additional way to characterize the activity handling the intent, usually related to the user gesture or location from which it's started. There are several different categories supported by the system, but most are rarely used. However, all implicit intents are defined with CATEGORY_DEFAULT by default.

**VIP** is that If any two pairs of action and data are mutually exclusive in their behaviors, you should create separate intent filters to specify which actions are acceptable when paired with which data types.

