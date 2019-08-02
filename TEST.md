---
title: Notifications
scope: Global
excerpt: Notifications are an essential communication tool for informing users about various events happening both inside and outside of the Sprout tool that may require their attention and action. 
contact: Nicki Stearns
private: true
---

By delivering users real-time information that they’ve self-identified as important to channels that they’ve selected, we’re both promoting user efficiency and supporting experience personalization. In order to ensure an optimal Notifications experience for every user, all team members building notifications must strive for consistency in respect to design, delivery channels, and technical implementation.

### Best Practices

**Does my feature need a notification?**
Notifications should be transactional meaning they should alert the user about something they need to be aware of or that they need to do. If your feature has recurring, event-based information out-puts that will improve an individual users’ awareness or performance within our tool, you might want to consider creating a notification. While there is no clear-cut criteria for whether or not you should create a Notification, before pursuing, you should have a clear answer to the question, “Why does my user need to receive this piece of information in various ways outside of the direct feature area on an ongoing basis?”

**Notifications are most effective when…**

- They alert a user to something that they could not have quickly known on their own
- They succinctly present users with the necessary information 
- They can navigate a user closer to where they need to be in order to take an action
- They are not overwhelming in either frequency or volume 
- Users can control if or how they want to receive them

**Considerations when building notifications**

- Where, on click, will the notification take the user? 
    - What are the deep-link options available? How close can we get the user to the action?
- Have we built a notification variant for each delivery channel we support: Email, Notification Center, and Mobile Push?
- Have we added preferences for the notification in the Notification Settings Table within the desktop application?
- What does the entire lifecycle look like for this notification? 
    - Will the notification ever become “stale” at any point? *(ie the deep-link you’ve attached to the notification no longer exists)*
    - What will happen if the notification is acted upon or resolved on one device and not another *(ie resolved on mobile but not desktop)*?
- What metadata are we presenting to the user within the notifications?
    -  Will they have a clear understanding from a quick glance about what has happened or what needs to happen?
- How does this fit into the larger notification ecosystem? [See list of active notifications](https://docs.google.com/spreadsheets/d/1c-PY0yELKclgMz1IoKM5ufxeVGsgQc8zrbQV6YNaAKM/edit#gid=639599714)


### Types

There are several types of notifications:

**Notifications**
This is the most common type of notification in the notification center. These notifications are user-to-user, meaning they are sent when one user takes an action and another user is notified. This type of notification is minimal disruptive and interactive.

**Issues**
Issue notifications are a type of notification sent from the Sprout system. These notifications are usually related to problems with an account, such as disconnected profiles. This type of notification is minimal disruptive, can hold more specific helper text to guide the user and may or may not be actionable depending on user permissions.

**Banners**
Banner notifications are persistent and cannot be dismissed until the issue is resolved. These are notifications from the system, usually related to issues that degrade part of an experience, such as failed posts, API issues from a single network, etc.

**Dialogs**
Dialog notifications are for degraded experiences that prevent the user from using Sprout as intended. Examples of these experiences:

- Credit card has expired and user is locked out of application.
- Trial has ended and user hasn’t upgraded to a plan.
- User has canceled plan and no longer has access.

### Triggers & Behavior

There are two primary ways notifications are triggered:

1. **User-based:** An action taken by another Sprout user in your account ecosystem fired off an event that alerted you. These will be referred to as "Notifications".
    - Example *“Tom F. assigned you a post for Approval”*
2. **System-based:** An action by Sprout Social fired off an event that alerted you. These will be referred to as "Issues".
    - External Example: *“Your Instagram Profile needs reauthorization.”* 
    - Internal Example: *“Your credit card on file is set to expire in 14 days”* 

Notifications have a menu containing, "Mark as read" or "Mark as unread" and "Delete". On click, a notification will navigate the user to the page the notification is referencing, at that time, the notification will transition to the read style card. "Mark as read" and "Mark as unread" will transition the notification between the unread and read card style (see Structure & Style section). On delete, the notification will exit out of the notification center. See [*Message Feeds*](https://sproutsocial.com/seeds/patterns/message-feeds) for details on how notifications should enter and exit the Notification Center.

Issues have a "Learn more" button. On click, the Issue will expand and display more details related to the issue. For certain issues, the user may see a button at the bottom of the details allowing them to take an action. A user will only see this button if they have appropriate permissions to take an action on the issue.

### Structure & Style

There are two styles of cards that may appear within the notification center:

**Notifications**
Notifications will be structured with an icon (to indicate type), sender’s avatar, sender’s name, request, overflow menu icon and byline. A notification byline should always include the group name and timestamp. Timestamp will appear by hours until 24 hours, at that point it will convert to the abbreviated date format, month date year (*e.g.* Jul 1, 2019).

**Unread, Unseen**
Unread, unseen notifications appear within the notification center after action is initated by another user.

![](https://paper-attachments.dropbox.com/s_F5B7E0DD23239649D3E02D939F99CDD77FF5741A0DD8F8AEE8E8D89CFCC6CE6F_1564752581535_Notification+Unread+Unseen.png)

**Unread, Seen**

![](https://paper-attachments.dropbox.com/s_F5B7E0DD23239649D3E02D939F99CDD77FF5741A0DD8F8AEE8E8D89CFCC6CE6F_1564752593333_Notification+Unread+Seen.png)

**Read, Seen**

![](https://paper-attachments.dropbox.com/s_F5B7E0DD23239649D3E02D939F99CDD77FF5741A0DD8F8AEE8E8D89CFCC6CE6F_1564752601874_Notification+Read+Seen.png)

******Issues**
Issues should always have a red warning icon, profile / network’s name, status, details and byline. An Issue byline should always include the network and abbreviated date format, month date year (*e.g.* Jul 1, 2019). Issues may or may not have a profile’s avatar.

- Example of an Issue with avatar: *“Sprout Coffee Co is disconnected”*
- Example of an Issue without an avatar: *“Facebook is experiencing issues”*

*Note: Issues do not have an unread state.*

**Read, Collapsed**

![](https://paper-attachments.dropbox.com/s_F5B7E0DD23239649D3E02D939F99CDD77FF5741A0DD8F8AEE8E8D89CFCC6CE6F_1564752621429_Issue+Read+Collapsed.png)


**Read, Expanded with Button**

![](https://paper-attachments.dropbox.com/s_F5B7E0DD23239649D3E02D939F99CDD77FF5741A0DD8F8AEE8E8D89CFCC6CE6F_1564752635550_Issue+Read+Expanded.png)


**Read, Expanded without Button (no permissions)**

![](https://paper-attachments.dropbox.com/s_F5B7E0DD23239649D3E02D939F99CDD77FF5741A0DD8F8AEE8E8D89CFCC6CE6F_1564752654180_Issue+No+Button.png)


**No Avatar**

![](https://paper-attachments.dropbox.com/s_F5B7E0DD23239649D3E02D939F99CDD77FF5741A0DD8F8AEE8E8D89CFCC6CE6F_1564752661907_Issue+No+Avatar.png)


### Do's & Don’ts

- **DO:** Use notifications if information is time sensitive and there are consequences if left unresolved
- **DO:** Use notifications if the information is pivotal to workflows within Sprout
- **DO:** Use notifications if information is pivotal to user-to-user interactions and collaboration within Sprout
- **DON'T:** Use notifications if the information is already assumed in the feature’s core functionality
- **DON'T:** Use notifications to explicitly promote feature awareness, usage or adoption


### Building and releasing a new notification

**Who should see notifications?**
Notifications can be released to both trial users and subscribers that have the adequate feature access in respect to plan availability and permissions. 

**How can my team build a notification?**
For any additional product, design, and technical implementation details please refer to this Notification Framework Document. 

**Who can I reach out to for assistance if I need it?**
The Global tribe, specifically the Capabilities squad, oversees the Notification service, Notification Center, and Notification Settings. Hop into #eng-global and mention @capabilities so we can be sure to give you attention.


### Q&A

| **Question**                                                                                                      | **Answer**                                                                                                                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| How are notifications scoped?                                                                                     | Notifications are scoped at the user level across groups & customers.                                                                                                                                                                    |
| Will permissions be kept the same?                                                                                | Yes, users can only receive notifications on events they are able to access                                                                                                                                                              |
| What will it be like if you have only a few groups versus many groups?                                            | We have contextualized experiences that differ depending on the amount of groups the user is in to cater to their unique needs.                                                                                                          |
| What are the different states of a notification?                                                                  | New, Seen, and Read                                                                                                                                                                                                                      |
| If you already saw a notification on your mobile device, will it also appear in the desktop notifications center? | This and all other decisions related to a notification’s lifecycle will be the responsibility of the individual squad to decide. The service will provide internal users state control over notifications: New, Seen, Read, and Deleted. |
| What happens if you click on a notification?                                                                      | You will be taken away from the page you’re currently on and into an area relevant to the notification.                                                                                                                                  |