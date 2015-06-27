## How to read the colors? ##

There are tree colors used to indicate your usage:

  * red: your limit is reached by at least 100%
  * yellow: your limit is used more than your billing period. this means when using your limit with the same speed, you will end up red. eg. at the half of the month, you used more than half of your limit.
  * green: everything is good

## What are these bill modes? ##

xx/yy means the first xx seconds are billed. no matter how long the call takes.
The next billing periods are yy seconds long.

Some examples:
  1. a call with a duration of 45s is billed as
    * 60s with 60/yy
    * 45s with 30/1
    * 50s with 30/10
    * 30s with 30/0
  1. a call with a duration of 65s is billed as
    * 60s with 60/0
    * 65s with xx/1
    * 70s with xx/10
    * 120s with 60/60

## My plan starts at x. Not at the 1st of each month. How do I set that? ##
You need to set up the bill period.
A shortcut is long pressing the bill period in main view.
Set the "bill date" to whatever you need.

## I get billed every x days/months. How do I set that? ##
You need to set the bill period's length
A shortcut is long pressing the bill period in main view.
Set the "bill period length" to whatever you need.

## What should I set the cost / call/sms/mb to? ##
You should set it in your main currency eg. 0.09€/SMS.
You need to set it with a "." regardless of your locale (This is a bug in android itself).

## How do I set fixed package cost? ##
There is an option in each plan. If you pay for the whole thing, just set it to the bill period.

## Why is data traffic incorrect? ##
The Android system itself does not collect traffic statistics. This app reads the information directly from the linux kernel. This is why statistics from before last reboot is unavailable.
Additionally traffic stats may vary with our provider's.

## Is there a way to distinguish between WLAN/WIFI and 2G/3G/4G traffic? ##
This app currently does count 2G/3G/4G traffic only.
It never gathered any WIFI stats.
Please see [issue #120](https://code.google.com/p/callmeter/issues/detail?id=#120) for furthor information.

## How do I exclude a few numbers from a plan? ##
  1. Go to the Rules view.
  1. Look for "exclude numbergroups".
  1. Add/Edit a numbergroup:
    * Add all numbers you want to be excluded to the group
    * Wildcards are allowd. E.g. add +491% and 01% to exclude all German mobile numbers.
  1. Go back to the rule and select the created the number group.

## How do I bill a few numbers different from the rest? (calls and txt, premium number, preminum sms, local vs. mobile calls, international calls, ...) ##
A common setup for example for calls billed differently by number:
  1. Add a second plan for outgoing calls.
  1. Add a second rule for outgoing calls. Set the new plan as it's target.
  1. Add a number group which handles all calls of one of these plans. E.g. add 0800% and 00800% to a group of free numbers.
  1. Exclude the number group in one rule, make sure, the rule your numbers are excluded is listed above of the other rule.
This basic setup is a common pattern an is needed for quite a few configurations.
A good starting point/example is the preconfigured rule set for splitting landline/mobile calls in germany:
http://www.ub0r.de/android/callmeter/rulesets/#f_00_split_outgoing_calls_into_mobilelandline_plans

## I have free minutes every day. How do I set that? ##
This setup is a little bit more complicated, but feasable:
  1. Add a second bill period with lenth of 1 day
  1. Add a socond plan for outgoing calls. Set its bill period to the new from above. Set its limit and cost to whatever you want.
  1. Set the old outgoing calls plan to merge the new plan added above.
  1. Set the exising rule for outgoing calls to target the new plan from above.

## I use viber. Why are viber calls counted? How can I stop that? ##
Currently there is no way to distingues viber call logs from android call logs.
There is an public interface to CM3 to notify CM3 about the internet calls.
Viber is not using this interface so far.
Please drop a mail at viber's support and point them to me.
A few real VoIP apps did implement the interface already.

## I'm using WebSMS/Sipdroid/CSsimple to send txt message/call over the internet. What can I do to ignore these logs? ##
There is an public interface to CM3 to notify CM3 about the internet calls/websms.
WebSMS, SMSdroid and CSsimple are known to implement this interface to notify CM3 about the fake logs they write.
You can filter these logs in the rules with the "Is WebSMS"/"Is SIP call" setting.

There are example rules for both of this:
http://www.ub0r.de/android/callmeter/rulesets/#f_00_exclude_WebSMS__Sipdroid

## I have two SIM cards, switching them regulary. How to handle that? ##
Most SIM cards are showing their phone number to the phone.
If yours is doing that, you can set "my number" to any rule to match only logs, when the given SIM card is active.
This check is done live. If you reset stats, or just installed the app, it won't work.

## How do I set up Call Meter with dual SIM phones? ##
Although more and more dual SIM phones are flooding the market, Android itself does not have any API to handle more than one SIM card.
Anything you have is proprietary for your phone/manufacturer. That's why the answer is not that easy.
Most users asking me about dual SIM had an additional column in their call log database: simId.
If your phone has that id, CM3 shows the id of the call log entry in the logs view (swipe to the right from the main view).
If your phone has that id, you might set this id to any rule targeting calls.
E.g. you could set one outgoing call rule for sim 0, one for sim 1.
As far as I know, this simId does only exist for call logs. There is no way to split neither txt messages nor data traffic by simId.

## Is there any way to backup and restore the statistics (e.g. when changing the phone)? ##
There are 3 ways to backup/restore your stats/configuration.
  1. If your phone is rooted, you could use some app like TitanimBackup to do this like with any other app.
  1. To save call logs and txt stats, you could use apps like SMSBackupREstore and CallLogBackupRestore.
    * These apps will backup your android internal data for later restore.
    * When restoring these data, you need to tell CM3 to throw away all it's data and reread it from android's internal data source.
    * If you are moving to a new phone without any call logs or messages, your are just done.
    * One devices, where CM3 has gathered any tats already, you need to select the "reset stats" menu option in CM3.
    * Please note: As The android system is not saving traffic stats (or at least is not giving that away), this does not include data stats.
  1. You can export your rules and your logs:
    * Export rules and logs.
    * Choose to send it by mail to yourself or copy the files from SD card
    * Open these two files with CM3 on your new device for later restore. Any rule or log inside your CM3 installation will get replaced.

## Why does the app need network-based location access? ##
It's just for the ads provided by admob.
If you are afraid of this apps behavior, you should check out the source code.
As this is an open source project, the source is available for everyone!

## How do I import preconfigured rule sets? ##
Just visit http://www.ub0r.de/android/callmeter/rulesets/ with your phone or PC. Select any of the rule sets.

When viewing with PC, the barcode let's you import the rule set on your phone.
When viewing with your phone, you can just click the direct link.

## How does this whole thing work? ##
Basically there are 3 parts to understand:
  1. There is the LogRunner running in background every now and then collecting information from your device and storing them in a database.
  1. There are Plans. This is where you set cost, limits, bill modes etc.
  1. There are Rules. These rules define, which log is billed in which plan to show up on may screen.


## Please add... ##
Please post your feature request as issue:
http://code.google.com/p/callmeter/issues/list

## I have a question which is not listed here... ##
I really can not read all the comments down there. I only check them every few month.
There is even no way to respond to any of the questions.

Please file an issue:
http://code.google.com/p/callmeter/issues/list
I'll try to help as soon as possible.