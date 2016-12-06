# My Plugin

# Requirements

Python Modules
* telepot (8.3)

# Configuration

Register your "Home-Bot" to Telegram:

* Send command "/newbot" to "BotFather" in order to create your new bot
* you will asked for a bot name and unique username 
* BotFather will send you a token (=shard secred) you will need for plugin registration in plugin.conf

## plugin.conf

plugin.conf snippet for telegram plugin

<pre>

[telegram]
        class_name = Telegram
        class_path = plugins.telegram
        token = "123456789:BBCCfd78dsf98sd9ds-_HJKShh4z5z4zh22"
        trusted_chat_ids = 123456789,9876543210

</pre>


## items.conf


### telegram_message 

Message text to broadcast if value changed


### Example

Please provide an item configuration with every attribute and usefull settings.

# items/my.conf
<pre>
[warnitem]
	name = Warn Item xy
	type = bool
	eval_trigger = ...
	telegram_message = "Windalarm!"

</pre>

## logic.conf
If your plugin support item triggers as well, please describe the attributes like the item attributes.


# Methodes
If your plugin provides methods for logics. List and describe them here...

## method1(param1, param2)
This method enables the logic to send param1 and param2 to the device. You could call it with `sh.my.method1('String', 2)`.

## method2()
This method does nothing.
