# THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS:


ersistent local storage is one of the areas where native client applications have held an advantage over web applications. For native applications, the operating system typically provides an abstraction layer for storing and retrieving application-specific data like preferences or runtime state.

# A BRIEF HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5:
In the beginning, there was only Internet Explorer. Or at least, that’s what Microsoft wanted the world to think. To that end, as part of the First Great Browser Wars, Microsoft invented a great many things and included them in their browser-to-end-all-browser-wars, Internet Explorer. One of these things was called DHTML Behaviors, and one of these behaviors was called userData.

userData allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure. (Trusted domains, such as intranet sites, can store 10 times that amount. And hey, 640 KB ought to be enough for anybody.) IE does not present any form of permissions dialog, and there is no allowance for increasing the amount of storage available.

# USING HTML5 STORAGE:
HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.

interface Storage { getter any getItem(in DOMString key); setter creator void setItem(in DOMString key, in any data); };

# TRACKING CHANGES TO THE HTML5 STORAGE AREA
If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something. For example, if you set an item to its existing value or call clear() when there are no named keys, the storage event will not fire, because nothing actually changed in the storage area.

# STORAGEEVENT OBJECT
| |PROPERTY TYPE DESCRIPTION| |:——:|:——————-:| |key|string the named key that was added, removed, or modified| |oldValue| any the previous value (now overwritten), or null if a new item was added| |newValue| any the new value, or null if an item was removed| |url*| string the page which called a method that triggered this change|

# LIMITATIONS IN CURRENT BROWSERS
In talking about the history of local storage hacks using third-party plugins, I made a point of mentioning the limitations of each technique, such as storage limits. I just realized that I haven’t mentioned anything about the limitations of the now-standardized HTML5 Storage. I’ll give you the answers first, then explain them. The answers, in order of importance, are “5 megabytes,” “QUOTA_EXCEEDED_ERR,” and “no.”
HTML5 STORAGE IN ACTION
Data is stored as strings. If you are storing something other than a string, you’ll need to coerce it yourself when you retrieve it.
BEYOND NAMED KEY-VALUE PAIRS: COMPETING VISIONS
While the past is littered with hacks and workarounds, the present condition of HTML5 Storage is surprisingly rosy. A new API has been standardized and implemented across all major browsers, platforms, and devices. As a web developer, that’s just not something you see every day, is it? But there is more to life than “5 megabytes of named key/value pairs,” and the future of persistent local storage is… how shall I put it… well, there are competing visions.
One vision is an acronym that you probably know already: SQL. In 2007, Google launched Gears, an open source cross-browser plugin which included an embedded database based on SQLite. This early prototype later influenced the creation of the Web SQL Database specification. Web SQL Database (formerly known as “WebDB”) provides a thin wrapper around a SQL database, allowing you to do things like this from JavaScript:
WEB SQL DATABASE SUPPORT:

IE : .
1. FIREFOX : .
2. SAFARI : 4.0+
3. CHROME : 4.0+
4. OPERA : 10.5+
5. IPHONE : 3.0+
6. ANDROID : 2.0+