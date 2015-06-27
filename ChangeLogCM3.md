#### 3.11.2 ####
  * add support for some more dual sim devices ([issue #163](https://code.google.com/p/callmeter/issues/detail?id=#163))
  * fix default rule set for second sim if any ([issue #949](https://code.google.com/p/callmeter/issues/detail?id=#949))
  * fix closing dialog after importing ([issue #959](https://code.google.com/p/callmeter/issues/detail?id=#959))
  * fix for second bill period ([issue #956](https://code.google.com/p/callmeter/issues/detail?id=#956))
#### 3.11.1 ####
  * fix alert strings for Hungarian
  * fix some minor FCs
#### 3.11 ####
  * fix for Sony's broken android implementation
  * fix missing alerts on 80% and 100% plan usage ([issue #490](https://code.google.com/p/callmeter/issues/detail?id=#490))
  * add sim id to csv export ([issue #945](https://code.google.com/p/callmeter/issues/detail?id=#945))
#### 3.10 ####
  * fix RuleEdit for dual sim phones ([issue #898](https://code.google.com/p/callmeter/issues/detail?id=#898))
  * filter sms by sim id ([issue #163](https://code.google.com/p/callmeter/issues/detail?id=#163))
  * new default rule set with dual sim/websms/voip if available ([issue #163](https://code.google.com/p/callmeter/issues/detail?id=#163))
  * remove translation with <55% translated texts
#### 3.9.1 ####
  * handle merged plans in LogsFragment ([issue #877](https://code.google.com/p/callmeter/issues/detail?id=#877))
  * add Serbian translation (thanks to Igor Kutlarevic)
  * add Portuguese translation (thanks to Sérgio Marques)
  * update translations
#### 3.9 ####
  * show last day of bill period ([issue #856](https://code.google.com/p/callmeter/issues/detail?id=#856))
  * fix multi sim on ZTE V970 ([issue #163](https://code.google.com/p/callmeter/issues/detail?id=#163))
  * confirm deleting plans/rules ([issue #853](https://code.google.com/p/callmeter/issues/detail?id=#853))
  * tune widget layout
#### 3.8.4 ####
  * fix % in number groups ([issue #833](https://code.google.com/p/callmeter/issues/detail?id=#833))
  * set widget color directly ([issue #834](https://code.google.com/p/callmeter/issues/detail?id=#834))
  * minor fixes
  * update translations
#### 3.8.3 ####
  * show confirmation when deleting groups ([issue #827](https://code.google.com/p/callmeter/issues/detail?id=#827))
  * sort plans/rules by buttons instead of menu entries ([issue #828](https://code.google.com/p/callmeter/issues/detail?id=#828))
  * add russian translation (massive thanks to Dmitriy Rublev)
  * update translations
#### 3.8.2 ####
  * hide total stats by default ([issue #812](https://code.google.com/p/callmeter/issues/detail?id=#812))
  * hide amount for "total merger plans" ([issue #633](https://code.google.com/p/callmeter/issues/detail?id=#633))
  * include/exclude numbers for MMS ([issue #775](https://code.google.com/p/callmeter/issues/detail?id=#775))
  * fix showing total cost in bill period ([issue #819](https://code.google.com/p/callmeter/issues/detail?id=#819))
#### 3.8.1 ####
  * fix limit calculation for cost limits ([issue #553](https://code.google.com/p/callmeter/issues/detail?id=#553))
  * fix mixed plans merging data plans ([issue #802](https://code.google.com/p/callmeter/issues/detail?id=#802))
  * fix cost in mixed plans merging other plans ([issue #801](https://code.google.com/p/callmeter/issues/detail?id=#801))
#### v3.8 ####
  * show users' rules in app
  * fix custom bill mode settings
  * update translation
#### v3.7.2 ####
  * fix import of rules with "longdescription" ([issue #790](https://code.google.com/p/callmeter/issues/detail?id=#790))
#### v3.7.1 ####
  * fix cost in merged plans (reset stats please) ([issue #785](https://code.google.com/p/callmeter/issues/detail?id=#785))
  * fix progress bar size for android 3+ ([issue #774](https://code.google.com/p/callmeter/issues/detail?id=#774))
  * some more fixes ([issue #773](https://code.google.com/p/callmeter/issues/detail?id=#773))
#### v3.7 ####
  * fix limit breaking calls/data ([issue #301](https://code.google.com/p/callmeter/issues/detail?id=#301))
  * fix cost settings help for plans without limit ([issue #365](https://code.google.com/p/callmeter/issues/detail?id=#365))
  * merge data in mixed plans ([issue #619](https://code.google.com/p/callmeter/issues/detail?id=#619))
  * hide progressbar for unlimited bill periods ([issue #707](https://code.google.com/p/callmeter/issues/detail?id=#707))
  * strip anything but first x seconds ([issue #629](https://code.google.com/p/callmeter/issues/detail?id=#629), [issue #712](https://code.google.com/p/callmeter/issues/detail?id=#712))
  * deleting last call will stay deleted until reset stats ([issue #764](https://code.google.com/p/callmeter/issues/detail?id=#764))
  * fix & in exports ([issue #770](https://code.google.com/p/callmeter/issues/detail?id=#770))
  * fix numbers/hours imports ([issue #771](https://code.google.com/p/callmeter/issues/detail?id=#771))
  * fix hidden help/summary
  * fix float cost limits
  * minor fixes
#### v3.6.4 ####
  * fix FC on some samsung phones ([issue #767](https://code.google.com/p/callmeter/issues/detail?id=#767))
  * fix out of memory exception
  * minor fixes ([issue #765](https://code.google.com/p/callmeter/issues/detail?id=#765))
#### v3.6.3 ####
  * basic dual sim support ([issue #163](https://code.google.com/p/callmeter/issues/detail?id=#163))
  * export/impor XML file
  * fix moving plans/rules ([issue #746](https://code.google.com/p/callmeter/issues/detail?id=#746))
  * add widget for "last log" ([issue #755](https://code.google.com/p/callmeter/issues/detail?id=#755))
  * fix some FCs
  * minor fixes
#### v3.6.2 ####
  * fix FC when exporting rules
  * fix some more settings ([issue #735](https://code.google.com/p/callmeter/issues/detail?id=#735))
#### v3.6.1 ####
  * fix cost settings ([issue #733](https://code.google.com/p/callmeter/issues/detail?id=#733))
#### v3.6 ####
  * export logs as csv file ([issue #719](https://code.google.com/p/callmeter/issues/detail?id=#719))
  * reimplement preferences
  * fix minor bugs
  * update translations
#### v3.5.1 ####
  * fix some FCs
  * fix dark theme
  * fix titles in main view ([issue #711](https://code.google.com/p/callmeter/issues/detail?id=#711))
#### v3.5 ####
  * update ActionBarScherlock 4.1
  * prepare for android 4.1 aka. jelly bean
  * fix some FCs ([issue #703](https://code.google.com/p/callmeter/issues/detail?id=#703) and more)
  * update translations
#### v3.4.2 ####
  * fix 31d bill period ([issue #665](https://code.google.com/p/callmeter/issues/detail?id=#665))
  * update translations
#### v3.4.1 ####
  * show past bill periods as 100% ([issue #662](https://code.google.com/p/callmeter/issues/detail?id=#662))
  * fix import/export of rules with new and old bill periods
#### v3.4 ####
  * add bill period length 14d 15d 31d 1m+1d ([issue #650](https://code.google.com/p/callmeter/issues/detail?id=#650))
  * fix merged cost limits ([issue #579](https://code.google.com/p/callmeter/issues/detail?id=#579))
  * minor UI fixes ([issue #626](https://code.google.com/p/callmeter/issues/detail?id=#626), [issue #658](https://code.google.com/p/callmeter/issues/detail?id=#658))
  * remove stale widgets ([issue #630](https://code.google.com/p/callmeter/issues/detail?id=#630))
  * text in number groups ([issue #625](https://code.google.com/p/callmeter/issues/detail?id=#625))
  * fix prepaid cost in widget ([issue #640](https://code.google.com/p/callmeter/issues/detail?id=#640))
  * show up to 20plans in "ask for plans" activity ([issue #643](https://code.google.com/p/callmeter/issues/detail?id=#643))
#### v3.3.1 ####
  * fix FC on android 1.6
#### v3.3 ####
  * fix FC on android 1.6
  * fix sorting plans/rules ([issue #606](https://code.google.com/p/callmeter/issues/detail?id=#606))
  * fix sum of cost for multi bill period plans ([issue #594](https://code.google.com/p/callmeter/issues/detail?id=#594))
  * fix accuracy of data stats (esp. for samsung devices) ([issue #603](https://code.google.com/p/callmeter/issues/detail?id=#603))
  * fix widget for galaxy nexus ([issue #610](https://code.google.com/p/callmeter/issues/detail?id=#610))
  * configure existing widgets
  * add widget for bill period ([issue #332](https://code.google.com/p/callmeter/issues/detail?id=#332))
  * show intro for new users
  * data stats for acer e130 ([issue #615](https://code.google.com/p/callmeter/issues/detail?id=#615))
#### v3.2.2 ####
  * fix FC
  * update translations
#### v3.2.1 ####
  * fix FC ([issue #602](https://code.google.com/p/callmeter/issues/detail?id=#602))
  * fix unlimited bill periods
  * add data log record ([issue #604](https://code.google.com/p/callmeter/issues/detail?id=#604))
  * fix color of in widget ([issue #605](https://code.google.com/p/callmeter/issues/detail?id=#605))
  * update translations
#### v3.2 ####
  * improve performance ([issue #592](https://code.google.com/p/callmeter/issues/detail?id=#592))
  * fix setting text size
  * fix donation view ([issue #593](https://code.google.com/p/callmeter/issues/detail?id=#593))
  * fix date and cost format in logs view ([issue #595](https://code.google.com/p/callmeter/issues/detail?id=#595))
#### v3.1 ####
  * RECALCULATON OF STATS NEEDED! this will take some time
  * disable rules ([issue #584](https://code.google.com/p/callmeter/issues/detail?id=#584))
  * more filters in logs view ([issue #548](https://code.google.com/p/callmeter/issues/detail?id=#548), [issue #549](https://code.google.com/p/callmeter/issues/detail?id=#549))
  * major change in design ([issue #414](https://code.google.com/p/callmeter/issues/detail?id=#414))
  * major change in database queries ([issue #579](https://code.google.com/p/callmeter/issues/detail?id=#579), [issue #587](https://code.google.com/p/callmeter/issues/detail?id=#587))
  * update translations
#### v3.0.1 ####
  * minor fix release
#### v3.0 ####
  * generic traffic for FroYo+ devices ([issue #464](https://code.google.com/p/callmeter/issues/detail?id=#464), [issue #527](https://code.google.com/p/callmeter/issues/detail?id=#527), [issue #547](https://code.google.com/p/callmeter/issues/detail?id=#547))
  * import rule sets from sd card ([issue #372](https://code.google.com/p/callmeter/issues/detail?id=#372))
  * update translations
#### v3.0 rc15 ####
  * fix data stats ([issue #509](https://code.google.com/p/callmeter/issues/detail?id=#509))
  * fix some minor FCs
#### v3.0 rc14 ####
  * simple preferences for default rule set
  * reimport default rule set, exlucde numbers for default rule set
  * add support for a601 and htc thunderbolt
  * update translations
  * minor fixes
#### v3.0 rc13 ####
  * Fix Samsung Phones ([issue #480](https://code.google.com/p/callmeter/issues/detail?id=#480))
  * Translate Default Rule Set
#### v3.0 rc12 ####
  * Fix Samsung Galaxy S 2
#### v3.0 rc11 ####
  * show icon / small widget (thanks to luca niccoli for both)
  * update translations
#### v3.0 rc10 ####
  * set text size/color in widget ([issue #314](https://code.google.com/p/callmeter/issues/detail?id=#314))
  * set background color in widget ([issue #398](https://code.google.com/p/callmeter/issues/detail?id=#398))
  * add support for LG-P990 ([issue #432](https://code.google.com/p/callmeter/issues/detail?id=#432))
  * rename data stats by default ([issue #441](https://code.google.com/p/callmeter/issues/detail?id=#441))
  * update translation
#### v3.0 rc9 ####
  * Add support for GT-S5830 and possible all future samsung devices ([issue #426](https://code.google.com/p/callmeter/issues/detail?id=#426))
  * major inner changes ([issue #400](https://code.google.com/p/callmeter/issues/detail?id=#400))
  * update translations
#### v3.0 rc8 ####
  * fix an other sunday bug ([issue #373](https://code.google.com/p/callmeter/issues/detail?id=#373))
  * allow to split messages at fixed 160 chars  ([issue #370](https://code.google.com/p/callmeter/issues/detail?id=#370))
  * fix messages to yourself ([issue #386](https://code.google.com/p/callmeter/issues/detail?id=#386))
  * add support for GT-I5510 ([issue #390](https://code.google.com/p/callmeter/issues/detail?id=#390))
  * fix custom currency symbol  ([issue #402](https://code.google.com/p/callmeter/issues/detail?id=#402))
#### v3.0 rc7 ####
  * fix data logs ([issue #346](https://code.google.com/p/callmeter/issues/detail?id=#346))
  * fix sunday ([issue #373](https://code.google.com/p/callmeter/issues/detail?id=#373))
  * fix limit+cost for merged+mixed plans  ([issue #292](https://code.google.com/p/callmeter/issues/detail?id=#292), [issue #293](https://code.google.com/p/callmeter/issues/detail?id=#293))
  * add remote number for MMS ([issue #367](https://code.google.com/p/callmeter/issues/detail?id=#367))
  * update translations
  * add help
#### v2.9.6 ####
  * fix info toast after call
  * set custom delimiter / fix delimiter ([issue #358](https://code.google.com/p/callmeter/issues/detail?id=#358))
  * add mon-fri for hour groups
  * allow <1 units in mixed plans ([issue #292](https://code.google.com/p/callmeter/issues/detail?id=#292))
  * fix limit+cost for mixed+merged plans ([issue #292](https://code.google.com/p/callmeter/issues/detail?id=#292), [issue #293](https://code.google.com/p/callmeter/issues/detail?id=#293))
  * export/backup number groups, hour groups, logs ([issue #184](https://code.google.com/p/callmeter/issues/detail?id=#184), [issue #203](https://code.google.com/p/callmeter/issues/detail?id=#203))
#### v2.9.5 ####
  * set date+time for start of billing period ([issue #258](https://code.google.com/p/callmeter/issues/detail?id=#258), [issue #345](https://code.google.com/p/callmeter/issues/detail?id=#345))
  * improve data logging ([issue #346](https://code.google.com/p/callmeter/issues/detail?id=#346))
  * match (inter-)national numbers (enter your prefix in preferences) ([issue #349](https://code.google.com/p/callmeter/issues/detail?id=#349))
  * show today\'s stats ([issue #242](https://code.google.com/p/callmeter/issues/detail?id=#242))
  * allow multi bill period merger ([issue #56](https://code.google.com/p/callmeter/issues/detail?id=#56))
  * show call info after hanging up ([issue #318](https://code.google.com/p/callmeter/issues/detail?id=#318))
#### v2.9.4 ####
  * hide progress bars ([issue #328](https://code.google.com/p/callmeter/issues/detail?id=#328))
  * add bill periods: 4,5,6,12 month
  * strip leading zeros ([issue #266](https://code.google.com/p/callmeter/issues/detail?id=#266))
  * hide no cost plans
#### v2.9.3 ####
  * Integrate with sipdroid >1.6.1
  * default update interval: 60m
  * fix MMS counter
  * fix mixed+merged limits
  * progressbar color
  * add chinese translation
#### v2.9.2 ####
  * Delete old logs (default: 90days)
  * multiselection on groups ([issue #298](https://code.google.com/p/callmeter/issues/detail?id=#298))
  * fix NPE
#### v2.9.1 ####
  * Fix cost for long sms ([issue #279](https://code.google.com/p/callmeter/issues/detail?id=#279))
  * fix cost when reaching limit
  * set name/shortname for widget ([issue #249](https://code.google.com/p/callmeter/issues/detail?id=#249))
  * show cost in widget ([issue #218](https://code.google.com/p/callmeter/issues/detail?id=#218))
  * show billperiod in widget ([issue #218](https://code.google.com/p/callmeter/issues/detail?id=#218))
  * settable sizes ([issue #245](https://code.google.com/p/callmeter/issues/detail?id=#245))
  * don't bill first x seconds ([issue #261](https://code.google.com/p/callmeter/issues/detail?id=#261))
  * merge plans ([issue #262](https://code.google.com/p/callmeter/issues/detail?id=#262))
  * hide empty plans
#### v2.8.10 ####
  * Integration with WebSMS
  * set custom locale
#### v2.8.9 ####
  * clean groups in rules
  * fix numbergroups
  * fix adding logs
  * fix import from file
  * reduce collected traffic data
#### v2.8.8 ####
  * fix for GT-I5500 ([issue #246](https://code.google.com/p/callmeter/issues/detail?id=#246))
  * fix cost for data ([issue #251](https://code.google.com/p/callmeter/issues/detail?id=#251))
  * decimal limit ([issue #248](https://code.google.com/p/callmeter/issues/detail?id=#248))
#### v2.8.7 ####
  * Fix length of billing period
#### v2.8.6 ####
  * Fix some FCs
  * hide total stats ([issue #227](https://code.google.com/p/callmeter/issues/detail?id=#227))
  * prepaid plans ([issue #86](https://code.google.com/p/callmeter/issues/detail?id=#86))
  * set textsize
  * manipulate logs by hand ([issue #189](https://code.google.com/p/callmeter/issues/detail?id=#189))
  * fix some more bugs ([issue #224](https://code.google.com/p/callmeter/issues/detail?id=#224))
  * add 60/15 bill mode ([issue #222](https://code.google.com/p/callmeter/issues/detail?id=#222))
#### v2.8.5 ####
  * Fix default displaying values for pans/rules
#### v2.8.4 ####
  * Fix some FCs
  * fix number groups with more than one entry
  * readd druch, spanish and portuguese translations
#### v2.8.3 ####
  * Fix excluded numbers
#### v2.8.2 ####
  * Simplify rules (You must reset them!)
  * fix export
  * fix NPEs
  * set update interval
  * set beginning of record
#### v2.8.1 ####
  * Add default rule sets
  * reduce complexity for simple setups
  * some changes to gui
  * force internal install
#### v2.7.3 ####
  * Fix uneditable fields
  * fix FC for empty bill modes
  * allow to hide title bar
  * readd polish+russion translation
#### v2.7.2 ####
  * History
  * alert
  * widget
  * total expense
  * ...
#### v2.7.1 ####
  * Custom date format
  * currency format/symbol
  * speedup boot/shutdown process
  * changing color of limit bars
  * new screens for plans/rules
#### v2.7.0 ####
  * Initial alpha of Call Meter 3G
  * Major architecture refactoring